-   `Title:` [[⌨️Hotkeys]]
-   `Type:` [[=]]
-   `Tags:` #🧠️/⚙️ 
-   `Formation Date:` [[2023-02-01]]
---



# Obsidian
- crtl + o - travel to another note
- art + E - templator
- ctrl + V - paste link in clipboard
- ctrl + + - emoji

# HWP
- Shift + ESC , Enter : 표 밖으로 커서 꺼내기
- Crtl + Enter: 쪽 나누기 

---

# Microsoft
## Window
- window + SPACE : 입력기 전환 (==한영전환 안될때==)
- window + b : 알림영역
	- window + b + -> + SPACE + End  : ==음소거할때==
- window + u : 접근성 센터 ('추가 디스플레이 설정 클릭'으로 ==디스플레이 설정 들어갈때==)
- window + a : 알림창
- window + Shift + 화살표: 한번에 모니터 끼리 이동

## Windows Explorer
- Ctrl + Shift + n : 새폴더 생성
- F2 : 이름바꾸기 
	- Tab 하면 이동
- F4 : 주소창 목록보기 
	- Alt + Shift + d : 주소창으로 포커스
	- Alt  + f + numkeys : ==자주가는 폴더 ==
- Alt + p : 내용 미리보기
- Alt + Enter : 파일 속성 표시

## Word
- Ctrl + Shift + N: 표준 스타일 적용
- Ctrl + Shift + C: 서식 복사
- Ctrl + Shift + V: 서식 붙여넣기

## PPT
- Alt + 숫자(빠른실행메뉴) : (ESC + Enter 로 글자색 변경에 사용)

---

# Google
## Chrome / Edge
-  F6 : 주소창 혹은 툴바로 포커스 전환 (==북마크바로 이동할때 3번 클릭==)
- Alt + D : 주소창으로 바로 이동
- Shift + Alt + t : 툴바의 첫 번째 항목에 포커스 설정
- F10 : 툴바의 가장 오른쪽에 있는 항목(창옵션)에 포커스 설정
- F12 + Ctrl + Shift + M : 모바일모드 보기 (==고신닥터스 사용시==)
- alt + HOME : HOME 페이지 열기

## Gmail
- 대화선택 x
- 삭제 #
- 사이드바와 받은편지함 간 전환 Ctrl + Alt + , (==Todoist 사용==) 
- 목록으로 돌아가기 u ( 또는 , + enter)
- 커서를 툴바로 ,
- 마지막작업 취소 z
- 편지쓰기
	- 새편지 c
	- 답장 r
	- 새창에서 답장 Shift + r
	- (숨은)참조추가 Ctrl + Shift + c(b)
	- 전달 f

---

# Zotero
- Ctrl + Shift + C : 내보내기 설정 스타일로 복사



# 마크다운 문법 


## 줄 바꾸는 법

---
<br> 혹은 문장의 마지막에서 스페이스 두번 후 엔터

무궁화 꽃이 피었습니다.무궁화 꽃은 너무나 아름답게 피었습니다.  
무궁화 꽃이 피었습니다.무궁화 꽃은 너무나 아름답게 피었습니다. 무궁화 꽆이 피었습니다. 문장은 엔터로 띄어서 썼으나 붙여서 출력됩니다. 밑줄을 표현하기 위해서는 문장은 <br>혹은 공백 2칸이 필요합니다.  
이렇게 말입니다.

```
&lt;br&gt; 혹은 문장의 마지막에서 스페이스 두번 후 엔터

무궁화 꽃이 피었습니다.무궁화 꽃은 너무나 아름답게 피었습니다.<br>
무궁화 꽃이 피었습니다.무궁화 꽃은 너무나 아름답게 피었습니다.
무궁화 꽆이 피었습니다. 문장은 엔터로 띄어서 썼으나 붙여서 출력됩니다.
밑줄을 표현하기 위해서는 문장은 &lt;br&gt;혹은 공백 2칸이 필요합니다.  
이렇게 말입니다.
```

    
  
  

