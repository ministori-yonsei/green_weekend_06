# HTML, CSS, JS 기초

## HTML

> HTML : Hyper Text Markup Language - 마크업(표시) 언어
> 
> 웹페이지의 구조를 표시
> 
> 웹페이지의 콘텐츠를 표시

### HTML Elements

> Element : 요소 - 의미적
> 
> Tag : 태그 - 기술적

> 문법(Syntax)
> 
> <>로 감싸줌
> 
> 소문자 사용
> 
> 시작태그와 종료태그 세트로 구성됨.
```
<tagname>contents</tagname>
```
> 
> 예외) 시작태그만 존재하는 경우 : 빈 요소(Empty Element)
> 
> 포함관계(Nested)
```
<body>
  <div>
    text
  </div>
</body>
```

### HTML Attribute

> HTML 속성
> HTML 요소의 부가 정보
> 속성이름 = "속성값"

```
<a href="http://www.naver.com">naver</a>
```
### HTML 페이지에서 표시하는 콘텐츠

- 텍스트 콘텐츠

- 멀티미디어 콘텐츠(임베디드embeded 콘텐츠)
  - 이미지
  - 비디오
  - 오디오

### 제목 태그

> heading -> h
> 
> h1 ~ h6
> 
> h1이 가장 큰 제목

### HTML 기본 구조

```
<!DOCTYPE html> - 1
<html> - 2
  <head> -3
    <meta charset="utf-8"> - 4
    <title>My test page</title> - 5
  </head>
  <body> - 6
    <p>This is my page</p>
  </body>
</html>
```

1. 웹 문서의 버전 : HTML5
2. html 문서의 가장 바깥쪽 요소
3. 웹 문서를 설명하는 정보가 담기는 영역 요소
4. 웹 문서의 정보 표시 요소
5. 웹 문서의 제목을 표시 요소
6. 웹 문서의 콘텐츠 요소들이 담기는 영역 요소

### 단락 태그

> p(Paragraph) : 단락을 표시
> 
> 단락과 단락사이를 구분하는 수평선
```
<hr> - Horizontal Rule
```
> 단락을 구분하지 않고 줄 바꿈
```
<br> - Break
```
### 목록 태그

> 순서없는 목록 ul(Unordered List)
> 순서있는 목록 ol(Ordered List)
> 목록 항목 li(List Item)

```
<ul>
  <li>HTML</li>
  <li>CSS</li>
</ul>

<ol>
  <li>HTML</li>
  <li>CSS</li>
</ol>
```
> 포함관계(nested)로 구성된 목록 - 코딩할때 밖에서 안쪽 방향 순서로
- HTML
  - HTML4
  - HTML5
- CSS
  - CSS2
  - CSS3
```
<ul>
  <li>
    HTML
    <ul>
      <li>HTML4</li>
      <li>HTML5</li>
    </ul>
  </li>
  <li>
    CSS
    <ul>
      <li>CSS2</li>
      <li>CSS3</li>
    </ul>
  </li>
</ul>
```

> 설명목록(Description List) - dl

```
<dl>
  <dt>HTML</dt> (dt : Desctpition Title)
  <dd>표준 마크업 언어</dd> (dd : Description Data)
</dl>
```

### HTML Hyper link

> 하이퍼링크 a(anchor)
> 
> attribute(속성) : href(Hypertext Reference) : 연결되는 웹 문서의 URL
```
<a href="http://www.naver.com">네이버로 이동</a>
```
> 북마크 기능
> 
> 외부 페이지 연결이 아닌 같은 페이지에서 특정위치로 이동할 수 있게 해주는 기능
> 
> 도착지점에 id attribute를 사용하여 이름을 지정
```
<a href="#t1"></a>
...
<h2 id="t1">제목</h2>
```

### Table Element

> 기본 사용 태그 : table, thead, tbody, tr, th, td
> 
> 열 제목 : thead(table head), th(table heading)
> 
> 표 내용 : tbody(table body), td(table data)
> 
> 행 : tr(table row)

https://www.tablesgenerator.com/html_tables

### Image element
> Tag : img
> 
> Attribute : src(image 위치, 파일명), alt(대체텍스트)

` : backtick
```
<img src="image.jpg" alt="대체텍스트">
```
### Video Element

> 비디오및 오디오 콘텐츠는 용량이 크기 때문에 서버에 저장을 해서 콘텐츠를 제공하면 많은 트래픽이 발생할수 있음
> 
> 트래픽 과부하를 해결하기 위해서 유튜브 서비스를 사용하기도 함
> 
> attribute
> 
> controls : 컨트롤 버튼 표시
> 
> autoplay : 자동재생(* muted와 같이 사용해야 함)
> 
> muted : 음소거
> 
> loop : 반복 재생

### Youtube

> 비디오 콘텐츠 제공시 서버의 트래픽 과부하를 해결할 수 있는 방법중의 하나
> 
> 매개변수
> 
> controls=1, 0
> 
> autoplay=1, 0 (mute와 같이 사용)
> 
> mute=1, 0
> 
> loop=1, 0(playlist와 같이 사용)

> 텍스트는 HTML 문서에 직접 입력되는 콘텐츠
> 이미지와 동영상, 오디오 콘텐츠는 외부에서 만들어지는 콘텐츠
> 이미지, 동영상, 오디오는 직접 입력하는 것이 아니고 외부 파일을 삽입 => 임베드(embed) 콘텐츠


### 웹사이트 템플릿 디자인

https://freebiesbug.com/psd-freebies/minimo-minimal-blog-template/

### Container Element(단순 영역 구분 요소)

> div(division)
> 
> span

### Block, Inline

> 모든 element는 각각의 고유 영역을 가지고 있음
> 
> block element, Inline Element 구분은 이들 영역의 화면 표시 방식에 따른 구분
> 
> block element는 줄바꿈 되어 표시 - block element 영역의 가로 너비가 부모요소에 100% 채워짐
> (** 포함하는 요소 : 부모요소, 포함되는 요소 : 자식요소)
> 
> block element에는 위,아래 여백을 적용할 수 있음
> 
> inline element는 같은 줄에 나란히 표시 - inline element 영역의 가로 너비가 콘텐츠 크기만큼만 정해짐
> 
> inline element는 위,아래 여백을 적용할 수 없음



