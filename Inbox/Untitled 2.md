r, shiny, HTML5 Canvas로 그림그리는 앱 만드는 법 알려줘

1. R Shiny 앱을 만들기 위해 RStudio를 열고 새 프로젝트를 생성합니다.

2. Shiny 패키지를 설치합니다.

```
install.packages("shiny")
```

3. 앱을 위한 파일을 생성합니다.

- ui.R : 사용자 인터페이스를 정의하는 파일입니다.
- server.R : 서버 측 로직을 정의하는 파일입니다.

4. ui.R 파일에서 HTML5 Canvas를 추가하기 위해 다음 코드를 추가합니다.

```R
library(shiny)

shinyUI(fluidPage(
  tags$canvas(id = "myCanvas", width = "500", height = "500")
))
```

5. server.R 파일에서 그림 그리기 기능을 추가하기 위해 다음 코드를 추가합니다.

```R
library(shiny)

shinyServer(function(input, output) {
  
  observe({
    session$sendCustomMessage("clearCanvas", "")
  })
  
  observe({
    session$sendCustomMessage("drawLine", list(x1 = input$x0, y1 = input$y0, x2 = input$x1, y2 = input$y1))
  })
})
```

6. JavaScript 코드를 추가하기 위해 www 폴더를 만듭니다.

7. www 폴더에 app.js 파일을 생성하고 다음 코드를 작성합니다.

```JavaScript
$(document).ready(function(){
  
  var canvas = document.getElementById("myCanvas");
  var context = canvas.getContext("2d");
  
  // Clear canvas
  Shiny.addCustomMessageHandler("clearCanvas",
    function(message) {
      context.clearRect(0, 0, canvas.width, canvas.height);
    }
  );
  
  // Draw line
  Shiny.addCustomMessageHandler("drawLine",
    function(message) {
      context.beginPath();
      context.moveTo(message.x1, message.y1);
      context.lineTo(message.x2, message.y2);
      context.stroke();
    }
  );
  
});
```

8. 앱을 실행하고 그림 그리기 기능을 사용해보세요!

이제 R Shiny와 HTML5 Canvas로 간단한 그림 그리기 앱을 만들어 보았습니다! 이 방법은 다양한 기능과 사용자 인터페이스를 포함할 수 있으므로 확장할 수 있습니다.