## list를 표현하는 법

---

-   list 1
-   list 2
-   list 3
-   list 4
    -   list 5
        -   list 5-1
        -   list 5-2
    -   list 6
        -   list 6-1
        -   list 6-2

```
- list 1
- list 2
- list 3
* list 4
    - list 5
        + list 5-1
        + list 5-2
    - list 6
        + list 6-1
        + list 6-2  
```

    
1.  list 1
2.  list 2
3.  list 3

```
1. list 1
2. list 2
3. list 3
```

    

## dl dt dd 표현

---

레시피

1.레시피를 표현하는 방법

```
<dl><dt>레시피</dt><dd>1.레시피를 표현하는 방법</dd></dl>
```

  
  
  

## table을 표현하는 법

---

| th | th | th |
|---|---|---|
| 지원 | 미지원 | 지원
| 미지원 | 지원 | 지원   
| 미지원 | 지원 | 지원   

```
| th | th | th |
|---|---|---|
| 지원 | 미지원 | 지원
| 미지원 | 지원 | 지원   
| 미지원 | 지원 | 지원   
```

   
  

## 문장 요소 표현

---

**강조**<br>
*강조*<br>
~~ddddd~~<br>
<u>파란나비야, 저 멀리 날아가는구나</u><br>
`alert('즐기면서 하세요.')`<br>
>즐기면서 길게 하세요.

```
**강조**<br>
*강조*<br>
~~ddddd~~<br>
<u>파란나비야, 저 멀리 날아가는구나</u><br>
`alert('즐기면서 하세요.')`<br>
>즐기면서 길게 하세요.
```

  
  
  

## 그 외 요소들(abbr, acronym, sub, sup, etc)

---

일반적으로 <sup>두꺼비</sup>과의 개구리류를 통칭하기도 한다. <sub>몸길이 60~100 mm</sub> 이다. 등면은 보통 갈색이고 <cite>피부융기의 위끝 부분은 흑색이다</cite>. 몸통과 네다리의 등면에 불규칙한 흑갈색 무늬가 있다. 몸의 옆쪽에는 흑색 세로줄이 있다. 배면은 전체적으로 연한 황갈색이지만 황색을 띤 회백색의 개체도 있으며, 암갈색의 작은 무늬가 산재한다. 

머리는 몸에 비하여 크며 등면에 골질의 융기가 있다. <acronym title="안하무인 비만 선고ㅋㅋ">안비선(眼鼻線)</acronym>이 현저하고 주둥이의 등면과 뺨 부분이 약간 패어 들어갔다. 고막은 원형 또는 타원형이고 작다. 귀샘은 길고 뚜렷하다. 몸통 등면에는 많은 피부융기가 있고 네다리는 보통 짧다.

암컷은 수컷에 비하여 몸길이가 길고 다리는 짧으며 피부융기는 조밀하고 무늬가 좀 더 확장되어 있다. 주로 육상에서 생활하며 곤충류나 지렁이 등을 포식한다. 산란기에는 하천이나 늪 등에 모여들고 이 시기 이외에는 습한 곳에서 생활하는 것으로 알려진다. 한국, 일본, 중국, 몽골 등지에 분포한다. 
한국 민속에서는 집 지킴과 재복(업)의 상징으로 여겨지기도 한다.

<abbr title="인정?">ㅇㅈ?</abbr>

