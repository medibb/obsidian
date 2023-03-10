r과 shiny로 서명받는 앱 만드는 법 알려줘

서명을 받는 앱을 만들기 위해서는 다음과 같은 단계를 따르면 됩니다.

1. R 설치

우선 R을 설치해야 합니다. R은 데이터 분석 및 통계에 사용되는 오픈 소스 프로그래밍 언어입니다. R을 다운로드하려면 https://cran.r-project.org/ 에 접속하면 됩니다.

2. Shiny 패키지 설치

Shiny는 R에서 웹 애플리케이션을 개발할 수 있는 패키지입니다. Shiny를 설치하려면 아래와 같은 명령어를 입력하세요.

```
install.packages("shiny")
```

3. 서명 기능 구현

서명 기능은 htmlwidgets 패키지에서 제공하는 signature_pad 위젯을 사용하여 구현할 수 있습니다.

```
library(shiny)
library(htmlwidgets)

ui <- fluidPage(
  tags$head(tags$script(src="https://cdn.jsdelivr.net/npm/signature_pad@2.3.3/signature_pad.min.js")),
  tags$div(id = 'signature', style = "width:500px; height:250px;")
)

server <- function(input, output) {
  observe({
    signature <- htmlwidgets::createWidget("signature_pad", list(), width = 500, height = 250)
    session$sendCustomMessage(type = 'signature', list(signature))
  })
}

shinyApp(ui, server)
```

위 코드에서는 Shiny의 UI 부분에서 signature_pad 위젯을 불러오고, 서버 부분에서 observe 함수를 이용하여 signature_pad 위젯의 값을 받아오게 됩니다.

4. 서명 저장하기

서명이 완료되면 저장 버튼을 눌러서 서버에 저장합니다.

```
library(shiny)
library(htmlwidgets)

ui <- fluidPage(
  tags$head(tags$script(src="https://cdn.jsdelivr.net/npm/signature_pad@2.3.3/signature_pad.min.js")),
  tags$div(id = 'signature', style = "width:500px; height:250px;"),
  actionButton("save", "Save")
)

server <- function(input, output) {
  
  observe({
    signature <- htmlwidgets::createWidget("signature_pad", list(), width = 500, height = 250)
    session$sendCustomMessage(type = 'signature', list(signature))
    
    observeEvent(input$save, {
      dataURI <- signature$get()
      dataURI <- gsub("^data:image/png;base64,", "", dataURI) # PNG 이미지 데이터 추출
      writeBin(base64Decode(dataURI), "signature.png") # 파일로 저장
    })
    
  })
}

shinyApp(ui, server)
```

위 코드에서는 Save 버튼 클릭 시 서명 이미지를 PNG 형식으로 저장합니다.

5. 서명 기록 확인하기

마지막으로 서명 기록 확인 기능을 추가해 보겠습니다.

```
library(shiny)
library(htmltools)

ui <- fluidPage(
  
  tags$head(tags$script(src="https://cdn.jsdelivr.net/npm/signature_pad@2.3.3/signature_pad.min.js")),
  
  tags$h1("서명"),
  
  tags$div(id = 'signature', style = "width:500px; height:250px;"),
  
  actionButton("save", "Save"),
  
  br(),
  
   uiOutput("signatures")
)


server <- function(input