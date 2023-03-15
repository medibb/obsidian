import turtle

## 전역 변수 부분 ##
num1, num2, result = 0, 0, 0
swidth, sheight = 1000, 300
curX, curY = 0, 0


##메인 코드 부분 ##
       
if __name__ == "__main__" :
    turtle.title("심화문제10")
    turtle.shape('turtle')
    turtle.setup(width = swidth + 50, height = sheight + 50)
    turtle.screensize(swidth, sheight)
    turtle.penup()
    turtle.left(90)


    num1 = int(input("숫자를 입력하세요 : "))
    num2 = int(input("숫자를 하나 더 입력하세요 : "))
    num3 = num1 & num2
    num = [num1, num2, num3]
    binary = [bin(num1), bin(num2), bin(num3)]
    length = [len(bin(num1)), len(bin(num2)), len(bin(num3))]
    curX = swidth / 2
    curY = 100
    for i in range(3) :
        curY -=50
        for j in range(int(length[i])-2) :
            turtle.goto(curX, curY)
            if num[i] & 1 :
                turtle.color('red')
                turtle.turtlesize(2)
            else : 
                turtle.color('blue')
                turtle.turtlesize(1)
            turtle.stamp()
            curX -= 50
            num[i] >>= 1

turtle.done()

코드 오류 설명해줘

1. 들여쓰기 오류: 파이썬에서는 코드 블록을 들여쓰기로 구분하기 때문에 들여쓰기 오류가 발생합니다. 예를 들어, 메인 코드 부분에서 for 문이 실행될 때 range() 함수에 인자값을 지정하지 않아서 에러가 발생합니다.

2. 변수명 중복: 변수명이 중복되는 경우가 있습니다. 예를 들어, 리스트의 이름과 리스트 내부의 값들을 저장하는 변수의 이름이 같아서 구분이 어렵습니다.

3. 타입 에러: range() 함수의 인자값은 정수형만 가능합니다. 하지만, length[i]는 리스트 내부의 문자열 값입니다.

4. turtle 모듈 사용 방법: turtle 모듈에서 turltesize() 함수는 거북이의 크기를 조절하는 함수입니다. 하지만, 이 함수는 색상과 관련된 기능은 없습니다. 따라서, 색상을 바꾸기 위해서는 pencolor() 함수나 fillcolor() 함수를 사용해야 합니다.

5. for 문 실행 범위: for i in 3 이라고 되어 있지만, 실제로는 i에 0, 1, 2가 저장됩니다. 따라서 range(3)으로 수정해야 합니다.

6. 형식 오류: 마지막 줄에 있는 'turtle.done()'은 띄어쓰기 없이 작성되어 있습니다. 따라서 'turtle.done ()'으로 수정해야 합니다.

import turtle
## 전역 변수 부분 ##
num1, num2, result = 0, 0, 0
swidth, sheight = 1000, 300
curX, curY = 0, 0


##메인 코드 부분 ##
       
if __name__ == "__main__" :
    turtle.title("심화문제10")
    turtle.shape('turtle')
    turtle.setup(width = swidth + 50, height = sheight + 50)
    turtle.screensize(swidth, sheight)
    turtle.penup()
    turtle.left(90)


    num1 = int(input("숫자를 입력하세요 : "))
    num2 = int(input("숫자를 하나 더 입력하세요 : "))
    num3 = num1 & num2
    num_list = [num1, num2, num3]
    binary_list = [bin(num1), bin(num2), bin(num3)]
    length_list = [len(bin(num1)), len(bin(num2)), len(bin(num3))]
    
    curY = 100
    
    for i in range(3):
        curX = swidth / 2
        curY -=50
        for j in range(length_list[i]-2) :
            turtle.goto(curX, curY)
            if num_list[i] & 1 :
                turtle.color('red')
                turtle.turtlesize(2)
            else : 
                turtle.color('blue')
                turtle.turtlesize(1)
            turtle.stamp()
            curX -= 50
            num_list[i] >>= 1

turtle.done()