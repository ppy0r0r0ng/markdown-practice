# 제목(Header)

<!-- html의 h1 ~ h6태그로 변환되서 브라우저에서 동작함 -->
# 제목 1 
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6

<!-- # 다음에 띄어쓰기 해주는 걸 권장! 
마크다운 출력 환경에 따라서 띄어쓰기 안 해주면 제대로 제목으로 해석이 안 될 수도 있기 때문에 -->
# 제목1
#제목1

# 문장(Paragraph)
동해물과 백두산이 마르고 닳도록
하느님이 보우하사 우리나라 만세
<!-- 별 다른 기호를 사용하지 않고 문장을 넣으면 해당하는 문장이 화면에 출력됨. p태그로 완성됨! -->

# 줄바꿈(Line Breaks)
동해물과 백두산이 마르고 닳도록  
하느님이 보우하사 우리나라 만세  
무궁화 삼천리 화려 강산<br/>
대한 사람 대한으로 길이 보전하세    
<!-- 문장 뒤에서 두 번의 띄어쓰기를 하면 줄바꿈이 됨,
또는 <br/> 태그를 뒤에 붙여주면 됨 (마크다운을 출력하는 환경에 따라서 띄어쓰기 2번으로 안 될 경우 사용) -->
  
# 강조(Emphasis)

_이텔릭_
<!-- 원하는 문장의 앞 뒤로 언더바 -->

**두껍게**  
<!-- 원하는 문장의 앞 뒤로 ** -->

**_이텔릭 + 두껍게_**

~~취소선~~
<!-- 원하는 문장의 앞 뒤로 ~~ -->

<u>밑줄</u>
<!-- 마크 다운 문법에서 밑줄을 표시하는 기능은 제공되지 않음. 그냥 u태그 사이에 넣어주면 됨 -->

# 목록(List)

1. 순서가 필요한 목록
1. 순서가 필요한 목록
1. 순서가 필요한 목록
    1. 순서가 필요한 목록
    1. 순서가 필요한 목록
1. 순서가 필요한 목록
<!-- 들여쓰기 2번할 경우 서브로 들어감-->

- 순서가 필요하지 않은 목록
- 순서가 필요하지 않은 목록
- 순서가 필요하지 않은 목록
    - 순서가 필요하지 않은 목록
    - 순서가 필요하지 않은 목록
- 순서가 필요하지 않은 목록

# 링크(Links)

<!--HTML 태그-->
<a href="https://google.com">GOOGLE</a> 

<!--마크 다운-->
[GOOGLE](https://google.com)

<!--HTML 태그-->
<a href="https://naver.com" 
title="NAVER로 이동!">NAVER</a> 

<!--마크 다운-->
[NAVER](https://naver.com "NAVER로 이동!")

<a href="https://naver.com" 
title="NAVER로 이동!"
target="_blank">NAVER</a> 
<!-- 마크다운에서는 target 속성은 제공하고 있지 않음 -->

# 이미지(Images)

![HEROPY](https://heropy.blog/css/images/logo.png)
<!-- [] 사이에는 대체 텍스트가 들어감 -->
<!-- 링크와 이미지의 차이: 맨 앞에 !가 있느냐 없느냐 -->

[![HEROPY](https://heropy.blog/css/images/logo.png)](https://heropy.blog/)
<!-- []사이에 이미지 코드 전체를 넣으면 이미지 선택하게 되면 ()안에 있는 주소로 이동하게 됨
(이미지에 링크 걸기)-->

# 인용문(BlockQuote)

> 남의 말이나 글에서 직접 또는 간접으로 따온 문장.  
> (네이버 국어 사전)

> 인용문을 작성하세요!
>> 중첩된 인용문
>>> 중중첩된 인용문 1  
>>> 중중첩된 인용문 2  
>>> 중중첩된 인용문 3

# 인라인(inline) 코드 강조

CSS에서 `background` 혹은 
`background-image` 속성으로 요소에 배경 이미지를 삽입할 수 있습니다.
<!-- 강조할 곳 앞 뒤로 `백틱 기호 사용, 원하는 강조 부분 드래그 하여 백틱기호 한 번만 누르면 앞 뒤로 자동대로 붙여짐 -->

# 블록(block) 코드 강조

```html
<a href="https://google.com" target="_blank">GOOGLE</a> 
```

```css
.list > li {
  position: absolute;
  top: 40px;
}
```

```javascript
function func() {
  var a = 'AAA';
  return a;
}
```

```bash
$ git commit -m 'Study Markdown'
```

```plaintext
동해물과 백두산이 마르고 닳도록
하느님이 보우하사 우리나라 만세
```

# 표(Table)

position 속성

값 | 의미 | 기본값  
--|--|--
static | 기준 없음 | O
relative | 요소 자신 | X
absolute | 위치 상 부모 요소 | X
fixed | 뷰포트 | X        
<!-- --| 은 표의 머리 부분과 몸통 부분을 구분하는 용도임,
표 안에서 왼쪽정렬 되어 있음 -->    
<br/>     
position 속성

값 | 의미 | 기본값  
--|:--:|--:
static | 기준 없음 | O
relative | 요소 자신 | X
absolute | 위치 상 부모 요소 | X
fixed | 뷰포트 | X
<!-- 하이픈 앞 뒤로 : 붙여주면 가운데 정렬이 됨 -->
<!-- 하이픈 뒤에 : 하나만 붙여주면 오른쪽 정렬이 됨 -->
<br/>

# 원시 HTML(Raw HTML)
<!-- 마크다운은 브라우저에서 출력이 되어야 하기 때문에 표준의 HTML로 변환이 됨. 그런데 사용되는 플랫폼이나 환경에 따라서 다르게 변환될 수 있음 
=> 표준이 없기 때문에... 

아무튼, 마크다운은 변환 전에도 우리가 알고있는 HTML 문법을 그대로 사용할 수 있음-->

동해물과 <span style="text-decoration: underline">백두산</span>이 마르고 닳도록<br/>
하느님이 보우하사 우리나라 만세

<!-- * 원시 HTML: 마크다운 안에서 실제 HTML 문법을 사용하는 것을 말함 -->

<a href="https://google.com" 
title="NAVER로 이동!"
target="_blank">NAVER</a> 
<!-- target 사용 -->

<img width="70" src="https://heropy.blog/css/images/logo.png" alt="HEROPY">
<!-- 너비 지정 -->
