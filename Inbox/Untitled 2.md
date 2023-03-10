show me the  r & shiny code acting as follow: showing 'pain diagram' to user, user draw a simple annotation, and save the picture

Unfortunately, as an AI language model, I am not able to provide visual outputs. However, I can give you the code for a basic R Shiny app that allows the user to draw on an image and save it as a file. 

Here's an example code for you:

```
library(shiny)

# Define UI
ui <- fluidPage(
  titlePanel("Pain Diagram"),
  sidebarLayout(
    sidebarPanel(
      actionButton("clear", "Clear"),
      br(),
      downloadButton("downloadData", "Download")
    ),
    mainPanel(
      plotOutput("plot1", click = "plot_click")
    )
  )
)

# Define server logic
server <- function(input, output) {
  
  # Load pain diagram image
  img_url <- "https://www.painscale.com/media/uploads/pain_scale_diagram_2.jpg"
  img <- readPNG(img_url)
  
  # Initialize variables
  clicked_points <- reactiveValues()
  
  # Draw plot with image
  output$plot1 <- renderPlot({
    plot(1:10, type = "n", axes = FALSE, xlab = "", ylab = "")
    rasterImage(img, xleft = 0.5, ybottom = 0.5, xright = 9.5, ytop = 9.5)
    
    # Add points if clicked by user
    if (!is.null(clicked_points$x)) {
      points(clicked_points$x, clicked_points$y, col = "red", pch = 16)
    }
    
    # Clear points if button is clicked
    observeEvent(input$clear,{
      clicked_points$x <- NULL
      clicked_points$y <- NULL
    })
    
    # Save image if button is clicked
    output$downloadData <- downloadHandler(
      filename = function() {
        paste0("pain_diagram_", Sys.Date(), ".png")
      },
      
      content = function(file) {
        png(file)
        plot(1:10, type = "n", axes = FALSE, xlab = "", ylab = "")
        rasterImage(img, xleft = 0.5, ybottom = 0.5, xright = 9.5, ytop=9.5)
        if (!is.null(clicked_points$x)) {
          points(clicked_points$x,
                 clicked_points$y,
                 col="red",
                 pch=16)
        }
        dev.off()
      }
      
    )
    
  })
  
   # Record clicks on plot and store in reactiveValues object 
   observeEvent(input$plot_click,{
     click_x <- round(input$plot_click$x)
     click_y <- round(input$plot_click$y)
     if(click_x <8 & click_x>2 & click_y <8 & click_y>2){
       isolate({
         clicked_points$x<-c(clicked_points$x,
                             input$plot_click$x)
         clicked_points$y<-c(clicked_points$y,
                             input$plot_click$y)}
       )
     }
     
   })
}

# Run the application 
shinyApp(ui=ui , server=server )
```

This code will display a pain diagram image in the center of the app window and allow the user to draw on it using their mouse cursor. Whenever the user clicks on the image with their mouse cursor in a specific area (between (2-8), (2-8)), a red dot will be placed at that location.

The 'Clear' button allows users to clear all previous annotations made on the picture.

The 'Download' button saves an image of the annotated pain diagram as a PNG file with a filename following `pain_diagram_<date>.png` where `<date>` is replaced by today's date.

Users can use this code to create their own Shiny app that displays any other images they want to annotate and save annotations made by users as