```
일반적으로 <sup>두꺼비</sup>과의 개구리류를 통칭하기도 한다. <sub>몸길이 60~100 mm</sub> 이다. 등면은 보통 갈색이고 <cite>피부융기의 위끝 부분은 흑색이다</cite>. 몸통과 네다리의 등면에 불규칙한 흑갈색 무늬가 있다. 몸의 옆쪽에는 흑색 세로줄이 있다. 배면은 전체적으로 연한 황갈색이지만 황색을 띤 회백색의 개체도 있으며, 암갈색의 작은 무늬가 산재한다. 

머리는 몸에 비하여 크며 등면에 골질의 융기가 있다. <acronym title="안하무인 비만 선고ㅋㅋ">안비선(眼鼻線)</acronym>이 현저하고 주둥이의 등면과 뺨 부분이 약간 패어 들어갔다. 고막은 원형 또는 타원형이고 작다. 귀샘은 길고 뚜렷하다. 몸통 등면에는 많은 피부융기가 있고 네다리는 보통 짧다.

암컷은 수컷에 비하여 몸길이가 길고 다리는 짧으며 피부융기는 조밀하고 무늬가 좀 더 확장되어 있다. 주로 육상에서 생활하며 곤충류나 지렁이 등을 포식한다. 산란기에는 하천이나 늪 등에 모여들고 이 시기 이외에는 습한 곳에서 생활하는 것으로 알려진다. 한국, 일본, 중국, 몽골 등지에 분포한다. 
한국 민속에서는 집 지킴과 재복(업)의 상징으로 여겨지기도 한다.

<abbr title="인정?">ㅇㅈ?</abbr>
```

  
    

## 링크 표현하는 법

---

[Google](https://www.google.com/)  
[naver](https://www.naver.com/)

```
[Google](https://www.google.com/)  
[naver](https://www.naver.com/)
[내가 지은 링크이름](링크주소)
```

  
  
  

## 이미지 표현하는 법

---

[![](http://ww1.sinaimg.cn/mw690/81b78497jw1emfgwkasznj21hc0u0qb7.jpg)](http://ww1.sinaimg.cn/mw690/81b78497jw1emfgwkasznj21hc0u0qb7.jpg)

[![Caption](http://ww3.sinaimg.cn/mw690/81b78497jw1emfgwjrh2pj21hc0u01g3.jpg)](http://ww3.sinaimg.cn/mw690/81b78497jw1emfgwjrh2pj21hc0u01g3.jpg)

[![](http://ww2.sinaimg.cn/mw690/81b78497jw1emfgwil5xkj21hc0u0tpm.jpg)](http://ww2.sinaimg.cn/mw690/81b78497jw1emfgwil5xkj21hc0u0tpm.jpg)

```
![](http://ww1.sinaimg.cn/mw690/81b78497jw1emfgwkasznj21hc0u0qb7.jpg)

![Caption](http://ww3.sinaimg.cn/mw690/81b78497jw1emfgwjrh2pj21hc0u01g3.jpg)

![](http://ww2.sinaimg.cn/mw690/81b78497jw1emfgwil5xkj21hc0u0tpm.jpg)

```

  
  
  

## 이미지에 링크걸기

---

[![](http://ww1.sinaimg.cn/mw690/81b78497jw1emfgwkasznj21hc0u0qb7.jpg)](https://www.naver.com/)

```
[![](https://is1-ssl.mzstatic.com/image/thumb/Purple118/v4/58/3a/42/583a42c5-881a-5c67-ecf2-c38177fd0468/AppIcon-1x_U007emarketing-85-220-0-8.png/246x0w.jpg)](https://www.naver.com/)

```

  
  
  

## 글 정렬하기

---

> 마크다운은 가운데 정렬만 지원한다.

<center>가운데</center>  
<div style="text-align: left"> 왼쪽 </div>
<div style="text-align: right"> 오른쪽 </div>

```
<center>가운데</center>  
<div style="text-align: left"> 왼쪽 </div>
<div style="text-align: right"> 오른쪽 </div>
```

  
  
  

## 인용문 표현하는 법

---

> d
> 
> > d
> > 
> > > ddd
> > > 
> > > > dddd
> > > > 
> > > > > ddddd

```
>d
>>d
>>>ddd
>>>>dddd
>>>>>ddddd
```