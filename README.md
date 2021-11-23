## 📍 엘리스 SW 엔지니어 트랙 

## 📍 O.T
1. 주 5일, 총 560시간 동안 온/오프라인 병행하여 진행
- Part 1: JS 기초(1~4주차)
- Part 2: `Typescript`, `Node.js`, `SQL(5~9주차)` + 웹 서비스 프로젝트1
- Part 3: `React` + 웹 서비스 프로젝트2

2. 열심히 했는지 안 했는지 플랫폼에서 추천 할 수 있는 기능이 있음. 열심히 한 만큼 회사에 추천 가능성 증가
3. 팀 프로젝트(GitLab): 기여도 확인, 커스터마이징 가능, 답을 밖에 공개하기 보다는 `GitLab`의 `private` 사용 
4. 수료는 전체 교육의 80% 이상 출석해야 수료
5. 온라인 학습일 (수, 금): 로그인 / 로그아웃 시간 데이터 확인(학습시간이 7시간이 넘어야 출석으로 인정된다. 일정 시간 이상 활동하지 않으면 학습시간 기록 종료)
6. 오프라인 교육시 선릉역, 삼성역 인근의 교육장을 이용
   
## 📍 10.26.화. 1일차(실시간 강의)
수업은 <a href='https://www.youtube.com/c/%EC%83%9D%ED%99%9C%EC%BD%94%EB%94%A91'>이고잉</a>튜터님께서 가르쳐주셨다. 내가 맨 처음 프론트엔드를 하겠다는 마음을 먹고 유튜브에서 찾아봤던 영상이 이고잉님 강의였는데, 다른 레이서들과 함께 온라인 수업을 실시간으로 가르쳐주시니까 놀라웠다.

### ❏ CSS 우선순위
1. `!important` 태그
2. `HTML` 태그 안에 직접 `style`을 지정한 태그( `inline style`은 별로 추천하지 않는다.) 
3. `#id` 
4. `.class`, `추상class`, `수도클래스(:first-child)`
5. `HTML` 태그 
6. 상위 객체에 상속된 속성

### ❏ 수업 내용
1. `CSS`는 `HTML` 이 등장한지 4년 이후에 나왔다.
2. `DOM`: `JS`를 이용하여 웹 브라우저를 제어하는 방법
3. 수업내용 이전에 배운 내용이 잇다면 처음부터 전체적인 구조를 생각하며 배운다. (제일 중요한 것은 `HTML`)
4. 지식인이 되기 보다는 실천적인 사람이 되자.
5. 중급자로 올라 갈 수록 해당 개념에 대한 세부적인 강의도 없어진다. 따라서 어떤 개념이 베이스가 되는지 알고 추론을 잘해야한다.
6. `tag`: 옷에 달려있는 태그가 옷을 설명하듯이 코드를 감싸는 태그는 코드를 설명하는 기능을 한다.
7. `git`: 내가 작성한 코드를 안전하게 마치 `dropbox` 같은 곳에 저장하는 저장소
8. `img`는 `width`만 사용하고, `height`만 사용하는 것을 권장한다. (`width`만 사용하면 `height`는 컴퓨터가 알맞은 높이를 자동으로 계산하여 나타내고, 반대로 `height`만 사용하면 `width`는 컴퓨터가 알맞은 너비를 자동으로 계산하여 나타낸다.)
9. 태그에 붙어있는 `src`, `alt`, `width`, `height` 등은 속성(attribute)를 나타낸다.
10. `hyper link`: 모든 형식의 자료를 클릭 한번으로 연결하고 가리킬 수 있는 참조 고리이다.
11. `server - client`: `client`에서 주소표시창에 `Domain name`을 입력하고 `Enter`를 누르면 `Domain name`과 연결되어있는 `IP address`를 찾고 해당 주소를 통해 `server`에 접근한다. 이때, `server`는 `client`에게 `HTML`파일을 보여주는데 기본적으로 `index.html`로 설정되어있다.
12. `CSS selector`: CSS 규칙을 적용할 요소를 정의한다.
13. 하단과 같이 시각적인 도움만 주는 `CSS`코드는 권장되지 않는다. `HTML2`부터는 `HTML`태그로 문서의 구조와 의미를 표현하고, `CSS`태그로 문서의 스타일만 표현하면서 문서의 구조와 스타일을 분리하는 쪽으로 발전되었다. 즉, 시각적인 정보만 주는 태그는 사용하지 않는다. (`HTML5`부터 더 이상 지원하지 않는다.)

```css
<font color="red">
    <h1>html</h1>
</font>
<font color="orange">
    <h1>css</h1>
</font>
<font color="blue">
    <h1>js</h1>
</font>
```

14. `HTML tag`는 각자 자기만의 `style`이 존재한다. (예 `h1`: `display:block`, `font-size:2em`, `font-weight:bold` 등)
15. `padding`: `content`와 `테두리(border)` 사이의 간격
16. `margin`: `테두리(border)`와 `테두리(border)` 사이의 간격 (상하 관계의 `margin`은 <a href='https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing'>margin-collapsing</a>으로 인해 제일 큰 여백의 크기를 가진 단일 여백으로 상쇄된다.)
17. `block`: 화면 전체를 사용한다. 가로 길이를 조정하고 싶으면 `width`를 사용하기
18. `inline`: 자기 `content` 만큼의 크기만을 갖는다.

## 📍 10.27.수. 2일차(온라인 강의)
오늘은 실시간 강의 대신 온라인 강의를 듣는 날이다. 기존에 `HTML/CSS`를 어느정도 알고있다고 판단하여 금방 끝날 줄 알았는데 생각보다 오래걸렸다. 매 강의마다 `이론 + 퀴즈 + 실습` 구성으로 이루어져 있는데, 실습에서 코드를 제출해야 점수가 기록되므로 알고 있는 내용이라고 그냥 건너뛸 수 없었다. 강의를 다 들은 다음 배운 내용을 점검하는 작은 테스트까지 봐야 훈련이 끝난다. 첫 날이라 8시간이 걸렸고, 온라인 강의가 있는 날은 10시 이전부터 시작해야겠다는 생각이 들었다.

### ❏ 수업 내용
1. `프로그래밍`: 컴퓨터와 소통하는 방법, 웹 개발을 하기위한 언어로 브라우저와 소통하는 매개체
2. `HTML`: 정보 또는 설계도, `CSS`: 디자인 또는 스타일링, `JS`: 기능과 효과
3. `웹 표준`: 웹 사이트를 작성할 때 따라야 하는 공식 표준이나 기술 규격
4. `웹 접근성`: 장애(시각장애, 청각장애 등)의 여부와 상관없이 모두가 웹사이트를 이용할 수 있게 하는 방식
5. `크로스 브라우징`: 모든 브라우저 또는 기기에서 사이트가 제대로 작동하도록 하는 기법(기술 면접에서 질문받은 개념이다.)
6. `<!DOCTYPE html>`: 페이지의 `HTML`버전을 웹 브라우저에게 알려주는 역할을 한다. `HTML5`로 문서를 작성하겠다는 의미 (닫힌 태그가 없다.)
7. `<meta charset="UTF-8">`: charset은 `character setting`의 약어로, 모든 문자 코드를 웹 브라우저에서 `UTF-8`로 보여주겠다는 의미다. (한글이 들어가면 빼먹지 말자.)
8. `<title></title>`:웹 사이트 탭에 나타내는 제목을 적는 태그
9. `contents`: 열린태그와 닫힌태그 사이에 있는 내용들 (`<body>`태그안의 모든 코드는 `body`의 `contents`가 된다.)
10. `<head></head>`: 웹 사이트의 간단한 요약 정보를 담는 영역, 웹 사이트에서 노출되지 않는 정보
11. `<body></body>`: 웹 사이트에서 눈에 보이는 정보를 담는 영역, 이미지나 텍스트처럼 출력되는 정보
12. `<img src="logo.png" alt="회사로고">`: 이미지는 닫힌 태그가 없다.(react에는 닫힌 태그가 있다.) `src`: 삽입 할 이미지의 파일 경로, `alt`: 웹 사이트가 이미지를 출력하지 못했을 경우 텍스트 정보로 대체, `width`만 사용하면 원래 갖고있던 이미지의 비율에 맞춰 `height`를 보여준다. 
13. `<h tag>`: 웹 사이트의 타이틀 표현, `h1` 태그는 가장 중요한 정보를 담으므로, 하나의 `html`문서에서 한번만 사용된다.
14. `p`: `paragraph`의 약자로 본문 내용을 표현한다. 웹 사이트의 중요 정보를 담는 태그
15. `ul`: `unOrdered list`의 약자로, 순서가 없는 리스트 생성, 주로 메뉴버튼을 만들 때 사용한다. 자식태그로는 `li`가 있다. (`ol`은 순서가 있는 리스트 생성)
16. `a`: `anchor`의 약자로 다른 웹 페이지로 이동하거나, 문서내에서 이동하는 경우에 사용한다. `<a><img></a>` 처럼 이미지를 클릭하면 다른 링크로 이동 할 수 있다.

```js
// a태그에 사용 가능한 속성(attribute)
1. href: 연결 할 주소를 설정
2. target: 링크를 클릭 할 때 창을 어떻게 열 것인가?
  * `_self`: 링크를 클릭한 해당 창에서 연다.
  * `_blank`: 링크를 새 창으로 연다.
  * `_parent`: 부모 창에서 연다.
  * `_top`: 전체 브라우저 창에서 가장 상위의 창에서 연다.
3. title: 해당 링크에 마우스 커서를 올릴 때 도움말 설명을 설정한다.
```

```html
<ul>
    <li><a href="">홈</a></li>
    <li><a href="">게시판</a></li>
    <li><a href="">마이페이지</a></li>
</ul>
```

17. `<header>`: 웹 사이트의 머리 글을 담는 공간(`nav`가 담겨있는 경우가 많음)
18. `<nav>`: 메뉴 버튼을 담는 공간, 네비게이션 (주로, `ul`, `li`, `a`와 함께 사용한다.)

```html
<header>  <!-- 상단 영역 -->
	<img src="elice_logo.png" alt="엘리스 로고">
	<nav>  <!-- 메뉴 버튼 영역 -->
		<ul>
			<li><a href="">홈</a></li>
			<li><a href="">전체 목록</a></li>
		</ul>
	</nav>
</header>
```

19. `<main role="main">`: 웹 사이트의 주요 내용을 담는 공간 (IE에서는 `main` 태그를 지원하지 않으므로 `role="main"` 속성을 필수로 입력한다.)
20. `<article />`: 영역을 대표하는 타이틀 정보가 존재하기 때문에 태그 내에 구역을 대표하는 타이틀인 `<h>`태그가 존재해야 한다.

```html
<main role="main">  <!-- 본문 영역 -->
	<article>  <!-- 정보 영역 -->
	</article>
</main>
```

21. `<footer>`: 웹 사이트의 가장 하단에 들어가는 정보를 표기할 때 사용
22. `<div>`: 임의의 공간을 만들 때 사용

```html
<footer>  <!-- 하단 영역 -->
	<div>  <!-- 회사 정보 -->
		<p>주소: 경기도 화성시 동탄공원로</p>
		<p>이메일: ywtechit@gmail.com</p>
	</div>
	<div>  <!-- 전자상거래소비자보호법 필수 정보 -->
		<p>사업자등록번호: 000-00-00000 | 대표: 안영우</p>
		<p>통신판매업신고번호: 제0000-토끼굴-0000호</p>
	</div>
</footer>
```

23. `display: block`과 `display: inline`의 큰 차이점: 줄 바꿈 현상, `width`, `height`, 상 하 배치
24. `display: block`: `y`축 정렬 형태로 출력(줄 바꿈 현상이 보인다.) `width`, `height`로 공간을 만들고 상하 배치 작업이 가능하다. (`h`, `p`)
25. `display: inline`: `x`축 정렬 형태로 출력(한 줄에 출력) `width`, `height`로 공간을 만들 수 없고 상하 배치 작업이 불가능하다. (`a`, `span`)
26. `CSS` 적용 방법 3가지: 첫번째로 `inline style sheet`로 태그 안에 직접 원하는 스타일을 적용한다. (`<h1 style="color: red;">)coding 101 </h1>`) 두번째는 `internal style sheet`로 `<style>` 태그 안에 넣어서 적용한다. (`<style> h1{ background-color: yellow;}</style>`) 마지막으로 `external style sheet`로 외부에 `css`파일을 저장해두고 `<link>` 태그로 불러오기 (`<head> <link rel="stylesheet" (연결 할 문서의 정보의 성격 지정) href="style.css(경로입력)"></head>`, `link` 태그는 닫힌 태그가 없다.  ) 마지막 CSS 방법(`external`)의 장점은 `html`, `css` 각각의 문서 안에서 따로 관리하여 상대적으로 가독성이 높고 유지보수가 쉽다. (실무에서 많이 사용)
27. `CSS` 선택자: 첫번째는 타입(`type`): `h2{color: red;}` 두번째는 클래스(`class`): `.tech{color: red;}` 마지막은 식별자(`ID`): `#tech{color: red;}`

```css
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>CSS 선택자</title>
  <style>
    h2 {
    	color: red;
    }
  
    .coding{
    	color: green;
    }
  
  	#coding{
  		color: yellow;
  	}
  </style>
</head>

<body>
	<h2>Type Hello World</h2>
	<h2 class="coding">Class Hello World</h2>
	<h2 id="coding">Id Hello World</h2>
</body>
</html>
```

28. `CSS cascading`: `CSS`의 우선순위를 결정하는 세 가지 요소. 첫 번째로 순서: 동일한 태그를 기준으로 나중에 적용한 속성값의 우선순위가 높다. 두번째는 디테일: 더 구체적로 작성된 선택자의 우선순위가 높다. 마지막으로 선택자: `inline style > id > class > type` 순으로 적용된다.

```css
/* 동일한 태그를 기준으로 나중에 적용한 속성 */
p { color: red; }
p { color: blue; }  // ✅

/* 더 구체적으로 작성된 선택자의 우선순위가 높다. */
header p { color: red;}  // ✅ detail
p {color: blue; }

/* `inline style > id > class > type` 순으로 우선순위가 높다. */
<h3 style = "color: pink" id="color" class="color">color</h3>  // 1
#color { color: blue; }  // 2
.color { color: red; }  // 3
h3 { color: green; }  // 4
```

### ❏ CSS의 주요 속성

1. `width` : 선택한 요소의 넓이를 설정 (고정값 (px), 가변값(%))
2. `height`: 선택한 요소의 높이를 설정
3. `font-family`: 브라우저마다 지원하는 폰트가 다름. 입력한 순서대로 우선순위 적용. `sans-serif` 는 마지막에 작성하는 디폴트 값.
4. `font-weight`: 100~900 사이의 숫자를 입력 할 수 있음
5. `border-style` : 실선 (solid) 점선 (dotted)
6. `background-repeat` : 이미지의 반복효과 설정, repeat-x, x축으로 반복, repeat-y, y축으로 반복, no-repeat: 반복하지 않음
7. `background-position`: 특정 공간 안에서의 이미지 위치

```css
.paragraph {
	background-color: yellow;
	background-image: url();
	backgorund-repeat: no-repeat;
	background-position: left;
	background: yello url() no-repeat left;  // 한번에 입력
}
```

### ❏ 웹 사이트 레이아웃에 영향을 미치는 요소

1️⃣ 박스모델: 공간 크기가 어떤 구조로 구성되어 있는지 확인하는 모델(`margin`, `border`, `padding`, `content`) 

1. `top`, `right`, `bottom,left` 순서로 입력가능
2. `margin` : `border`를 기준으로 바깥에 있는 요소
3. `padding`: `border` 와 `content` 사이의 간격

2️⃣  Block요소와 Inline 요소: `block`요소는 `y` 축 정렬(`header`, `p` , `width`, `height`, `margin`, `padding`  요소 사용가능), `inline` 요소는 `x` 축 정렬 (`a`, `span`), `margin-top`, `margin-bottom` 등 상하 배치 작업 속성은 사용 불가, 줄바꿈 없음

3️⃣  마진 병합 현상

1. 형제지간의 마진 병합: 큰 값을 우선순위로 `space` 를 만든다. 하단의 코드에서는 `250px` 이 아니라 `150px` 로 설정된다.

```html
<div class="box1">Hello World</div>
<div class="box2">Hello World</div>

.box1{ margin-bottom: 150px }
.box2{ margin-top: 100px } 
```

기존계산으로는 `margin` 이 `250px`이 되어야 하지만 마진의 교집합이 있을때는 더 높은 값에 우선순위가 주어지므로 `150px` 만큼만 차이가 난다.(마진 병합 현상)

2. 부모 자식간의 마진 병합: 부모도 함께 `space` 적용이 된다. 평소처럼 생각하면 자식 `div` 에만 `margin` 이 되어야하는데, 부모도 함께 `space` 적용이 된다.

```html
<main role="main">
	<article>
	</article>
</main>

.article {
	width: 200px;
	height: 200px;
	margin-top: 100px;
}
```

![](https://images.velog.io/images/abcd8637/post/f3f010ae-1148-4137-ba50-c6105892ab0b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-27%2020.24.52.png)

tip: 부모는 그대로인데 자식 `div`만 내리려면 자식 `div`에 `position: absolute`를 넣어준다.

![](https://images.velog.io/images/abcd8637/post/43cdd193-481e-427b-8ae5-19d937d48027/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-27%2020.26.05.png)

4️⃣  레이아웃에 영향을 미치는 속성

1. `display`: 원래 `block` 과 `inline` 이 갖고있는 성격을 바꿀 때 사용. `inline-block` 을 사용하면 두 요소의 성격을 모두 가짐 `inline-block`: `x` 축 정렬이면서 공간의 크기를 만들고 상하 배치 작업까지 진행하고 싶을 때 사용

2. `float`: 어떤 `object` 를 왼쪽 / 오른쪽에서부터 정렬시키고자 할 때 사용. 선택자를 띄워 새로운 레이어 층을 만드는 것, 레이어가 겹쳐지지 않는 상태로 왼쪽에서부터 정렬시키고 싶은 경우 `float:left` 를 연속적으로 입력, `clear` : `float` 에 대한 속성을 제어하고자 할 때 (특정 지점에서 `float` 의 기능을 `both` 로 꺼주고 컨텐츠를 배치하자. `clear` 는 마지막 `float` 를 사용한 태그 다음 태그에 넣어주자.)

3. 브라우저와 공간 사이의 공백 제거하기: 기본적으로 `html` 태그에는 기본 공간이 있는데 이를 없애준다.

```css
<style>
	html, body {
		margin: 0;
		padding: 0;
	}

  /* `*`은 모든 `html` 태그를 선택한다는 의미 */
	* {
		margin: 0;
		padding: 0;
}
</style>
```

4. `float` 사용 시 정렬 기준 점은 `div` 를 감싸고있는 부모의 크기를 기준으로 `float` 가 적용 된다. `float` 이 적용되는 부모의 길이가 더 커야 찌그러지지 않는다.

5. `float` 이 적용 된 지점 밑에 다른 `div` 가 들어올 수 있다.

```css
<style>
	.left{
		float: left;
	}

	.right{
		float: right;
	}
</style>

<div style = "width: 800px">
	<div class="left"></div>
	<div class="right"></div>
</div>
```

![](https://images.velog.io/images/abcd8637/post/eaaf1b5f-1d26-402a-89e5-896b92f2ddb4/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-27%2020.27.49.png)

6. `float` 을 마지막으로 사용한 태그 다음 태그에 `clear` 속성을 사용한다. 만약, `float: left` 만 되어있다면 `clear: left` ,   `float: right` 만 되어있다면 `clear: right` 양쪽은 `clear: both` 를 사용하면 된다. 보통의 경우에는 `clear: both` 를 많이 사용한다.

7. 기본적으로 `html`, `body` 에 `margin`, `padding` 이 존재하므로 이를 없애주자. `*{margin:0; padding:0;}`

> reference
1. a태그: <a href='https://developer.mozilla.org/ko/docs/Web/HTML/Element/a'>MDN</a>

---
## 📍 10.28.목. 3일차(실시간 강의)

### ❏ CSS Transition
1. `transform: rotate(45deg)`: 도형을 45도 만큼 회전(`+`는 시계방향, `-`는 반시계 방향)
2. `transform: scale(a, b)`: 가로폭 `a`배, 세로폭 `b`배 만큼 확대 (`Equal to scaleX(a) scaleY(3)`)
3. `transform: translate(100px, 200px)`: `x`축으로 `100px`, `y`축으로 `200px` 만큼 이동시킨다. (`x`는 `row`, `y`는 `column`)
4. `transform: skew(10deg, 20deg)`: `x`축으로 10도, `y`축으로 20도만큼 비튼다.
5. `margin: 200px 0 0 200px`: 한 줄로 나타내기보다는 가독성을 위해 분리해서 작성하는 것을 권장한다. 예를 들면, `margin-top: 200px`, `margin-left: 200px` 이런식으로..
6. `transform(변형시키다)`: 하단의 코드처럼 `transform`을 여러번 사용하면 제일 마지막에 작성한 `transform` 속성만 적용된다. 여러개의 `transform`을 적용하고 싶으면 한 줄로 작성하자.
   
```css
/* `transform: skew(10deg, 20deg)` 코드만 적용된다. */
<style>
   .transform {
	     width: 100px;
	     height: 100px;
	     background-color: red;
		   margin: 200px 0 0 200px;
		   transform: rotate(45deg);
		   transform: scale(2, 3);
		   transform: translate(100px, 200px);
		   transform: skew(10deg, 20deg);
   }
</style>

/* `scale`, `rotate`, `translate`, `skew` 속성이 모두 적용된다.*/
<style>
	.transform {
			transform: scale(2,3) rotate(45deg) translate(100px,200px) skew(10deg, 20deg);
	}
</style>
```

7. `transition(전환)`: `property, duration, timing-function, delay` 순으로 적용한다. 나머지 속성값의 순서는 상관 없으나, 항상 `duration` 이 먼저, `delay` 가 나중에 작성되어야 한다. `transition:hover` 를 띄어쓰기 없이 작성한다.
8. `transition`을 작성할 때 결과물을 먼저 만들어 놓고 나서 생각하면 편하다.
9. `transition-property` 효과를 적용하고 싶은 속성을 작성한다. `a`, `b`의 속성을 한번에 적용하려면 `all` 혹은 `a b`(`,` 없이 띄어쓰기로 작성한다.) `transition`의 기본값은 `all 0 ease 0`이다.
10. 만약에, 너비를 바꾸는 과정을 보고 싶어서 다음과 같이 `property`를 `width`로 작성했는데 `hover`에 `height`를 작성하면 `transition` 은 적용되지 않고 `hover 300px`만 된다. (과정은 생략되고 결과물만 나온다.)

```css
<style>
  .transition { 
        width: 100px;
        height: 100px;
        background-color: red;
				transition: width 2s linear 0s;
  }
	
	.transition:hover {
			height: 300px;
	}
</style>
```

```css
👉🏽 transition-timing-function

1. ease - 느린 시작으로 전환 효과를 지정한 다음 빠르게 지정한 다음 천천히 종료합니다(기본값).
2. linear - 처음부터 끝까지 동일한 속도로 전환 효과를 지정합니다.
3. ease-in - 느린 시작으로 전환 효과를 지정합니다.
4. ease-out - 느린 끝으로 전환 효과를 지정합니다.
5.ease-in-out - 느린 시작과 끝으로 전환 효과를 지정합니다.
6. cubic-bezier(n,n,n,n) - 3차 베지어 함수에서 고유한 값을 정의할 수 있습니다.
```

11. `animation`: 다수의 스타일을 전환하는 애니메이션 (`animation-name, animation-duration, animation-timing-function, animation-delay, animation-iteration-count, animation-direction, animation-fill-mode, animation-play-state`) 적용 코드는 다음과 같다. 한 줄로 나타낼 수도 있지만 가독성을 위해 한 줄로 끊어서 작성했다. `keyframes`에 `from-to`를 `0%-100%`로 작성해도 된다.

```css
<style>
    .animation {
        width: 300px;
        height: 300px;
        background-color: yellow;
		
				animation-name: changeWidth;
				animation-duration: 3s;
				animation-timing-function: linear;
				animation-delay: 1s;
				animation-iteration-count: 6;
				animation-direction: alternate;
    }
	
		@keyframes changeWidth {
			from {
				width: 300px;
			}
			to {
				width: 600px;
			}
		}
</style>
```

12. `animation`과 `transition`의 주요차이는 사용자의 액션없이 자동으로 실행하는 것이 `animation`이고 사용자의 액션 (hover, click...)을 통해 보여지는 효과가 `transition`이다. 
13. 반응형 조건(`media query`)을 작성할 때는 `<meta name="viewport" content="width=device-width, initial-scale=1.0">`를 꼭 붙여주자.

![](https://images.velog.io/images/abcd8637/post/474902cd-a9d7-43c1-ab56-f34ca407ecff/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-28%2021.54.03.png)

14. 반응형 속성은 동일한 속성 이외에 미디어 쿼리에서 작성하지 않은 값도 상속한다. 만약, 상속하기 원치 않으면 `none`을 써주자

```css
<style>
.alice{
	border: 1px solid blue;
}

@media (min-width: 420px) and (max-width: 768){
	.alice {
		border: none;
	}
}

</style>
```

---
## 📍 10.29.금. 4일차(온라인 강의)
나름 프로젝트(<a href='https://github.com/YWTechIT/project-military-test'>병과테스트</a>, <a href='https://github.com/YWTechIT/starbucks-recipe-project'>스타벅스 히든 레시피</a>)를 진행하면서 `HTML`에 대해 많이 알고있다고 생각했는데, 4일밖에 안됐는데도 모르는 내용들이 많았고 더불어 정리 할 내용도 많았다. 현업에 뛰어들기 전에 하나라도 더 볼 수 있다는 점을 감사하게 생각하며 오늘 배운내용을 정리해본다.

### ❏ 2차원과 3차원의 속성을 결정짓는 요소인 `position` 속성 배우기
1. `position`: 내가 만든 속성을 2차원 혹은 3차원으로 바꿀 수 있는 기능 

![](https://images.velog.io/images/abcd8637/post/75fdba25-b9ea-46c6-a16c-2d675b386113/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-29%2019.56.02.png)

2. 2차원과 3차원의 속성을 결정짓는 3가지 조건

```html
1. 부모 자식 지간에 발생하는 마진 병합 현상(margin-collapse)이 일어나면 2차원 속성이다.
2. `top`, `left`, `right`, `bottom`을 설정 할 수 있는 속성은 3차원이다.
3. 부모가 높이 값을 갖고 있지 않을 때 자식의 높이 값이 부모의 높이 값에 영향을 준다면 2차원 속성이고, 영향을 주지 않는 다면 3차원 속성이다.
```

3. `position:static`: 2차원 속성, 마진 병합현상(margin-collapse)이 일어난다. `top`, `left`, `right`, `bottom` 속성을 사용 할 수 없다. 부모가 높이값을 갖고 있지 않을 때 자식의 높이 값이 부모의 높이값에 영향을 준다. 모든 `html`의 기본 `position` 값은 `static`이다. (`position`을 명시하지 않아도 적용된다.) 하단의 우측사진은 부모 - 자식간의 마진 병합현상으로 인해 부모까지 같이 `margin-top`이 적용된 모습이다.

![](https://images.velog.io/images/abcd8637/post/e491f6a4-a84c-476a-b3d7-7dfcef711f70/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-29%2020.15.30.png)

4. `position: fixed`: 3차원, 마진 병합 현상이 일어나지 않는다. `top`, `left`, `right`, `bottom` 속성을 사용 할 수 있다. 이때 기준점은 브라우저의 좌측 상단이다. 부모가 높이 값을 갖고 있지 않을 때 자식의 높이 값이 부모의 높이 값에 영향을 줄 수 없다. 보통 `fixed`는 화면에 고정시키는 역할로 쇼핑몰에 항상 따라오는 배너를 구현할 때 사용된다. 

![](https://images.velog.io/images/abcd8637/post/6d7c47dc-8255-40f6-a084-244b848fa9e4/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-29%2020.18.00.png)

5. `position: relative`: 2차원과 3차원이 혼합되어있다. 마진 병합 현상이 일어난다. `top`, `left`, `right`, `bottom` 속성을 사용 할 수 있다. 이때 기준점은 자기가 존재하는 위치다. 부모가 높이 값을 갖고 있지 않을 때 자식의 높이 값이 부모의 높이값에 영향을 줄 수 있다.

![](https://images.velog.io/images/abcd8637/post/e7df7821-c21a-4bcb-9c2a-db1a74626041/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-29%2020.19.41.png)

6. `position: absolute`: 3차원 속성, 마진 병합 현상이 일어나지 않는다. `top`, `left`, `right`, `bottom` 속성을 사용 할 수 있다. 이때 기준점은 부모 `position`에 따라 다른데, 부모가 `position: static`이면 브라우저 좌측 상단을 기준으로 적용되고, 부모가 `position: relative`면 현재 나의 위치를 기준으로 적용된다. 부모가 높이 값을 갖고 있지 않을 때 자식의 높이 값이 부모의 높이값에 영향을 줄 수 없다. 

![](https://images.velog.io/images/abcd8637/post/b8d3ebed-4ed9-4774-8a07-c056d2d44306/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-29%2020.21.17.png)

### ❏ 시작 페이지 제작하기
1. 모바일을 고려 할 때 `<head>` 태그에 `<meta name="viewport" content="width=device-width, initial-scale=1.0">` 태그를 꼭 추가하자. `viewport`는 내가 보고 있는 기기의 화면을 뜻하고, `content`는 `viewport`의 너비를 디바이스의 너비로 설정하고 실제 제작되는 화면의 비율을 `1.0`배로 설정하는 코드이다. 하단의 사진은 `<meta>`태그를 적용했을 때와 `<meta>`태그를 적용하지 않았을 때의 차이를 보여주는 사진이다.

![](https://images.velog.io/images/abcd8637/post/00ecf36a-391e-4f63-a6f2-447d4261dc00/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-29%2019.54.02.png)

2. `z-index` 속성: 레이어층의 변동을 주고 싶을 때, `z`축을 사용하기 위한 속성인 3차원 `position: absolute, fixed, relative`일 경우에만 사용가능하다. 3차원 `position` 중 나중에 작성된 `position` 값이 쓰인 태그가 `z`축의 우선이 더 높다.

3. `background`: 배경 이미지의 크기를 결정짓는 `css` 속성 주로 `background-size: contain`, `background-size:: cover` 속성을 자주 사용한다. `contain`은 배경을 모두 덮어 씌운다. 이미지 전체가 나타나지만 여백이 생길 수 있다. `cover`은 배경을 사용하는 공간을 꽉 채운다. 배경 이미지의 가로 세로 비율을 유지한다. 이미지의 일부가 잘려서 출력된다.

```html
`background-attachment`: 배경이미지의 스크롤 여부를 결정짓는 요소

1. `background-attachment: scroll`: 스크롤하면 배경이미지가 고정되지 않음
2. `background-attachment: fixed`: 스크롤하면 배경이미지가 고정되면서 같이 내려감
```

4. `y`축 정렬 방법: 다음의 공식을 이용한다.

```css
top: 50%;  /* position: fixed, relative, absolute */
transform: translateY(-50%);  /* Y축으로 -50%만큼 이동한다. 자신의 크기를 기준으로 좌표가 형성된다. */
```
  
5. `box-sizing: border-box`: `box-model` 중 `padding`을 사용하면 공간의 크기가 바뀌지 않게 안전장치를 걸어준다. 공간에 대한 크기는 그대로인 상태에서 `padding` 값만 적용된다.

### ❏ 메인 페이지 살펴보기
1. `box-shadow`: 공간의 그림자 효과를 만들 때 사용하는 `css` 속성

```css
.box_shadow {
	width: 300px;
	height: 300px;
	box-shadow: 10px 10px 10px 10px red;  /* 수평방향(x), 수직방향(y), 흐림의 반경(숫자가 클 수록 그림자의 끝이 흐려지고 0이 될수록 선명하다), 그림자가 확산되는 거리, 그림자의 색상 */
}
```

![](https://images.velog.io/images/abcd8637/post/c46dd826-7c3a-4cbb-a88c-077d1f81fcd9/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-29%2020.26.07.png)

2. `border-radius`: 테두리의 각도를 조절

```css
.box_shadow {		
	width: 300px;
	height: 300px;
	border: solid 10px red;
	border-radius: 30px;
}
```

### ❏ `form` 태그 알아보기
1. `form`: 사용자가 특정 정보를 가입할 수 있도록 하는 태그

```html
<!-- form 태그 예시 -->
<form id="question_form">
	<div class="form-group">
		<label for="topic">제목</label>
		<input type="text" id="topic" name="topic">
	</div>

	<div class="form-group">
		<button type="submit">문의하기</button>
	</div>
</form>
```

2. `input` 태그는 주로 `label` 태그와 같이 사용한다. `label for=""` 값과 `input id="" name=""` 값을 동일하게 맞춰주자. 이렇게 설정하면 `label`을 클릭 할 때 `input`태그에 자동으로 `focus`가 맞춰진다. `input type`에는 `text`, `email`, `tel` 등을 넣을 수 있다. `label for=""`와 `input name=""`을 맞춰주는 이유는 서버에 데이터를 전송할 때 필요하다.

```html
<form id="question_form">
	 <label for="title">제목</label>
	 <input type="text" id="title" name="title">
		  
	 <label for="email">이메일 주소</label>
	 <input type="email" id="email" name="email">
		  
	 <label for="password">비밀번호</label>
	 <input type="password" id="password" name="password">           
</form>
```

3. `label`태그 안에 `input` 태그를 넣어줘도 된다.
4. `input type="radio"`: `radio` 타입은 중복체크를 하지 않기 위한 타입이다. 이때, `input name=""`은 `category` 값을 동일하게 넣어주자.
5. `input type="checkbox"`: `checkbox` 타입은 중복체크가 가능하다. 대신 `input name=""` 값을 각자 다르게 설정하자.
6. 회원가입을 할 때 사용자가 특정 정보를 기입하고 이를 서버에 전달하는 버튼을 포함한 전체 영역은 `<form>`태그로 작성한다.

---
## 📍 10.30.토. 5일차(온라인 강의)
오늘은 `Git` 사용법에 대해서 배웠다. 평소에 `CLI` 환경 대신 `Github-desktop`을 사용했는데, `CLI` 명령어를 하나부터 열까지 배울 수 있어서 좋았다. 기록해놨다가 나중에 현업에서 써먹었으면 좋겠다.

### ❏ Git의 특징
1. `master`는 독립성을 유지한 채 진행하고 나중에 `master`에서 주로 배포하게 끔 설정한다.
2. 다른작업을 독립적으로 진행하고 원하는 시점에 `branch`끼리 병합 할 수 있다.
3. 가볍고 빠르다. (서버와의 통신 없이 로컬에서 진행, 원격저장소 사용 제외)
4. 네트워크: `SVN(SubVersion)`은 항상 네트워크가 필요한 반면, `Git`은 다른사람과 코드를 공유 할 때만 네트워크가 필요하다.
5. 분산작업의 효율성: 개발자들은 개발만하고 통합 관리자는 개발된 코드를 병합하는데 집중한다.
6. 데이터 보장: 모든 파일은 `checkSum` 과정을 거친다. (16진수 문자열로 구성, `commit ID` 라고도 불린다.) `commit ID` 가 동일하다는 것은 파일 구성이 완벽히 동일하다. 누가 어떤 파일을 작업했는지 기록 또는 `hash` 값으로 알 수 있다.
7. 준비 영역(Staging area): 수정한 내용을 실제 `repository`에 반영하기 전 검토하는 단계
8. 오픈 소스(Open source): 소스코드를 공개한 상태에서 인터넷에서 누구나 프로젝트 발전에 기여 할 수 있다.
9. `Git` 호스팅 서비스: `Github`, `Bitbucket`, `Gitlab`
10. `Git`에서 관리하는 세 영역: `작업 영역(Working Directory)`, `준비 영역(Staging Area)`, `저장소(Repository)`

![](https://images.velog.io/images/abcd8637/post/4416ce2f-abf6-4b5b-8c32-57ff17bb4742/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-30%2017.32.24.png)

### ❏ Git 주요 명령어
1. `git add`: 파일을 준비영역(staging area)로 보내야 한다. 이때 `git add` 명령어를 이용하자. 파일의 현재 상태를 확인하려면 `git status` 명령어를 이용하자.
2. `git commit`: `comment.js` 파일을 `staging` 으로 이동하였으므로 무엇을 수정하고 추가했는지 메시지를 남겨 저장소에 저장하는 작업을 진행한다. 이때 `commit message`도 추가하고 싶다면 다음의 명령어를 사용하자. `git commit -m "message"`
3. `git commit --amend`: 앞서 커밋한 메시지에 오타가 있거나 누락된 파일이 있는 경우 저장소 반영 내용 변경
4. `git log --pretty=oneline` : 각 `commit` 을 한 줄로 출력
5. `git log --graph`: `commit` 간의 관계를 아스키그래프로 출력한다. (보통 `branch` 과정에서 많이 사용한다.)
6. `git log -S function_name`: `-S` 코드에서 추가되거나 제거된 내용 중 특정 텍스트(예시는 `function_name` ) 가 포함되어 있는지 검사한다. 
7. `git status` : `git` 명령소의 현재 상태를 알 수 있다.
8. `untracked` : 코드의 변경 내용을 추적하는 단계가 아니다. `staging area`로 보내야 코드의 수정내용을 추적 가능함.
9. `git reset filename` : untracked 상태로 변경

```shell
# untracked인 파일 crawling.py와 README.txt 파일 중 crawling.py 파일 만 commit 하고 싶을 때
$ git add crawling.py
$ git commit -m "commit crawling.py"
$ git log --graph
```

### ❏ Git branch

![](https://images.velog.io/images/abcd8637/post/29dff39f-ea97-4516-be34-45d2f5708cfa/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-30%2017.40.52.png)

1. branch: 독립적으로 어떤 작업을 진행하기 위한 개념, 각각의 `branch`는 다른 `branch`에 영향을 받지 않는다. 독립적 기능 단위, 작업 단위로 나눌 수 있다.
2. `main branch`: 배포할 수 있는 수준의 안정적인 `branch`
3. `topic branch`: 기능을 추가하거나 버그 수정과 같은 단위 작업을 위한 `branch` (수시로 내용이 변경 될 수 있음)
4. `git branch <name>`: branch 생성 명령어
5. `git branch`: 현재 `branch`의 정보를 보여주는 명령어
6. `git checkout <name>`: `branch` 전환 (`HEAD`는 현재 가리키고 있는 레포지토리를 말함)
7. `checkout`은 `branch`의 전환 뿐만 아니라 `git log`로 확인한 `snapshot`을 넘나들 때도 사용이 가능하다. (`git checkout snapshot hash`)

```shell
# checkout 전 snapshot hash
$ git log --pretty=oneline
e4abb6f... (HEAD -> master) this is master
d917274... another snapshot

$ git checkout d917274
...
HEAD is now at d917274 another snapshot

# checkout 후 snapshot hash
$ git log --pretty=oneline
e4abb6f... (master) this is master
d917274... (HEAD) another snapshot
```

8. 새로운 `branch`를 만들고 해당 `branch`로 이동하기
```shell
# 현재 branch 확인
$ git branch 

# "alice" branch 생성
$ git branch alice

# "alice" branch로 이동
$ git checkout alice
```

9. `fast-forward` 방식: `foo` `branch` 의 내용이 `master` `branch` 에서 업데이트 된 내용이기 때문에 곧바로 `merge` 가 된다. 즉 기존의 `master` `branch` 의 내용은 변한 것 없이 `foo` 브랜치의 내용만 합쳐졌기 때문에 `fast-forward` 방식이라고 할 수 있다.
10. 갈라지는 `branch` 의 `merge` 는 `git log --graph -all` 을 사용하면 `commit graph` 로 편하게 확인 할 수 있다.
11. `git branch -d <branch name>` : branch 삭제 명령어
12. `conflict`: 병합하는 두 `Branch` 에서 같은 파일을 변경 했을 때 충돌이 발생한다. 이때 `git status` 명령어로 어느 파일에서 충돌이 발생했는지 확인 할 수 있다. 수정 완료 후 `기호(<<<<< =====, >>>>>)`들을 삭제 해준다. 수정 완료 후 `git add`, `git commit` 과정을 거쳐서 다시 `merge` 한다. master 브랜치의 변화를 지속적으로 가져와서 충돌이 발생하는 부분을 제거한다. 더 좋은 것은 master 브랜치가 자주 변경되는 일이 없도록 하는 것

### ❏ 원격 저장소
1. 원격 저장소: 인터넷이나 네트워크 어딘가에 있는 저장소
2. `Git` 원격 저장소 받아오기: `Git clone url`(기존 repository를 복사), `clone` 버튼을 누르고 `CLI`창에 `$ git clone url`을 입력한다.
3. 원격 저장소와 로컬저장소 연결하기: `$ git remote add origin https://gitlab.com/group/project` (웹 호스트 서비스: gitlab.com, 그룹 명 group, 프로젝트 명 project) 이후 git remote 로 연결된 저장소가 무엇인지 볼 수 있음 `git remote show origin` 을 통해 어떤 원격 저장소가 있는지도 확인 가능 
4. 원격 저장소 동기화


```shell
1. `$ git pull`: 원격 저장소에서 데이터 가져오기 + 나의 로컬 레포지터리와 병합(Merge)한다. (따로 `merge`하지 않아도 적용됨.)
2. `$ git Fetch`: 원격 저장소에서 데이터 가져오기 (별개로 `merge` 단계를 거쳐야 한다.)
```

5. `origin/master`: 내 컴퓨터에 저장되어 있는 저장소와 원격저장소를 연결하기 위해서 다음의 명령어를 사용한다. `git remote add origin https://~` 여기서 `origin`은 원격저장소의 단축이름을 origin 으로 지정한다는 의미다. origin이 아닌 다른 이름으로도 원격 저장소의 이름을 지정해 줄 수도 있다. (`git remote add foo https://~`) 원격저장소의 이름의 `default` 값은 `origin` 이다. 따라서 `clone` 으로 복사해온 저장소의 이름은 `origin` 으로 통일하게 된다. `git remote -v` 명령어를 사용하면 지정한 저장소의 이름과 주소를 함께 볼 수 있다. 

---
## 📍 11.2.화(실시간 강의)
앨리스 교육을 받은 기간도 어느덧 2주째가 되었다. 저번주에는 `HTML/CSS` 파트를 배워서 못 따라갈 정도로 어렵다고 느끼진 않았다. 이번주부터는 본격적으로 `JS` 과정을 배우는데, 저번주와는 다르게 이론강의 4시간, 실습강의 3시간으로 나눠서 배웠다. 이후 `JS`를 배우는 커리큘럼은 괜찮지만 나중에 `this`, `closure` 과정을 배울 때는 못 따라가진 않을까 약간의 걱정이 된다. 하지만 처음엔 뒤쳐져도 꾸준히 공부하다보면 언젠간 다 따라잡을 수 있을 것이다.

### ❏ 저번시간 복습
1. git `HEAD` 혹은 `branch` 바꾸기: `git checkout <hash>`, `git checkout <branchName>`
2. 과거 상태의 `HEAD`로 `reset` 했을 때 지금까지의 모든 커밋 보기: `git log --oneline --all` 
3. 개발자 도구(f12)의 `CSS` 창은 상단부터 우선순위가 높은 속성값을 보여준다. (즉, 제일 위에 있는 속성값 먼저 적용된다는 얘기)
4. `git log` 중 `HEAD`나 `master`로 찾지 못하는 `commit`이 있다면 `git reflog` 사용하기
5. `git reset --hard hashId`: `HEAD`가 가리키는 브랜치를 움직인다.

### ❏ JS 이론 수업
1. `HTML` 코드에서 `JS`를 호출하려면 `<script src=""></script>`태그를 사용하자. (css 파일 불러오는 태그인 `<link rel="stylesheet" href="style.css(경로입력)">`)와 목적이 비슷하게 `JS` 파일을 따로 불러올 수 있다.
2. `document.write("attribute")`: 자바스크립트 출력문으로 어떤 정보를 `HTML` 화면에 출력하는 기능(실무에서는 거의 쓰이지 않는다.)
3. `<input type="button" value="buttonName">`: `button`을 만드는 태그
4. `event`: 사용자와 상호작용하는 모든 사건
5. `document.querySelector("body")`: `body` 태그를 가져오는 속성
6. `document.querySelector("#container")`: css `id` 선택자가 `container`인 값 가져오기
7. `document.querySelector("body").style.backgroundColor="red";`: body태그의 `style` `background-color` 바꾸기
8. 주간 / 야간 다크모드 구현

```html
<!-- 구현1: 주간 / 야간 두개의 버튼을 만들고 `onClick`시 바뀌는 기능을 추가한다. -->

<!-- 주간 모드 -->
<input type="button" value="day" onclick="
      document.querySelector('body').style.backgroundColor='white';
      document.querySelector('body').style.color='black';
">

<!-- 야간 모드 -->
<input type="button" value="night" onclick="
      document.querySelector('body').style.backgroundColor='black';
      document.querySelector('body').style.color='white';
" />

<!-- 리팩토링 1: 토글기능(한 개의 버튼으로 모드 변경 가능) -->
<input id="dn" type="button" value="night" onclick="
      var target = document.querySelector('#dn');
      if (target.value === 'night'){
        body.style.backgroundColor='black';
        body.style.color='white';
        target.value = 'day'
      }else{
        body.style.backgroundColor='white';
        body.style.color='black';
        target.value = 'night'
      }
  " />

<!-- 리팩토링 2: this 사용(id값을 설정 할 필요 없이 `this`를 통해 동일한 버튼이 여러개여도 각각의 기능을 보장한다. -->
  <input type="button" value="night" onclick="
      var target = this;
      if (target.value === 'night'){
        body.style.backgroundColor='black';
        body.style.color='white';
        target.value = 'day'
      }else{
        body.style.backgroundColor='white';
        body.style.color='black';
        target.value = 'night'
      }
  " />
```

9. 변수(parameter): 익명의 데이터에 이름을 붙이는 행위, 가독성이 증가하는 장점이 있다.
10. 비교연산자: `1===1`, `1>0`
11. 조건문: `if(true)`

### ❏ JS 실습 수업
1. 줄 바꿈하는 태그: `<br>`
2. 큰 따옴표와 작은 따옴표가 섞인 문장 출력하기: 큰 따옴표와 작은 따옴표 앞에 `\`를 붙여 출력

```javascript
// "It's all right."
document.write("It's all right.");
document.write('\"It\'s all right."');
```

3. `var`, `let`, `const`의 차이: 이전에 작성한 <a href='https://ywtechit.tistory.com/227?category=951122'>글</a> 참고
4. `==`, `===`의 차이: `==`은 좌항과 우항의 피연산자를 비교할 때 `암묵적 타입변환(implicit coercion)`으로 타입을 동일하게 일치시키고 같은 값인지 비교한다. 따라서 `==`는 좌항과 우항의 피연산자가 타입은 다르더라도 암묵적 타입 변환 후에 같은 값일 수 있다면 `true`를 반환한다. 반면, `===`는 좌항과 우항의 피연산자가 타입도 같고 값도 같은 경우에 한하여 `true`를 반환한다. 즉, 암묵적 타입 변환을 하지 않고 값을 비교한다. 따라서 일치 비교 연산자는 예측하기 쉽다.

```javascript
// (==), true
5 == 5;
5 == "5";
0 == '';
false = '0';
0 == -0;

// (==), false
"0" == '';
false == 'false';
false == null;
false == undefined;

// (===), true
5 === 5;
0 === -0;

// (===), false
5 === '5';
NaN === NaN;
```

5. `암묵적 타입변환(implicit coercion)`: `JS` 엔진은 표현식을 평가할 때 개발자의 의도와는 상관없이 코드의 문맥을 고려해 암묵적으로 데이터 타입을 강제 변환(암묵적 타입 변환)할 때가 있다.

6. 문자열 타입으로의 변환

```javascript
// 피연산자가 모두 문자열 타입이어야 하는 문맥
"10" + 2 // 102

// 피연산자가 모두 숫자 타입이어야 하는 문맥
5 * "10" // 50

// 피연산자 또는 표현식이 불리언 타입이어야 하는 문맥
!0 // true
if (1) {} // {}

// 숫자 타입
0 + '' // "0"
-0 + '' // "0"
1 + '' // "1"
-1 + '' // "-1"
NaN + '' // "NaN"
Infinity + '' // "Infinity"
-Infinity + '' // "-Infinity"

// 불리언 타입
true + '' // "true"
false + '' // "false"

// null
null + '' // "null"

// undefined
undefined + '' // "undefined"
```

7. 숫자 타입으로 변환: `빈 문자열('')`, `null`, `false`는 `0으`로 `true`는 `1로` 반환된다. 객체와 빈 배열이 아닌 배열, `undefined`는 변환되지 않아 `NaN`이 된다는 것에 주의하자.

```javascript
1 - "1" // 0
1 * "10" // 10
1 / 'one' // NaN

// 문자열 타입
+'' // 0
+'0' // 0
+'1' // 1
+'string' // NaN

// 불리언 타입
+true // 1
+false // 0

// null 타입
+null // 0

// undefined 타입
+undefined // NaN
```

8. 불리언 타입으로의 변환: 아래의 값들은 `falsy`로 평가되는 `Falsy`값이다. 이 값들 외에 값은 `truthy(참으로 평가되는 값)`라고 보면 된다.

```javascript
// 아래의 조건문은 모두 코드 블록을 실행한다.
if (!'') {console.log("execute")}; 
if (!false) {console.log("execute")}; 
if (!undefined) {console.log("execute")}; 
if (!null) {console.log("execute")}; 
if (!0) {console.log("execute")}; 
if (!NaN) {console.log("execute")}; 
```

reference
1. <a href='https://www.aladin.co.kr/shop/UsedShop/wuseditemall.aspx?ItemId=251552545'>모던 자바스크립트 딥 다이브</a>

---
## 📍 7일차 11.3.수.(실시간 강의)
오늘은 어제 배운 내용에 이어서 `JS` 기본 문법(object, function 등 )들을 배웠다. 강의 난이도는 2/5이다.

### ❏ 복습
1. `JS`를 실행하는 코드: `개발자 도구(F12)`, `<script>`, `onclick`
2. 이고잉님 추천 도서는 <a href='https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=236186172'>리팩터링 2판 - 마틴 파울러</a> 였는데, 내용의 40%는 변수 이름 설정의 중요성에 대해 설파했다고 한다. 
3. 변수(parameter): 익명의 데이터에 이름을 붙인 값

### ❏ 이론강의(4시간) + 실습강의(3시간)
1. 배열(array): 여러 개의 값을 순차적으로 나열한 자료구조다. 배열은 사용 빈도가 매우 높은 가장 기본적인 자료구조다. 자바스크립트는 배열을 다루기 위한 유용한 메서드를 다수 제공한다. 배열은 사용 빈도가 높으므로 배열 메소드를 능숙하게 다룰 수 있다면 코딩에 매우 도움이 된다. 배열이 가지고 있는 값을 `요소`, `element`, `색인`, `index`라고 부른다. 대부분의 프로그래밍 언어에서 인덱스의 시작은 보통 `0`부터 시작한다. `JS`도 예외는 아니다. 특이한 점은 자바스크립트에서 배열이라는 타입은 존재하지 않는다. 배열은 객체 타입이다. 배열은 객체이지만, 일반 객체와는 구별되는 독특한 특징이 있다. 일반 객체와 배열을 구분하는 가장 명확한 차이는 `값의 순서`와 `length 프로퍼티`다. 인덱스로 표현되는 값의 순서와 `length` 프로퍼티를 갖는 배열은 반복문을 통해 순차적으로 값에 접근하기 적합한 자료구조다.
또, 자바스크립트 배열은 인덱스로 배열 요소에 접근 할 때 일반적인 배열보다 느릴 수밖에 없는 구조적인 단점을 보완하기 위해 대부분의 모던 자바스크립트 엔진은 배열을 일반 객체와 구별하여 좀 더 배열처럼 동작하도록 최적화하여 구현했다. 다음과 같이 배열과 일반 객체의 성능을 테스트해보면 배열이 일반 객체보다 약 2배정도 빠르다는 것을 알 수 있다.

```javascript
// 배열 선언
const arr = ["apple", "banana", "orange"];

// 배열 순회
for(let i=0; i<arr.length; i++){
	console.log(arr[i]);
}

// 배열 타입: object
typeof([1, 2, 3]) // object

// 배열과 객체 순회 속도 비교
const array = [];
console.time("Array Performance Test");

for (let i=0; i<10000000; i++){
	array[i]=i;
}

console.timeEnd("Array Performance Test"); // 약 340ms

const obj = {};
console.time("Object Performance Test");

for (let i=0; i<10000000; i++){
	obj[i]=i;
}

console.timeEnd("Object Performance Test"); // 약 600ms
```

2. `html`에서 `a`태그 모두 선택하기: `document.querySelectAll("a")`
   
```javascript
// 배열 길이 만큼 li태그에 값 넣기
for (let i=0; i<names.length; i++){
   document.write(`<li><a href="${i}.html" target="_blank">${names[i]}</a></li>`)
}

// `a` 태그의 모든 값 색상 바꾸기
for (let i=0; i<aTags.length; i++){
    console.log(aTags[i].style.color = "red");
}
```

3. `debugger`: 코드 작성시 브라우저는 퍼즈(pause) 상태 이후 한 단계씩 진행한다.
4. `function 함수명(){}`: 함수명은 이름만 봐도 어떤 로직으로 구성되어 있을지 추론가능해야한다.

```javascript
// 2개의 인자를 받는 함수
function getAdditionalTax(price, tax){
	return price * tax;
}

console.log(getAdditionalTax(1000, 0.1));
👉🏽 100

// 인자에 값이 넘어오지 않으면 기본 값을 설정 할 수 있다.
function getAdditionalTax1(price, tax=0.1){
	return price * tax;
}

console.log(getAdditionalTax1(1000));
👉🏽 100
```

5. 다크모드 리팩토링2: 어제 작성했던 다크모드 리팩토링2 코드를 살펴보면 `input`태그 안에서 `onclick` 함수를 일일이 작성하여 가독성이 떨어진다는 단점이 있다. 이를 보완하기 위해 `onclick`을 담당하는 함수를 따로 빼내어 작성했다. 이 기능을 해결 할 때 `this`가 살짝 헷갈렸는데 결론적으로 `input` 태그 안에서 사용된 `this`는 `input`을 가리키고 있지만 `toggleDarkMode`의 인자 없이 `this`를 사용하게 되면 `전역객체(global)`를 바라보기 때문에 정상적으로 `input value`가 변경되지 않는다. 따라서 `input`에서 사용하는 `this`를 `toggleDarkMode(this)`처럼 인자로 넘겨주어 `input`의 `this`를 그대로 유지하게 만들자. (`this`는 누가 호출하느냐에 따라 달라지는데 `this`를 호출 할 때 `this` 앞에 객체가 명시되어 있는 경우 메서드로 호출한 것이고, 그렇지 않은 모든 경우는 함수로 호출한 것이다. 어떤 함수를 함수로서 호출할 경우에는 `this`가 지정되지 않는데, `this`가 지정되지 않는 경우 전역 객체를 바라보게 된다.)

```html
<!-- 리팩토링 전: onclick 기능을 일일이 나열하여 가독성이 떨어지는 단점이 있다. -->
  <input type="button" value="night" onclick="
      var target = this;
      if (target.value === 'night'){
        body.style.backgroundColor='black';
        body.style.color='white';
        target.value = 'day'
      }else{
        body.style.backgroundColor='white';
        body.style.color='black';
        target.value = 'night'
      }
  " />

<!-- 리팩토링 후: onclick 기능 코드만 따로 함수로 빼내어 가독성을 높였다. -->
<input type="button" value="night" onclick="toggleDarkMode(this);">
<script>
    const body = document.querySelector("body");
    
    function toggleDarkMode(target){
      if (target.value === "night"){
        body.style.backgroundColor = "black";
        body.style.color = "white";
        target.value = "day";

        let a = document.querySelectorAll("a");
        for (let i=0; i<a.length; i++){
          a[i].style.color = "white";
        }
        
      }else{
        body.style.backgroundColor = "white";
        body.style.color = "black";
        target.value = "night";

        let a = document.querySelectorAll("a");
        for (let i=0; i<a.length; i++){
          a[i].style.color = "black";
        }
      }
    }
  </script>

	<input type="button" value="night" onclick="toggleDarkMode(this)">
```

6. 객체: 서로 연관된 데이터와 처리방법을 그룹화해서 이름을 붙인 것

```javascript
let taxData = {
	price : 10000,
	tax = 0.1,
	calcTax = function(){
		return this.price * this.tax;
	}
}
```

reference
1. <a href='https://www.aladin.co.kr/shop/UsedShop/wuseditemall.aspx?ItemId=251552545'>모던 자바스크립트 딥 다이브</a>

---
## 📍 8일차 11.4.목.(온라인 강의)
오늘은 온라인 강의로 `JS` 기초문법을 배웠다. 어제 배운 내용에서 크게 벗어나지 않는 내용이었고 추가로 배운것은 `JS`로 입력받는 방법과 `match` 정규식에 대해서 배웠다.

### ❏ 자바스크립트 소개
1. 자바스크립트란 이미지 슬라이드 효과, 팝업 효과 등의 기능을 포함한 동적인 웹사이트 제작 시 사용되는 프로그래밍 언어 (HTML 은 웹사이트의 구조를 짜고, CSS 웹사이트를 꾸며주고, JS 는 사용자와 상호작용할 수 있게 만들어준다.)
2. 자바스크립트 사용분야 : IoT(예: 전동커튼), 하이브리드 앱(예: 네이버 앱), 서버 개발(node.js)

### ❏ 자바스크립트 변수
1. 변수란? 데이터를 담는 공간

```javascript
var fruit;  // 변수 선언: 데이터를 담을 공간을 생성하는 것
fruit = "apple";  // 변수 초기화: 생성된 변수에 공간을 생성하는 것

var fruit = "apple";  // 변수 선언 및 초기화
```

2. 데이터 변경: 변수 `fruit` 의 데이터를 `apple` 에서 `banana`로 변경했지만 변수는 이미 앞서 선언되었으므로 `var`로 다시 선언 할 필요가 없다.

```javascript
var fruit = "apple";
fruit = "banana";
```

3. 변수 데이터 확인: `console.log()`

```javascript
var fruit = "apple";
console.log(fruit);
```

4. 변수 생성 시 주의 사항
```javascript
// 변수명은 숫자로 시작 할 수 없음
var 1str;

// 변수명은 최대한 자세하게 작성
var randomNumber;

// 의미가 불명확한 단어들의 조합은 피해야 함
var tmax;
```

5. 자바스크립트 사용 방법: `<script>` 태그 안에 `src` 속성 값으로 `js` 파일을 입력 후 `html`파일과 연동

```javascript
<body>
	<script src="index.js"></script>
</body>
```

6. 변수 데이터 확인 방법: 우 클릭 후 크롬 개발자 검사 or F12
7. `document.write()` : 변수의 데이터를 웹 화면에 출력하는 코드
8. `document.writeln()` : 출력값 사이에 공백을 넣는 코드

### ❏ 자바스크립트 데이터 타입
1. 데이터 타입: 초콜릿도 다양한 종류가 존재하듯, 변수에 전달되는 데이터 타입에도 여러가지 타입이 존재한다.
2. 데이터 타입의 종류: `string`, `number`, `boolean`, `function`, `object`, `undefined`, `null`, `array`
3. 문자열(`string`)

```javascript
var str1 = "Hello";
var str2 = 'i am';
var str3 = "27";  // 숫자가 아닌 문자열

var str4 = "Elice'; // 혼용 불가
var str5 = "He's a boy";
var str6 = 'He\'s a boy';  // 감싸주는 따옴표와 동일한 따옴표를 붙이려면 따옴표 앞에 `\`를 붙여주자.
```

4. 숫자(`number`)

```js
var num1 = 10;
var num2 = -10;
var num3 = 3.14;
var num4 = Number.MAX_SAFE_INTEGER  // 9007199254740991
var num5 = Number.MIN_SAFE_INTEGER  // 9007199254740991
```

5. 함수(`function`)

```js
// 함수 표현식
var func1 = function(){
	console.log("func1");
}  // 함수 생성

func1();  // 함수 호출

// 함수 선언식
function func2(){
	console.log("func2");
}

// 매개변수: width, height
var area = function(width, height){
	return width * height;
}

// 함수 호출 및 인자 전달
area(10, 20);

// 함수 데이터 호출방법
var result = area(10, 20);
console.log(result);

console.log(area(10, 20));
```

6. 배열(`array`): 비슷한 성격을 갖고 있는 데이터를 하나의 변수 안에서 관리

```js
var fruit = ["사과", "배", "수박"];
console.log(fruit);

// 데이터 좌표값(index) 작성, 첫번째 좌표값은 0
console.log(fruit[0]);

// 배열 데이터 변경하기
fruit[0] = "포도";
```

7. 객체(`object`): 프로퍼티, 메서드, 데이터로 구성, 여러 종류의 데이터 타입 삽입 가능

```js
var student = [
	name : "AYW",
	age : 27,
	stack : ["JS", "TS"],
	sum : function (num1, num2) { return num1 + num 2};
]

// 객체 데이터 출력하기
console.log(student.name);
console.log(student["name"]);

// 객체 데이터 변경하기
student.name = "AYJ"
console.log(student.name);
```

8. `undefined`: 변수 안에 데이터를 입력하지 않은 상태(데이터가 없는 것)
9. `null`: 개발자가 임의로 변수 안에 빈 데이터를 삽입한 상태(빈 데이터를 지정한 것)

```js
var unde;
var empty = null;
```

10. `boolean`: `true`, `false`

```js
var t = true;
var f = false;
```

### ❏ 자바스크립트의 프로퍼티와 메서드
1. 프로퍼티, 메서드: `js`에서 사용자를 위해 사전에 작성된 편의 기능
2. 문자열 메서드

```js
var str1 = "Hello World";
str1.length;  // 문자열 길이 11
str1.charAt(0);  // 문자열 추출
str1.split(' ');  // 공백 기준으로 문자를 나누고 배열에 담는 메서드
```

3. 배열 메서드

```js
var fruit = ["사과", "배", "포도"];
fruit.length;
fruit.push("딸기");  // 배열 뒤에 데이터 삽입
fruit.unshift("레몬");  // 배열 앞에 데이터 삽입
fruit.pop();  // 배열 뒤의 데이터 제거
fruit.shift();  // 배열 앞의 데이터 제거
```

4. `math` 의 수학 연산 메서드

```js
Math.abs(-3) // 절대값
Math.ceil(0.3) // 올림
Math.floor(10.9)  // 내림
Math.random()  // 임의의 숫자 출력
```

5. 문자를 숫자로 변환하는 메서드

```jsx
parseInt("20.6")  // 정수 형태의 20 변환
parseFloat("20.6")  // 실수 형태의 20.6 변환
```

6. 자바스크립트 출력시 역 슬래시(`\`)의 출력과 `\n` 같은 이스케이프 시퀀스를 구분하기 위해서는 앞에 `\` 를 붙여준다.

### ❏ 자바스크립트로 입력 받기

```javascript
const readline = require("readline");
const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

// 한번 입력 받고 출력
rl.on("line", (line) => { 
    // 한 줄씩 입력받은 후 실행할 코드
    // 입력된 값은 line에 저장된다.
		console.log(line)
    rl.close(); // close가 없으면 입력을 무한히 받는다.
});
rl.on('close', () => {
    // 입력이 끝난 후 실행할 코드
})

// 입력이 한 줄 공백으로 주어질 때 
let input = [];
rl.on("line", function (line) {
  input = line.split(" ");
	r1.close();
}).on("close", function () {
  console.log(input);
});
```

### ❏ 자바스크립트 match 정규식
1. 다음 문자열 중 `e` 의 개수는 몇 개인가?

```js
let lorem = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias iste tempore voluptatem architecto pariatur obcaecati provident sint neque. Ratione debitis officia quo? Vero tempora sequi laborum maxime fugiat fuga sapiente?" 

// 정규식 
console.log(lorem.match(/e/g).length);
👉🏽 23

// 반복문
let cnt=0;
for (let x of lorem){
	if(x === "e") cnt++ 
}
console.log(cnt);
👉🏽 23
```

---
## 📍 9일차 11.5.금.(온라인 강의)
오늘은 어제에 이어서 `JS` 기초 문법 및 활용에 대해서 배웠다. 문법은 어렵지 않았는데 문제를 풀 때 `edge Case`가 잘 떠오르지 않아서 조금 헤맸다.

### ❏ 자바스크립트 기초 문법 및 활용

### ❏ 연산자
1. 산술 연산자: 사칙연산, `%(나머지)` , 숫자 뿐만 아니라 문자열도 산술 연산자 사용 가능 (문자열은 서로 붙어서 출력된다. `+` 는 문자열이 붙여서 출력, 나머지는 숫자로 바꿔서 계산)

```js
console.log(20 + 10);  // 30
console.log(20 - 10);  // 10
console.log(20 * 10);  // 200
console.log(20 / 10);  // 2
console.log(20 % 10);  // 0
```

2. 증감 연산자: `++`: 1씩 증가, `--`: 1씩 감소 (전치연산자는 먼저 연산을 하고 출력한다. 후치연산자는 먼저 출력을 하고 연산한다.)

```js
let num = 10;

console.log(++num);  // 11
console.log(--num);  // 10

console.log(num++);  // 10
console.log(num--);  // 11
```

3. 비교 연산자: 데이터의 대소비교

```js
console.log(10 == 20);  // false, 값이 같다
console.log(10 === 20);  // false, 데이터 타입도 같고 값도 같다.
console.log(10 !== 20);  // true

console.log(10 > 20);  // false
console.log(10 >= 20);  // false
console.log(10 < 20);  // true
console.log(10 <= 20);  // true
```

4. 논리 연산자

```jsx
console.log(10 === 10 && 20 === 30);  // false, 앞 뒤 조건 모두 참인 경우만 true를 반환하는 AND 연산자
console.log(10 === 10 || 20 === 30);  // true, 둘 중 하나만 참이여도 true를 반환하는 OR 연산자
```

### ❏ 조건문
1. `if` 문: `if(조건){수행할 명령}`

```js
let a = 20;
let b = 40;
if( a < b){
	console.log("a는 b보다 작다.");
}
```

2. `if-else` 문: 조건이 `true` 면 `if`문, `false` 면 `else` 문 실행

```js
let a = 20;
let b = 40;

if( a < b){
	console.log("a는 b보다 작다.");
} else {
	console.log("a는 b보다 작거나 같다.");
}
```

3. `else-if` 문: 여러 개의 조건문을 생성할 때 사용, 참인 조건이 여러개면 위에서부터 참인 조건문만 반환

```jsx
let a = 20;
let b = 40;
let c = 60;

if( a > b){
	console.log("a는 b보다 크다.");
} else if (b > c){
	console.log("b는 c보다 크다.");
} else if (a < c){
	console.log("a는 c보다 작다.");
} else if (b < c){
	console.log("b는 c보다 크다.");
} else {
	console.log("모든 조건을 만족하지 않는다.");
}
```

4. `중첩 if문` : if문 안에 또 다른 if문을 삽일 할 때 사용

```jsx
let a = 20;
let b = 40;

if( a !== b){
	if (a > b) console.log("a는 b보다 크다");
	else console.log("a는 b보다 작다");
} else {
	console.log("a와 b는 같다.");
}
```

### ❏ 반복문
1. `for` 문: `for( 초기화 한 변수값; 조건; 증감 표시){ 수행할 명령 }`

```js
for (let i=0; i<10; i++){
	console.log(i);
}
```

2. `while` 문: `while( 조건 ) {수행할 명령}`

```js
let num = 0;

while (num < 10){
	console.log(num);
	num++;
} 
```

3. `do - while` 문: `do {수행할 명령} while (조건)`, `while` 의 조건과 관계없이, `do` 의 명령을 무조건 실행부터 한다. (재시도를 테스트하는 상황에 활용가능)

```jsx
let i = 12;

do {
	console.log(i);
	i++;
} while (i < 10);
```

### ❏ 자바스크립트 활용
자바스크립트를 이용하여 구현 문제들을 풀었는데, 강의에서 배운 코드 대신 내가 작성한 코드를 올린다. (테스트 문제는 올리지 않겠다.)

1. 주사위 게임

```js
// 1. Math.random(): 0 ~ 1사이 랜덤한 값을 출력한다.
// 2. Math.random() * 6: 0 ~ 6사이 랜덤한 값을 출력한다.
// 3. (Math.random() * 6) + 1: 1 ~ 6 사이 랜덤한 값을 출력한다.
// 4. Math.floor((Math.random() * 6) + 1): 소수점을 버린다.
let dice = Math.floor(Math.random() * 6) + 1;
```

2. 소수 출력하기: <a href='https://ywtechit.tistory.com/13'>이전</a>에 프로그래머스에서 한번 푼적 있는데 하단의 코드로 풀면 시간복잡도를 효과적으로 줄일 수 있다.

```js
// 나의 코드
function isPrime(n){
    if(n === 1) return false;
    for (let i=2; i<Math.floor(n/2)+1; i++){
        if (n%i===0) return false;
    }
    return true;
}
```

3. 문자열 거꾸로 출력하기: 강의에서는 `charAt`메소드를 사용했는데 그것보다 문자열 인덱싱으로 풀었다.

```jsx
// 나의 코드
function reverse(str){
    var reverStr = "";
    for (let i=str.length-1; i>=0; i--){
        reverStr += str[i];
    }
    return reverStr;
}

document.write(reverse("Nice to meet you"));
```

4. 구구단 출력하기

```js
for(let i=2; i<=9; i++) {
    for(let j=1; j<=9; j++){
        document.write(`${i}x${j}=${i*j}`);
        document.write("<br>")
    }
    
}

timesTable(2); // 2단만 출력
timesTable(3); // 3단만 출력
```

---
## 📍 10일차 11.6.토.(자기소개 홈페이지 만들기)
오늘은 강의 대신 `HTML`, `CSS`, `JS`를 이용해서 자기소개 페이지를 만드는 과제가 있었다. 주제는 어렵지 않은데 이것저것 추가하다 보니까 다른기능을 추가하고 싶다는 생각이 많이 들어서 섣불리 끝나지는 않았다. `GitLab`에 파일을 배포하는 형식으로 진행했다. 디자인에 잼병인 내가 어떻게 홈페이지를 꾸며볼까 하다가 <a href='https://dribbble.com/'>dribble</a>이라는 사이트에서 괜찮은 템플릿을 하나 골라 비슷하게 만들었다. `header`에는 `navbar` 대신 `img`를 `blur` 처리해서 넣었고, 가운데에 선명한 사진을 또 넣었다. `body`에는 과제에 포함해야하는 질문들을 포함해서 넣었고 글만 넣기에는 뭔가 심심해서 `toggle` 버튼을 넣었다. 그리고 나의 스택을 쉽게 알려주는 사이트인 <a href='https://shields.io/'>shields.io</a>에서 `img`를 따왔다. 마지막으로 `footer`에는 내가 지금까지 만든 포트폴리오의 링크를 첨부했다. 결과물은 이 <a href='http://ywtechit.kdt-gitlab.elice.io/produce-myself/'>사이트</a>에서 볼 수 있다.

---
## 📍 11일차 11.9.화.(실시간 강의)
오늘은 오랜만에 비가 내려서 새벽런닝을 하지 못했고 날씨도 급격하게 추워졌다. 벌써 11월이라니.. 2021년 올해도 벌써 1달 조금 넘게밖에 남지 않았다. 내년 2월까지 최선을 다하자..! 저번시간에 `JS I`을 통해 자기소개 <a href='http://ywtechit.kdt-gitlab.elice.io/produce-myself/'>홈페이지</a>를 만들었고, 이번주는 진도를 더 나가서 `JS II`를 배우게된다. `DOM`, `Event`, `this`, `closure` 등에 대해서 배우는데 이번주차는 어려운 파트기 때문에 복습을 더 열심히 해야겠다는 생각을 했다.

### ❏ 저번주 복습
1. `indexOf(target)`: `target`이 `index` 몇 번째에 위치해있는지 반환하는 메소드(없으면 `-1` 반환)
2. 함수에 `return` 값이 없으면 `js`엔진이 `undefined`를 리턴한다. (여담으로 `JS`엔진이 `undefined`를 반환하는 경우는 3가지가 있는데 `변수에 값을 할당하지 않은 경우`, `객체 프로퍼티에 값이 없는 경우`, `함수에 리턴값이 없는 경우`이다.)

### ❏ 브라우저의 렌더링 과정
1. 브라우저는 `HTML`, `CSS`, `JS`, `img`, `font` 등 렌더링에 필요한 리소스를 요청하고, 서버로부터 응답을 받는다.
2. 브라우저의 렌더링 엔진은 서버로부터 응답된 `HTML`, `CSS`를 파싱하여 `DOM`과 `CSSOM`을 생성하고 이들을 결합하여 렌더 트리를 생성한다.
3. 브라우저의 `JS` 엔진은 서버로부터 응답된 `JS`를 파싱하여 `AST(Abstract Syntax Tree)`를 생성하고, 바이트코드로 변환하여 실행한다. 이때 `JS`는 `DOM API`를 통해 `DOM`이나 `CSSOM`을 변경할 수 있다. 변경된 `DOM`과 `CSSOM`은 다시 렌더트리로 결합된다.
4. 렌더 트리를 기반으로 `HTML` 요소의 레이아웃(위치와 크기)을 계산하고(리플로우), 브라우저 화면에 `HTML` 요소를 페인팅한다.(리페인팅) 

### ❏ DOM을 파싱하는 과정
1. 위 `브라우저의 렌더링 과정`에서 `2`번 과정을 조금 더 자세하게 설명하자면 브라우저의 요청에 의해 서버가 응답한 `HTML` 코드만으로는 브라우저가 이해할 수 없다. 따라서 일련의 과정을 거쳐 브라우저가 이해할 수 있도록 바꿔줘야 하는데 `바이트` -> `문자` -> `토큰` -> `노드` -> `DOM`의 과정을 거친다. 
2. `바이트(byte)`: `HTML` 파일이 브라우저 요청에 의해 응답되는데, 서버는 브라우저가 요청한 `HTML` 파일을 읽어 들여 메모리에 저장한 다음, 메모리에 저장된 바이트(2진수)를 인터넷을 경유하여 응답한다. 
3. `문자`: 2진수 형태의 `HTML` 문서는 `<meta charset="UTF-8">`코드에 의해 문자열로 변환된다. 
4. `토큰(token)`: 문자열로 변환된 `HTML` 문서를 읽어 문법적 의미를 갖는 코드의 최소 단위인 `토큰(token)`으로 분해한다.
5. `노드(node)`: 각 토큰들을 객체로 변환하여 `node`를 생성한다. 토큰의 내용에 따라 `문서 노드`, `요소 노드`, `어트리뷰트 노드`, `텍스트 노드`가 생성된다. 노드는 이후 `DOM`을 구성하는 기본 요소가 된다.
6. `DOM`: `HTML` 요소는 중첩관계를 갖는데, 이러한 `HTML` 요소간의 부자관계를 반영하여 모든 노드들을 `트리 자료구조`로 구성한다. 이 노드들로 구성된 트리 자료구조를 `DOM(Document Object Model)`이라 부른다. 즉, `DOM`은 `HTML` 문서를 파싱한 결과물이다. 이 `DOM` 형태가 되어야 `js` 언어로 객체 형태에 접근이 가능하다.

### ❏ DOM(Document Object Model)
1. `HTML` 문서의 계층적 구조와 정보를 표현하며 이를 제어 할 수 있는 `API`, 즉 프로퍼티와 메소드를 제공하는 트리 자료구조다.
2. `HTML element`: `HTML 요소`는 `HTML` 문서를 구성하는 개별적인 요소를 의미한다. 예를 들어 `<div class="greeting">Hello</div>`와 같은 코드에서 `class`는 어트리뷰트 값(attribute value)이고 어트리뷰트 노드로 변환된다. `Hello`는 콘텐츠(contents)를 뜻하며 텍스트 콘텐츠는 텍스트 노드로 변환된다.

### ❏ 요소 노드 취득
1. `HTML` 요소 노드를 가져오고 싶을 땐 다음의 4가지 방법을 이용하자.
2. `Document.prototype.getElementById("id")`: 인수로 전달한 `id` 어트리뷰트 값을 갖는 하나의 요소 노드를 탐색하여 반환한다. 이때 문서노드인 `document`를 통해 호출하자. `class` 어트리뷰트와는 달리 동일한 `id` 태그 여러개가 겹쳐도 제일 처음의 노드 1개만 반환한다.
3. `Document.prototype.getElementsByTagName("Tag")`: 인수로 전달한 태그 이름을 갖는 모든 요소 노드들을 탐색하여 반환한다. 이때 여러 개의 요소 노드 객체를 갖는 `HTMLCollection` 객체를 반환한다. `HTMLCollection`은 유사배열개체이며, 이터러블하다.
4. `Document.prototype.getElementsByClassName("class")`: 인수로 전달한 `class` 어트리뷰트 값을 갖는 모든 요소 노드들을 탐색하여 반환한다. `getElementsByTagName` 메서드와 마찬가지로 `HTMLCollection`객체를 반환한다.
5. `Document.prototype.querySelector`: 인수로 전달한 `CSS` 선택자를 만족시키는 하나의 요소 노드를 탐색하여 반환한다.
6. `Document.prototype.querySelectorAll`: 인수로 전달한 `CSS` 선택자를 만족시키는 모든 요소 노드를 탐색하여 반환한다. `getElement` 메서드와는 다르게 `NodeList` 객체를 반환하는데 유사배열개체이며, 이터러블하다.
7. `CSS 선택자 문법`을 사용하는 `querySelector`, `querySelectorAll` 메서드는 `getElementsBy*~`보다 다소 느리지만 `CSS` 선택자 문법을 사용하여 좀 더 구체적인 조건으로 요소 노드를 취득할 수 있고, 일관된 방식으로 요소 노드를 취득할 수 있는 장점이 있다. 따라서 `id` 어트리뷰트가 있는 요소 노드를 취득할 때는 `getElementById` 메서드를 사용하고 그 외의 경우 `querySelector`, `querySelectorAll` 메서드 사용을 권장한다.
8. 앞서 `4`번과 `7`번에서 등장한 `HTMLCollection`와 `NodeList`의 차이점은 다음에 알아보자.

### ❏ 자식노드 탐색
1. `Node.prototype.childNodes`: 자식 노드를 모두 탐색하여 `NodeList`에 담아 반환한다. `childNodes` 프로퍼티가 반환한 `NodeList`에는 요소노드뿐 아니라 텍스트 노드도 포함되어 있다.
2. `Element.prototype.children`: 자식 노드 중 요소 노드만 탐색하여 `HTMLCollection`에 담아 반환한다. 텍스트 노드가 포함되지 않는다.

### ❏ event
1. event는 내일 이론강의 수강 이후 작성하겠다.

reference
1. <a href='https://www.aladin.co.kr/shop/UsedShop/wuseditemall.aspx?ItemId=251552545'>모던 자바스크립트 딥 다이브</a>

---
## 📍 12일차 11.10.수.(온라인 강의)
오늘은 `DOM`과 `event`를 온라인강의로 배우는 날이다. 이전 챕터와는 다르게 `DOM`은 자주 다뤄보지 않은 개념이어어서 관련 문제를 푸는데 오래걸렸다. 익숙해질때까지 반복해야겠다. `DOM`에 관한 기본적인 개념은 어제 다뤘기 때문에 오늘은 `event`를 집중적으로 다뤄볼까 한다.

### ❏ `DOM`과 이벤트 소개
1. `DOM(Document Object Model)`: 문서 객체모델, 객체 지향 모델로써 구조화된 문서를 표현하는 방식(문자열로 된 코드를 트리구조 형태로 바꿔주는 것)
2. `DOM` 은 `XML` 이나 `HTML` 문서의 구조화된 표현을 제공하여 프로그래밍 언어가 문서 구조, 스타일, 내용 등을 변경할 수 있도록 한다. 
3. `DOM` 의 종류: `Core DOM`(모든 문서타입을 위한 모델), `HTML DOM`(HTML 문서를 위한 모델), `XML DOM` (문서를 위한 모델)
4. `Document`: 웹 페이지 자체를 의미하며, 웹 페이지에 존재하는 `HTML` 요소에 접근할 때는 `Document` 객체부터 시작해야 한다.
5. `Document Method`: HTML 요소 선택, 요소 생성, 이벤트 핸들러 추가, 객체의 선택

### ❏ 자바스크립트와 DOM
1. dom 요소의 선택: `Document.prototype.getElementById("id")`, `Document.prototype.getElementsByTagName("Tag")`, `Document.prototype.getElementsByClassName("class")`, `Document.prototype.querySelector`, `Document.prototype.querySelectorAll`
2. `dom` 스타일 변경: `document.getElementById("id").style.color = "red`
3. `dom` 내용 변경: `document.getElementById("id").innerHTML = "Hi"`

### ❏ Node 객체
1. 노드: `HTML DOM` 에서 정보를 저장하는 계층적 단위, 노드 트리는 노드들의 집합으로, 노드 간의 관계를 나타낸다. `JS`에서는 `HTML DOM` 을 이용하여 노드 트리에 포함된 모든 노드에 접근할 수 있다.
2. 노드 트리의 모든 노드는 서로 계층적 관계를 맺고 있다.
3. 노드의 종류: `문서 노드(document node)`(HTML 문서 전체를 나타내는 노드), `요소 노드(element node)`(모든 HTML 요소는 요소 노드로 속성을 가질 수 있는 유일한 노드), `주석 노드(comment node)`(HTML 문서의 모든 주석은 주석노드), `속성노드(attribute node)` (해당 요소 노드의 자식 노드에는 포함되지 않는다.), `텍스트 노드(text node)`(HTML 문서의 모든 텍스트는 텍스트 노드)

### 💡 nodeType 프로퍼티 값: `nodeType` 값은 텍스트가 아닌 숫자로 표현됩니다.

```jsx
요소 노드(Element Node): 1
속성 노드(Attribute Node): 2
텍스트 노드(Text Node): 3
주석 노드(Comment Node): 8
문서 노드(Doucment Node): 9
```

4. 노드 타입 접근 예제
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>자바스크립트 기초</title>
</head>
<body>
    <div name="red"  class="fruit" id="apple">apple</div>
		<div name="yellow" class="fruit" id="banana">banana</div>
    <div name="red"  class="vegetable" id="carrot">carrot</div>
		<div name="white"  class="vegetable" id="onion">onion</div>
<script src="index.js"></script>
</body>
</html>
```

```javascript
let $apple = document.getElementById("apple").childNodes[0];  // "apple"
let $appleNodeValue = $apple.nodeValue;  // "apple"
let $appleNodeType = $apple.nodeType;  // 3(텍스트 노드)
```

### ❏ 이벤트(Event)
1. 이벤트(Event): 웹 브라우저가 알려주는 HTML 요소에 대한 사건의 발생, JS는 발생한 이벤트에 반응하여 특정 동작을 수행할 수 있다. (mouse, scroll, keyboard, window 객체 등)

```javascript
// 마우스 클릭 이벤트 예시
<p onclick = "changeText(this)"> 여기를 클릭해주세요</p>

function changeText(element){
	element.innerHTML = "내용이 바뀌었읍니다."
}
```

2. 이벤트 핸들러: 이벤트가 발생했을 때 그 처리를 담당하는 함수. 지정된 이벤트가 발생하면 웹 브라우저에게 등록된 이벤트 핸들러 함수호출을 위임하게 된다.

```js
// HTML 문서가 로드될 때 실행됨
window.onload = function(){
	let text = document.getElementById("text");
	text.innerHTML = "HTML 문서가 로드되었읍니다."
}
```

3. 이벤트 타입: 이벤트의 종류를 나타내는 문자열이다. 약 200여가지의 타입이 있는데, <a href='https://developer.mozilla.org/ko/docs/Web/Events'>`MDN`</a>을 참고하자.

### 💡 이벤트 핸들러 등록
1. 이벤트가 발생했을 때 브라우저에게 이벤트 핸들러의 호출을 위임하는 것
2. 어트리뷰트 방식: 함수 호출문 등의 문을 할당하면 이벤트 핸들로가 등록된다. `HTML`과 자바스크립트는 관심사가 다르므로 혼재하는 것보다 분리하는 것이 더 좋다. 하지만 `Vue`를 담당하는 `Angular/React/Svelte/Vue.js` 같은 프레임워크 / 라이브러리에서는 이벤트 핸들러 어트리뷰트 방식으로 이벤트를 처리한다. 뷰를 구성하기 위한 구성 요소로 보기 때문에 관심사가 다르다고 생각하지 않는다.

```html
<html>
	<body>
		<button onclick="sayHi('Lee')">Click me!</button>
		<script>
			function sayHi(name){
				console.log(`Hi! ${name}`);
			}
		</script>
	</body>
</html>
```

3. 이벤트 핸들러 프로퍼티 방식: `DOM` 노드 객체는 이벤트에 대응하는 이벤트 핸들러 프로퍼티를 가지고 있다. 이벤트 핸들러 프로퍼티에 함수를 바인딩하면 이벤트 핸들러가 등록된다. `2`번에서 살펴본 어트리뷰트의 단점을 보완한 케이스이다. 하지만 이벤트 핸들러 프로퍼티에 하나의 이벤트 핸들러만 바인딩 할 수 있다는 단점이 있다.

```html
<html>
	<body>
		<button id="btn">Click me!</button>
		<script>
			const $button = document.getElementById("btn");

			$button.onclick = function () {
				console.log("button click!");
			}
		</script>
	</body>
</html>
```

4. `addEventListener` 이벤트 방식: 이벤트 핸들러 프로퍼티 방식과는 달리 `on` 접두사를 붙이지 않는다. 두 번째 매개변수에는 이벤트 핸들러를 전달한다. 마지막 매개변수에는 이벤트를 캐치할 이벤트 전파 단계(캡처링 또는 버블링)를 지정한다. 생략하거나 `false`로 지정하면 버블링 단계에서 이벤트를 캐치하고, `true`를 지정하면 캡처링 단계에서 이벤트를 캐치한다. `3`번 과정과는 다르게 하나 이상의 이벤트 핸들러를 등록할 수 있다. 이때, 이벤트 핸들러는 등록된 순서대로 호출한다.

```html
<html>
	<body>
		<button id="btn">Click me!</button>
		<script>
			const $button = document.getElementById("btn");

			$button.addEventListener("click", function(){
					console.log("button click!");
			});
		</script>
	</body>
</html>
```

### ❏ DOM 요소의 기본 동작 조작
1. `DOM` 요소는 저마다 기본 동작이 있다. 예를 들어 `a` 요소를 클릭하면 `href` 어트리뷰트에 지정된 링크로 이동하고, `checkbox` 혹은 `radio`를 클릭하면 체크 또는 해제된다. 이벤트 객체의 `preventDefault()` 메서드는 이러한 `DOM` 요소의 기본 동작을 중단시킨다.

```html
<html>
	<body>
		<a href="#">Click me!</a>
		<input type="checkbox">
		<script>
			const $a = document.getElementsByTagName("a")[0];
			$a.addEventListener("click", function(e){
				e.preventDefault();
			});

			const $input = document.querySelector("input[type=checkbox]");
			$input.addEventListener("click", function(e){
				e.preventDefault();
			})
		</script>
	</body>
</html>
```

### ❏ 이벤트 핸들러 내부의 this
1. 다음 예제의 `handleClick` 함수 내부의 `this`는 전역 객체 `window`를 가리킨다.

```html
<html>
	<body>
		<button onclick="handleClick(this)">Click Me</button>
		<script>
			function handleClick(button){
				console.log(button);  // button 요소
				console.log(this);  // window
			}
		</script>
	</body>
</html>
```

![](https://images.velog.io/images/abcd8637/post/78888e26-14e5-479d-81d4-b43dca931fea/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-11-10%2020.01.38.png)

2. 이벤트 핸들러 프로퍼티 방식: `addEventListener` 메서드와 동일하게 모두 이벤트 핸들러 내부의 `this` 는 이벤트를 바인딩한 `DOM` 요소를 가리킨다. 즉, 이벤트 핸들러 내부의 `this` 는 이벤트 객체의 `currentTarget` 프로퍼티와 같다.
    
```html
<!DOCTYPE html>
<html lang="en">
<body>
  <button id="btn">Click me!</button>
  <script>
    const $button = document.querySelector("#btn");
    
    $button.onclick = function(e){
      console.log(this)
      console.log(e.currentTarget)
      console.log(this === e.currentTarget)
    }
  </script>  
</body>
</html>
```
    
![](https://images.velog.io/images/abcd8637/post/c9e9e6cd-683d-4e3b-ac4b-47f3584ce8de/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-11-10%2020.03.38.png)

3. `addEventListener`

```html
<!DOCTYPE html>
<html lang="en">
<body>
  <button id="btn">Click me!</button>
  <script>
    const $button = document.querySelector("#btn");
    
    $button.addEventListener("click", function(e){
      console.log(this);
      console.log(e.currentTarget);
      console.log(this === e.currentTarget)
    })
  </script>  
</body>
</html>
```

![](https://images.velog.io/images/abcd8637/post/7a2dc9ec-9be0-49c5-b791-a1449087836b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-11-10%2020.05.03.png)

4. 화살표 함수로 정의한 핸들러 내부: 이벤트 핸들러 내부의 `this` 는 상위 스코프의 `this` 를 가리킨다. 화살표 함수는 함수 자체의 `this` 바인딩을 갖지 않는다.
    
```html
<!DOCTYPE html>
<html lang="en">
<body>
  <button id="btn">Click me!</button>
  <script>
     const $button = document.querySelector("#btn");
    
    $button.onclick = e => { 
      console.log(this)
      console.log(e.currentTarget)
      console.log(this === e.currentTarget)
    }

    const $button = document.querySelector("#btn");
    
    $button.addEventListener("click", (e) => {
      console.log(this);
      console.log(e.currentTarget);
      console.log(this === e.currentTarget)
    })
  </script>  
</body>
</html>
```

![](https://images.velog.io/images/abcd8637/post/d8b4152a-0bd8-4aed-bf82-a03f2ffbe16f/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-11-10%2020.07.35.png)

---
## 📍 13일차 11.11.목.(실시간 강의)
오늘은 `JS`에서 어려운 문법인 `scope`, `this`, `실행 컨텍스트`, `함수`, `restParameter`에 대해서 배웠다. 이 내용들은 저번에 읽었던 <a href='https://ywtechit.tistory.com/325?category=952803'>코어 자바스크립트</a>에 나왔던 내용이다. 책을 읽은지 약 2개월정도밖에 안됐는데 부분부분 까먹은 내용들이 있었다. 까먹지 않게 틈틈이 읽어야겠다.

### ❏ 스코프
1. 변수가 작동하는 유효범위
2. 변수에 접근 할 수 있는 범위
3. `Global`: 어느곳에서든지 해당 변수에 접근할 수 있다. `Local`: 해당 지역에서만 접근할 수 있다.

### ❏ 실행 컨텍스트
1. 실행 컨텍스트를 바르게 이해하면 스코프를 기반으로 식별자와 식별자에 바인딩 된 값(식별자 바인딩)을 관리하는 방식과 호이스팅이 발생하는 이유, 클로저의 동작 방식, 그리고 태스크 큐와 함께 동작하는 이벤트 핸들러와 비동기 처리의 동작 방식을 이해할 수 있다. 
2. `전역 실행 컨텍스트(GEC: Global Execution Context)`: JS가 실행될 때 가지고 시작함. `JS`에서 유일하게 하나만 존재한다. (`script`코드로 `js` 파일을 독립적으로 실행해도 전역변수는 공유된다.)
3. `지역 실행 컨텍스트(FEC, Functional Execution Context)`: 다수의 `FEC`가 존재 할 수도 있고, 존재하지 않을 수도 있다. `FEC`는 함수단위로 실행된다. 함수 호출 시 `FEC`가 생성된다.
4. 실행 컨텍스트에서 제일 중요한 내용은 렉시컬(lexical) 환경에 변수가 선언되어있지 않다면, 상위 `scope`에서 해당 값을 찾고, 상위 `scope`에도 값이 없다면, 전역 객체에 값을 할당한다. 다음의 코드가 이를 반증하는데 다음 `a`값은 무엇일까? 정답은 3이다. 전역 변수에 `a`값이 없는데 왜 `3`이 할당되는지는 `scope chain`을 따라가면 되는데, `outer` 내부에 `a`가 `var, let, const`로 할당된것이 아니기 때문에 현재 `scope`에서는 `target`이 없다. 따라서 상위 단계의 `scope`를 탐색하게 되고, 전역 객체까지 나갔을 때도 값이 없다면 전역객체에 `a`값을 할당하게 된다. 

```javascript
function outer(){
	a = 3;
}

outer();
console.log(a)  // 3
```

### ❏ 실행 컨텍스트의 실행 과정
1. `Creation Phase`: 실행 컨텍스트의 뼈대가 만들어지는 단계이며, 변수는 선언만(undefined) 이루어지며, 실질적인 할당은 이루어 지지않는다. 함수는 `pointer`만 생성된다.
2. `Execution Phase`: 실행 컨텍스트의 실행 단계이며, 변수의 값이 할당되는 단계이다. 함수의 주소도 할당된다.

### ❏ 호이스팅
1. 변수 선언 / 함수 선언을 코드의 맨 위로 끌어 올려진 것 같은 현상
2. `var` 변수는 함수 내부에서만 호이스팅이 일어난다.(전역까지는 접근 불가)
3. `let`, `const`는 호이스팅에 의해 선언은 이루어지지만 초기화단계는 해당 코드에 도달했을 때 진행되기 때문에, 이전까지 일시적 사각지대(TDZ)에 빠지게 된다. (선언은 되어있지만 아직 초기화가 되지않아 변수에 담길 값을 위한 공간이 메모리에 할당되지 않은 상태) 따라서 변수를 마주한 코드부터 접근이 가능하다.

```js
// var
console.log(a)  // undefined
var a = 1;

// let
console.log(b)  // Cannot access 'b' before initialization
let b = 1;

// const
console.log(c)  // Cannot access 'c' before initialization
let c = 1;
```

### ❏ 자바스크립트 내장 객체
다음 <a href='https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects'>`MDN`</a>을 참고하자

```javascript
// 0 ~ 5사이의 난수 구하기
// random(): 0 <= x < 1
// 내가 원하는 최대값과 random을 곱하고 소수점을 떼면 0~최대값까지 난수가 생성된다.
console.log(Math.floor(Math.random() * 6));
```

### ❏ 함수 선언식, 함수 표현식, 화살표 함수
1. 함수 선언식: 평소에 `js`를 사용할 때 함수 선언하는 방법이다. 함수 이름을 생략할 수 없는 특징이 있다. 함수 선언식은 함수 선언문 이전에 호출할 수 있다.

```jsx
function add(a, b){
	return a+b;
}
```

2. 함수 표현식: 함수 이름을 생략할 수 있는데, 이를 익명 함수라고 한다. 만약, 함수이름을 선언한다면 함수 내부에서만 유효한 식별자이므로 함수 이름으로 함수를 호출할 수 없다. 함수 표현식으로 정의한 함수는 함수 표현식 이전에 호출할 수 없다. 함수의 생성시점이 다르기 때문이다.

```jsx
const add = function (a, b){
	return a+b;
}
```

3. 화살표 함수: `function`키워드 대신 화살표를 사용해 좀 더 간략한 방법으로 함수를 선언할 수 있다. 화살표 함수는 항상 익명 함수로 정의한다.

```jsx
// 기본 코드
const add = (a, b) => {return a+b};  

// 함수 몸체가 하나의 몸으로 구성된다면 함수 몸체를 감싸는 중괄호를 생략할 수 있다.
const add = (a, b) => a+b;

// 매개변수가 1개인 경우 소괄호를 생략할 수 있다.
const pow = n => n*n;
```

reference
1. <a href='https://www.aladin.co.kr/shop/UsedShop/wuseditemall.aspx?ItemId=251552545'>모던 자바스크립트 딥 다이브</a>

---
## 📍 14일차 11.12.금.(온라인 강의)
오늘은 `closure`, `arrow-function`, `spread operator`, `this` 등 자바스크립트 동작 원리에 대해서 배웠는데, `closure` 부분에서 막힌 부분이 조금 많았다. 아무래도 내가 지금까지 잘 사용하지 않았던 문법이어서 그런가보다. 자주자주 보고 익숙해져야겠다.

### ❏ 자바스크립트 함수가 실행되는 과정
1. JS의 코드가 없는 경우

```javascript
// 동작 순서
1. 실행환경(실행 컨텍스트)을 초기화한다.
2. scope는 코드가 현재 실행되는 환경, 맥락(context)을 의미한다.
3. this 포인터, 스코프에 저장된 변수들, 스코프 체인 등이 환경에 포함된다.
4. this 포인터의 경우, 글로벌 스코프에서는 window를 가리킨다.

// GEC에서 실행되는 context
5. this
6. 변수들(Variable Object)
7. Scope
```

2. JS의 코드가 있는 경우

```javascript
// 1. 함수가 실행되면, 함수 스코프에 따라 환경이 만들어진다.
// 2. this, 함수 스코프의 변수들, 그리고 스코프 체인이 형성된다.
// 3. 스코프 체인을 따라 글로벌 환경에 도달한다.

function myFunc(){
  let a = 10;
  let b = 20;
  function add(first, second){
    return first + second
  }
  return add(a, b);
}

myFunc()

// 4. 객체의 메서드의 경우, 메서드 환경의 this는 해당 객체를 가리키게 된다.
// 5. 하지만 this가 가리키는 것은 환경에 따라 변할 수 있다.
```

### ❏ 실행 컨텍스트

1. `JS` 동작원리를 파악하기위해 중요한 개념이다.
2. 자바스크립트 코드가 실행되는 환경
3. 코드에서 참조하는 변수, 객체(함수 포함), this 등에 대한 레퍼런스가 있다.
4. 실행 컨텍스트는 전역에서 시작해, 함수가 호출될 때 스택에 쌓이게 된다.
5. `JS` 가 실행될 때 전역실행컨텍스트(GEC)가 만들어진다.
6. 함수가 실행될 때 함수실행컨텍스트(FEC)가 만들어진다.

```javascript
let a = 10;
function f1(){
	let b = 20;
	function print(v){console.log(v)};
	function f2(){
		let c = 30;
		print(a+b+c);
	}
	f2();
}
f1();  // 60
```

```javascript
const o = {
name: "Kim",
  changeMyName: function (name) { this.name = name },
};

const o2 = {
  name: "Song",
};

function callFuncWithArg(f, arg) {
  f(arg);
}

o.changeMyName.bind(o2)("Sam");
console.log("1번 - ", o2.name);  // "Sam"

callFuncWithArg(o.changeMyName, "Daniel");  // "Kim"
console.log("2번 - ", o.name);

o.changeMyName("Sam"); 
console.log("3번 - ", o.name);  // "Sam"
```

### ❏ 함수가 호출되는 상황 4가지(`dynamic binding`)
1. 직접 호출: 함수를 직접 호출한다 (myfunc())
2. 메서드 호출: 객체의 메서드를 호출한다.(o.method())
3. 생성자 호출: 생성자 함수를 호출한다. (`const p = new Person()`)
4. 간접 호출: `call`, `apply` 등으로 함수를 간접 호출한다.(`f.call(null, obj)`)
5. 콜백함수(특정 동작 이후에 불려지는 함수), 다른 함수의 인자로 보내지는 함수 등

```javascript
// 직접 호출
function myFunc(){
  console.log("my func called");
}

// 메소드 호출
const o = {
  name: "AYW",
  printName: function(){
    console.log(this.name);
  }
}

o.printName()

// 생성자 호출
function Person(name){
  this.name = name;
  this.consoleName = function(){
    console.log(this.name);
  }
}

const p = new Person("AYW")
console.log(p)
p.consoleName()

setTimeout(p.consoleName.bind(p), 1000);  // AYW
```

### ❏ this가 가리키는 것
1. 함수는 다양한 상황에서 호출될 수 있다.
2. 함수의 호출 환경에 따라 `this` 는 동적으로 세팅된다.
3. `this` 가 환경에 따라 바뀌는 것을 `dynamic binding`이라고 한다.
4. `bind`, `apply`,`call` 등으로 `this` 를 가리키는 것을 조작할 수 있다.
5. 일반 함수와 화살표 함수의 `this` 차이
5-1. 화살표 함수로 `this` 호출 시 `global` 을 가리킨다.
5-2. 일반 함수로 `this` 호출 시 누가 호출 했는지에 따라 값이 동적으로 바뀐다.

```javascript
const o = {
  name: "TED",
  arrowFunc: () => { console.log(this) },
  generalFunc: function(){console.log(this)}
}

o.arrowFunc();  // global
o.generalFunc();  // { name: 'TED', arrowFunc: [Function: arrowFunc], generalFunc: [Function: generalFunc] }

setTimeout(o.arrowFunc, 1000);  // global
setTimeout(o.generalFunc, 1000);  // global
```

7. `setTimeout` 의 `this` 는 `global` 을 가리킨다.
8. `bind`, `apply`, `call` 등의 함수로 `this` 를 조작한다.
9. `setTimeout` 은 함수 호출과는 다른 콜백 호출이다.
10. `printName` 메서드는 `bind` 함수를 이용해 `this` 변수가 `o` 를 가리키도록 컨텍스트를 동적 바인딩한다.

```javascript
const o = {
  name: "TED",
  printName: function(){console.log("내 이름은" + this.name)},
}

o.printName();  // 내 이름은 TED
setTimeout(o.printName, 1000);  // 내 이름은 undefined
setTimeout(o.printName.bind(o), 1000);  // 내 이름은 TED
```

### ❏ 화살표 함수와 일반 함수의 this

1. 화살표 함수의 `this` 는 호출된 함수를 둘러싼 실행 컨텍스트를 가리킨다. (선언 당시의 `this` 값을 유지한다. `this` 값을 `bind` , `apply`, `call` 로 바꿀 수 없다.) `this` 가 정해지면 바꿀 수 없다. `setTimeout` 등 `this` 가 바뀌는 상황에서 유용하다.
2. 일반 함수의 `this` 는 새롭게 생성된 실행 컨텍스트를 가리킨다. (`this` 값을 `bind` , `apply`, `call` 로 바꿀 수 있다.), `this` 가 바뀌어야하는 경우는 일반함수를 사용한다.

```javascript
const o = {
  method(){
    console.log(this)
    let f1 = function(){console.log(`f1`, this)};  
    let f2 = () => console.log(`f2`, this)  
    f1();  // global
    f2();  // o
  }
};

o.method()  // o
```

```javascript
window.name = "TED";

const o = {name: "AYW"};
const arrow  = (prefix) => console.log(prefix + this.name);

arrow("Dr. ");  // Dr. TED
arrow.bind(o)(("Dr. "));  // Dr. TED
arrow.call(o, "Dr. ");  // Dr. TED
arrow.apply(o, ["Dr. "]);  // Dr. TED
```

### ❏ closure
1. 일급객체란? 다른 변수처럼 대상을 다룰 수 있는것. JS에서 함수는 일급 객체이다. JS에서 함수는 변수처럼 다룰 수 있다.
2. 클로저는 함수의 일급 객체 성질을 이용한다.
3. 함수가 생성될 때, 함수 내부에서 사용되는 변수들이 외부에 존재하는 경우 그 변수들은 함수의 스코프에 저장한다.
4. 함수와 함수가 사용하는 변수들을 저장한 공간을 클로저라 한다.

```javascript
function add(a, b){
	return a+b;
}

[1, 2, 3].reduce(add, 0);

(() => {
	console.log("익명 함수를 생성한다.")
})()

function outer(a){
	function inner(b){
		return a + b
	}
	return inner(10)
}

// 함수를 변수로 생성한다.
const Person = (name) => {
  const printName = () => console.log(name);
  return { printName }  // 함수를 리턴하며 closure를 생성한다.
}

const person = Person("ted");
person.printName()

function printName(name){
  console.log(name)
}

// 함수끼리 비교한다.
// ===의 경우, 변수가 같은 객체(함수)를 가리키는지 체크한다.
console.log(printName === person.printName)
```

```javascript
// 클로저 함수 예시
// card1과 card2와 별도의 메모리 공간에 저장된다.

function createCard(){
  let title = "";
  let content = "";

  function changeTitle(text) {title = text};
  function changeContent(text) {content = text};
  function print(){console.log(title), console.log(content)};

  return { changeTitle, changeContent, print };
}

const card1 = createCard();
card1.changeTitle("생일 카드")
card1.changeContent("생일 축하해");
card1.print()

const card2 = createCard();
card2.changeTitle("감사 카드")
card2.changeContent("감사합니다.");
card2.print()
```

### ❏ Rest, spread operator
1. 함수의 인자, 배열, 객체 중 나머지 값을 묶어 사용하도록 한다.
2. 함수의 인자 중 나머지를 가리킨다.
3. 배열의 나머지 인자를 가리킨다.
4. 객체의 나머지 필드를 가리킨다.
5. 함수인자 `...arr` 은, 인자들을 배열로 묶는다.

```javascript
// 인자로 들어왔을 때
function findMin(...arr){
	return rest.reduce((a, b) => a < b ? a : b)}
}

findMin(7, 3, 5, 2, 4, 1)  // 1

// 객체로 사용할 때
const o = {
  name: "TED",
  age: 23,
  job: "zzz"
}

const { name, ...rest } = o;
console.log(rest)  // { age: 23, job: 'zzz' }
```

---
## 📍 15일차 11.13.토.(온라인 강의)
오늘은 `JS`엔진, `JS` 코드 실행, `렉시컬 환경`, `Hoisting`, `globalThis` 등에 대해서 배웠다.

### ❏ JS 엔진
1. `JS` 엔진은 `JS` 코드를 읽어 실행하는 프로그램이다.
2. `JS` 코드는 `JS` 엔진을 통해 파싱되고 실행된다.
3. `Chrome` 브라우저의 경우 `V8` 엔진을 사용한다.
4. `node.js` 는 브라우저 외의 환경에서 `JS` 코드를 실행하도록 하는 프로그램이다.
5. `node.js` 는 여러 프로그램으로 구성되며, `JS` 코드를 읽는 프로그램으로 `V8`을 사용한다.
6. 브라우저 환경과 `node.js` 환경은 같은 `JS` 코드를 작성해도 다르게 동작할 수 있다.

### ❏ JS  코드 실행
1. JS 엔진은 코드 실행 전 실행 컨텍스트를 실행한다.
2. 실행 컨텍스트는 두 단계를 통해 생성된다.
3. 생성단계에서 변수를 초기화시킨다.
4. 실행단계에서 변수 값을 할당한다.

### ❏ 렉시컬 환경
1. 함수의 렉시컬 환경은, 함수가 사용하는 변수들을 둘러싼 환경을 의미한다.
2. 특정 변수의 값은 함수의 렉시컬 환경 내에서 찾을 수 있다.
3. 렉시컬 환경은 실행 컨텍스트 안에 정의된 `Variable Object` 로 이해할 수 있다.
4. 실행 컨텍스트 안에 해당 변수가 없다면, 엔진은 함수스코프 외부에서 해당 변수를 찾으려고 한다. 이것을 `scope chain` 이라 부른다. 

### ❏ 스코프 체인(scope chain)
`scope`는 식별자에 대한 유효범위다. 어떤 경계 `A`의 외부에서 선언한 변수는 `A`의 외부뿐 아니라 `A`의 내부에서도 접근이 가능하지만, `A`의 내부에서 선언한 변수는 오직 `A`의 내부에서만 접근할 수 있다. 이러한 `식별자의 유효범의`를 안에서부터 바깥으로 차례로 검색해나가는 것을 스코프체인이라고 부른다. 이때 `outerEnvironmentReference`는 현재 호출된 함수가 선언될 당시의 `L.E`를 참조하게되는데, 중요한 점은 과거 당시 `선언된 시점`이다. 다음 코드의 `foo()`와 `bar()`의 값은 1로 동일한데, 그 이유는 `function bar`가 선언된 시점의 `x`는 전역 변수인 `x`를 바라보게 된다. 즉, `this`처럼 함수를 어디서 호출했는지가 아니라 함수를 어디에서 정의했는지에 따라 상위 스코프를 결정한다. 함수가 호출된 위치는 상위 스코프 결정에 어떠한 영향도 주지 않는다. 즉, 함수의 상위 스코프는 언제나 자신이 정의된 스코프다. 함수 선언문으로 정의된 `bar` 함수는 전역에서 정의된 함수다. 그러므로 전역 코드가 실행되기 전에 먼저 평가되어 함수 객체를 생성한다. 이때 생성된 `bar` 함수 객체는 전역 스코프를 기억한다. 그리고 `bar` 함수가 호출되면 호출된 곳이 어디인지 관계없이 언제나 자신이 기억하고 있는 전역 스코프를 상위 스코프로 사용한다.

```javascript
var x = 1;

function foo(){
  var x = 10;
  bar();
}

function bar(){
  console.log(x);
}

foo();  // 1
bar();  // 1
```

### ❏ Hoisting
1. `JS`가 코드를 읽으면, 생성 단계에서 실행 컨텍스트를 생성한다.
2. `var` 변수는 저장 시 `undefined` 로 초기화 된다. `let` 과 `const` 는 초기화되지 않는다. (해당 코드를 읽고 나서부터 사용 가능하다.)
3. `var`, `let` 은 변수에 재할당이 가능하지만 `const` 는 재할당이 불가능하다.
4. `var` 는 함수 스코프, `let`, `const` 는 블록 스코프 변수이다.

```javascript
// Hoisting은 변수가 선언된 시점보다 앞에서 사용되는 현상이다.
// 이는 var 변수가 생성 단계에서 undefined로 초기화되는것이 원인이다.
// 함수는 생성단계에서 함수 전체가 저장되므로 뒤에서 선언되어도 호출이 가능하다.

console.log(callMe())  // undefined

var x = 10;

console.log(callMe())  // 10

function callMe(){
	return x;
}
```

```javascript
// let, const 변수는 생성 단계에서 초기화되지 않는다.
// 선언문 이전에 접근 시 Reference Error가 발생한다.
// 이 경계를 TDZ라고 한다.
// 따라서, let, const는 hoisting이 발생하지 않는다.
// 함수는 생성단계에서 값까지 할당하지만 let, const는 생성단계에서 해당 값 이전에 접근하려고 했기 때문에 TDZ에 의해 참조에러가 난다.

console.log(callMe())  // undefined

var x = 10;

console.log(callMe())  // 10

function callMe(){
	return x;
}
```

```javascript
// varFor에서 i는 varFor 함수 범위에 존재하는 변수이다.
// 따라서, setTimeout이 호출될 때, i는 for 블럭이 끝난 시점에 소멸하지 않는다.
// letFor에서 i는 for 블럭안에 존재하는 변수이다.
// 각 for block이 실행되고 i는 소멸한다. 다만, 이 경우 각 화살표 함수의 closure에 저장된다.

function varFor(){
  for(var i=0; i<3; i++){
    setTimeout(() => console.log(i))
  }
}

function letFor(){
  for(let i=0; i<3; i++){
    setTimeout(() => console.log(i))
  }
}

varFor()  // 3 3 3
letFor()  // 0 1 2
```

### ❏ GlobalThis
1. `globalThis`: 전역 객체를 지칭하는 변수이다.
2. 전역 객체는 환경에 다라 다르다.
3. 브라우저 환경은 `window`, `node` 환경은 `global` 객체를 지칭한다.
4. `globalThis` 는 환경별 차이를 통일하여 하나의 변수로 서로 다른 전역 객체를 가리키게 한다.

```javascript
// DOM document를 포함하는 창을 나타내는 객체
// 전역 스코프에 선언된 변수는 모두 window의 property가 된다.
// 현재 창의 정보를 얻거나, 창을 조작한다.
// globalThis는 브라우저 환경에서 window 객체와 같다.

const targetURL = "https://www.naver.com";
const windowSize = `height=${window.innerHeight}, width=${window.innerWidth}`;
window.open(targetURL, "target", windowSize)

// globalThis
const windowSize = `height=${globalThis.innerHeight}, width=${globalThis.innerWidth}`;
globalThis.open(targetURL, "target", windowSize)
```

### ❏ Document
1. 브라우저에 로드된 웹 페이지
2. 문서의 `title`, `URL` 등의 정보를 얻는다.
3. `element` 생성, 검색 등의 기능 제공

```js
function printDocumentInfo(){
	console.log(document.URL);
	console.log(document.title);
	console.log(document.querySelectorAll("*"));
}
```

4. `createElement`, `createTextNode` 는 동적으로 원소를 생성한다.

```js
function createTodoList(todos){
	return todos
			.map((todo) => {
				const li =
	document.createElement("li")
	li.appendChild(document.createTextNode(todo))
})
		return li
	})
		.reduce((ul, li) => {
			ul.appendChild(li)
			return ul
}, document.createElement("ul"))
}
```

### ❏ Number, NaN
1. `number` 원시타입을 감싸는 객체
2. 유의미한 상수값, 숫자를 변환하는 메서드 등을 제공한다.
3. `NaN`: Not a Number를 나타내는 객체
4. `isNaN()`: 전역 함수로, 입력값을 숫자로 변환했을 때 `NaN` 이 되는지를 검사

```js
// toFixed
function changeToUsd(krw){
	const rate = 1046;
	return (krw/rate).toFixed(2);
}

const krw = 100_000;
console.log(changeToUsd(krw));

// isNaN
function formatNumber(n){
	if (isNaN(n) return "0");
	return Number(n).toFixed(2);
}

formatNumber("12.345");  // 12.35
```

1. `math`: `BigInt` 타입과 호환되지 않고, `Number` 타입만을 인자로 다룬다.

```js
// bigInt
let bigN = 1000000000000n

// Math.max, Math.min
function getMaxDiff(nums){
	return Math.max(...nums) - Math.min(...nums);
}

getMaxDiff([-1, -4, -7, 11]);

// Math.random
function getRandomNumberInRange(min, max){
	return Math.floor(Math.random() * (max - min + 1)) + min;
}

Array.from({ length: 10 }).map(() => getRandomNumberInRange(50, 100))
```

### ❏ Date
1. 특정 시점의 날짜를 표시하기 위한 객체
2. 날짜와 관련된 작업을 하기 위한 여러 메서드를 포함한다.

```js
// Date.getDay()는 요일을 0(일요일)부터 6(토요일)로 구한다.
// 이 외에 년도, 월, 일, 시, 분, 초, 밀리초 등을 구할 수 있다.
// getMonth(), getDate(), getHour()...

function isWeekend(today){
	let day = today.getDay();
	return day === 0 || day === 6;
}

console.log(isWeekend(new Date("2021/11/13")))

// setDate()등의 메서드로 시간을 설정한다.
// 설정 시 월 변경 등의 시간 변환은 Date 객체가 처리한다.
// toDateString() 메서드는 특정 포맷의 문자열을 반환한다.

function addDays(date, days){
	date.setDate(date.getDate() + days)
	return date.toDateString()
}

addDays(new Date("2021/9/22"), 100)  // Fri Dec 31 2021

// getTime() 메서드는 시간을 밀리초 단위로 반환한다.
// 이때 밀리초는 1970.1.1 시점부터 흐른 시간이다.
// fromNow는 주어진 시간이 현재로부터 며칠이나 흘렀는지를 계산한다
function timeDiff(date1, date2){
	return date2.getTime() - date1.getTime()
}

let dayTime = 60 * 24 * 60 * 1000
function fromNow(date){
	let diff = timeDiff(date, newDate())
	return `${Math.floor(diff / dayTime)} days ago...`
}

fromNow(new Date("2021/11/13"))
```

### ❏ String, JSON
1. 문자열 원시 타입의 래퍼객체
2. 문자열을 조작하기 위한 여러 메서드를 포함한다.
3. JSON - JSON 객체와 관련된 메서드를 담은 객체

```js
// toUserList는 이름의 배열을 받아 리스트 태그 목록의 문자열을 계산한다.
function toUserList(users) {
	return users
			.fileter((user) =>
	!user.includes("Admin"))
			.map((user) => 
	user.trim().toUpperCase())
			.map((user) => `<li>${user}</li>`)
			.join("")	
}

console.log(toUserList(["TED", "AYW", "AYJ"]))
```

```js
// JSON.stringify는 주어진 객체를 JSON 문자열로 만든다.
JSON.stringify({name: "TED", age: 27})  // {"name":"TED","age":27}

// JSON.parse()는 주어진 JSON 문자열을 JS 객체로 만든다.
JSON.parse('{"name":"TED","age":27}')  // { name: 'TED', age: 27 }
```

reference 
1. <a href='https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=206513031'>코어 자바스크립트</a>
2. <a href='https://www.aladin.co.kr/shop/UsedShop/wuseditemall.aspx?ItemId=251552545'>모던 자바스크립트 딥 다이브</a>

---
## 📍 16일차 11.16.화.(실시간 강의)
어느덧 엘리스를 시작한지 4주차가 되는 날이다. 4개월의 전체 과정 중 1/4인 약 25%를 달려온 셈인데, 생각보다 시간이 빨리가서 놀랐다. 남은 3개월도 꾸준하게 배운 내용을 기록하여 미래의 기본이 탄탄한 프론트엔드가 될 나의 밑바탕이 되어보자. 오늘은 `동기 / 비동기`, `콜백 함수`, `promise`에 대해서 배웠다. 항상 콜백함수를 배울 때는 `JS` 엔진의 동작방식이랑 같이 배우게 되는데, 잘 알아둬야하는 이유는 기술 면접에서 물어보기 때문이다. 실제로 면접을 볼 때마다 `call back`과 `promise` 함수의 차이점에 대한 질문을 받았다. 그때는 뭉뚱그려 대답했는데, 이번 기회를 통해 차이점을 확실하게 알아야겠다.

### ❏ 동기 / 비동기
1. 동기(synchronous): 동기적이다라는 표현은 일정한 순서에 의해 진행된다는 말인데, 보통 `python`과 같은 언어가 동기적으로 작동한다고 할 수 있다. `JS`도 마찬가지로 동기언어인데, 자바스크립트 엔진은 한 번에 하나의 태스트만 실행할 수 있는 싱글 스레드 방식이기 때문이다. 때문에, 시간이 걸리는 기능은 해당 기능이 끝날 때까지 기다려야하는 블로킹 현상이 발생하는데, 이는 동기처리 방식의 대표적인 예시이다. 장점으로는 실행 순서가 보장되어있다.
2. 비동기(Asynchronous): 동기처리 방식과는 반대로, 다음 태스크를 블로킹하지 않고 곧바로 실행하는 것을 비동기라고 하는데, 비동기 처리 방식은 현재 실행 중인 태스크가 종료되지 않은 상태라 해도, 다음 태스크를 곧바로 실행하므로 블로킹이 발생하지 않는다는 장점이 있지만, 태스크의 실행순서가 보장받지 않는 단점이 있다. `JS`에서 `setTimeout`, `setInterval`, `HTTP 요청`, `event handler`는 비동기 처리방식으로 동작한다. 

```javascript
// 동기 코드: 앞선 task가 종료할 때까지 나머지 task는 대기한다.
let initTime = Date.now();
let count = 0;

while (true) {
    let currentTime = Date.now();
    if (currentTime - initTime > 3000) {
        count++;
        break;
    }
}

function foo(){
  console.log('foo')
}

function bar(){
  console.log('bar')
}

foo();
bar();

// 비동기 코드: 동시에 실행되는 특징을 갖고 있다.
setTimeout(() => {
        count++;
}, 3000);

function foo(){
  console.log('foo')
}

function bar(){
  console.log('bar')
}

foo();
bar();
```

### ❏ 콜백함수(call back)
1. 콜백함수란 다른 함수의 인자로써 사용되는 함수를 말한다.
2. 우리가 JS에서 비동기 처리를 수행할 때는 콜백함수를 사용하는데, 콜백함수의 단점은 여러개의 콜백 패턴을 사용할 때 가독성이 떨어지고, 비동기 처리 중 발생한 예외 처리가 곤란하며, 여러개의 비동기 처리를 한 번에 처리할 때 한계가 있다. 

```javascript
// 1초가 지나고 undefined가 출력된다.
function findUser(id){
	let user;

	setTimeout(function (){
		console.log("1초 기다림")
		user = {
			id: id
		}
})

	return user
}

let user = findUser(1);

// 콜백으로 넘겨주기: 1초가 지나고 user에 값이 할당된다.
// 단점: 비동기를 또 넘겨주고 싶을 떄는 콜백지옥에 빠진다.
function findUser(id, callbackFunc){
	let user;
	setTimeout(function(){
		console.log("1초 기다림")
		user = {
			id: id
		};

		callbackFunc();
	}, 5000);
	return user;
}

findUser(1, function(user){
	console.log("user:", user)
})

// 이벤트 핸들링
addEventListener("click", function(){console.log("HI")})
```

### ❏ promise
1. ES6에서 비동기 처리를 위한 또 다른 패턴으로 프로미스를 도입했는데, 프로미스는 전통적인 콜백 패턴이 가진 단점(비동기처리를 연속적으로 진행할 경우 가독성이 떨어지는 문제, 비동기처리 중 예외 발생시 예외 처리의 어려움, 여러개의 비동기를 한번에 처리하기 어려움)을 보완하며 비동기 처리 시점을 명확하게 표현할 수 있다는 장점이 있다.
2. 프로미스는 비동기 방식의 코드를 동기 방식으로 동작하게 끔 만들어주는 장점이 있다. `promise` 객체는 3가지의 상태정보를 갖는데, `pending(비동기 처리가 수행되지 않은 상태) -> 프로미스가 생성된 직후 기본 상태`, `fulfilled(비동기 처리가 수행된 상태(성공)) -> resolve 함수 호출`, `rejected(비동기 처리가 수행된 상태(실패)) -> reject 함수 호출` 여기서 `fulfilled` 혹은 `rejected` 상태를 `settled` 상태라고 한다. `settled` 상태는 `fulfilled` 또는 `rejected` 상태와 상관없이 `pending`이 아닌 상태로 비동기 처리가 수행된 상태를 말한다. 프로미스는 `pending` 상태에서 `settled` 상태로 변화할 수 있지만, `settled` 상태에서 `pending` 상태로 변화할 수 없다.
3. `promise.prototype.then`: `then` 메서드는 두 개의 콜백 함수를 인수로 전달받는다. 즉, 첫 번째 콜백 함수는 비동기 처리가 성공했을 때 호출되는 성공 처리 콜백함수이며, 두 번째 콜백함수는 비동기 처리가 실패했을 때 호출되는 실패 처리 콜백 함수다. `reject`를 사용하지 않더라도 `then`으로 `promise`의 성공과 실패의 결과 값을 모두 받을 수 있는데 이는 `then`메소드에 두번 째 콜백 함수를 전달하는 것보다 `catch` 메소드를 사용하는 것이 가독성이 좋고 명확하기 때문에 별로 추천하지 않는다.
4. `promise.prototype.catch`: `catch` 메서드는 한 개의 콜백 함수를 인수로 전달받는다. `catch` 메서드의 콜백 함수는 프로미스가 `rejected` 상태인 경우만 호출된다. `then` 메소드와 마찬가지로 언제나 프로미스를 반환한다.
5. `promise.prototype.finally`: `finally` 메소드는 한 개의 콜백 함수를 인수로 전달받는다. `finally` 메서드의 콜백 함수는 프로미스의 성공(`fulfilled`) 또는 실패(`rejected`)와 상관없이 무조건 한 번 호출된다. `finally` 메서드는 프로미스의 상태와 상관없이 공통적으로 수행해야 할 처리 내용이 있을 때 유용하다. `finally` 메서드도 `then/catch` 메서드와 마찬가지로 언제나 프로미스를 반환한다.

지금까지 `동기 / 비동기`, `callBack`, `promise`를 짧게 알아봤는데, 결론적으로 `callBack`과 `promise`의 차이점은 `callback`으로 비동기 처리를 하려면 `callback` 함수 안에서만 처리해야하는데, `promise`는 비동기의 값이 `promise` 객체에 저장되기 때문에 함수 밖에서 처리할 수 있고, `promise`의 장점은 `callback`의 단점인 콜백 지옥, 예외 처리, 한번에 여러번 비동기 처리를 해결 할 수 있다는 장점이 있다.

reference 
1. <a href='https://blog.toycrane.xyz/promise-%EC%A0%95%EB%A7%90-%EC%89%BD%EA%B2%8C-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-a74b6e3c6722'>toy crane</a>
2. <a href='https://www.aladin.co.kr/shop/UsedShop/wuseditemall.aspx?ItemId=251552545'>모던 자바스크립트 딥 다이브</a>

---
## 📍 17일차 11.17.수.(온라인 강의)
오늘은 <a href='https://ywtechit.tistory.com/373'>어제</a> 배웠던 동기 / `비동기`, `콜백함수`, `promise`에 대해 더 자세하게 배웠다. `promise`는 3~4개월 전인가? 토스 코딩테스트에서 비동기적으로 `api` 호출하는 테스트가 나왔었는데, 그때 문제의 의도를 정확하게 파악하지 못해서 틀렸던 경험이 있었다. 프론트엔드와 비동기는 뗄레야 뗄 수 없는 관계이므로 잘 기억하자.

### ❏ 자바스크립트 제어 흐름
1. 자바스크립트는 다른 멀티스레드 프로그래밍 언어`(JAVA, C++)`와 다른 방식으로 비동기 동작을 처리한다.
2. 처음 자바스크립트를 접하는 경우, 동작에 대한 정확한 이해가 없으면 코드의 흐름을 따라가기 어렵다.
3. 자바스크립트 내부의 비동기 동작을 이해하기 위해서는 이벤트 루프 등의 개념을 알아야만 한다.
4. JS 엔진은 하나의 메인 스레드로 구성된다.
5. 메인 스레드는 코드를 읽어 한 줄 씩 실행한다.
6. 브라우저 환경에서는 유저 이벤트를 처리하고 화면을 그린다.

### ❏ 동기적 제어 흐름
1. 동기적 제어 흐름은 현재 실행중인 코드가 종료되기 전까지 다음 라인의 코드를 실행하지 않는 것을 의미한다.
2. 분기문, 반복문, 함수 호출은 동기적으로 실행된다.
3. 코드의 흐름과 실제 제어 흐름이 동일하다.
4. 싱글 스레드 환경에서 메인 스레드를 긴 시간 점유하면, 프로그램을 멈추게 한다.

### ❏ 비동기적 제어 흐름
1. 비동기적 제어 흐름은 현재 실행중인 코드가 종료되기 전에 다음 라인의 코드를 실행하는 것을 의미한다.
2. 프로미스 ,콜백 함수 등은 비동기적으로 실행된다.
3. 코드 흐름과 실제 제어 흐름이 다르다.
4. 비동기 작업을 기다리는 동안 메인 스레드는 다른 작업을 처리한다.

### ❏ 이벤트 루프
1. JS 엔진은 비동기 처리를 제공하지 않는다.
2. 대신, 비동기 코드는 정해진 API(`setTimeout`, `XMLHttpRequest`, `fetch`)를 제공하여 활용할 수 있다. 
3. `node.js` 의 경우 파일 처리 API, 암호화 API 등을 제공한다.

```js
// 타이머 비동기 처리
setTimeout(() => console.log("타이머 끝"), 1000);
setInterval(() => console.log("인터벌 타이머"), 1000);

// 네트워크 처리
fetch("https://google.com")
		.then(() => console.log("네트워크 요청 성공"))
		.catch(() => console.log("네트워크 요청 실패"))
```

4. 비동기 코드를 처리하는 모듈은 JS 엔진 외부에 있다.
5. `event queue`, `task queue`, `job queue` 등으로 구성된다.
6. API 모듈은 비동기 요청을 처리 후 태스크 큐에 콜백 함수를 넣는다.
7. JS 엔진은 콜 스택이 비워지면, `event Loop`에서 `task queue`의 콜백 함수를 `call stack`으로 `push`한다.
8. `call stack`에 있는 콜백 함수가 실행된다.

```js
// 비동기 처리가 끝나면 콜백 함수를 task queue로 밀어 넣는다.
request("user-data", (userData) => {
	console.log("userData 로드")
	saveUsers(userData)
})

console.log("DOM 변경");
console.log("유저 변경");
```

### ❏ Promise
1. 비동기 API 중 하나이다.
2. 태스크 큐가 아닌 잡 큐(`Job queue` 혹은 `Microtask queue`)를 사용한다.
3. 잡 큐는 태스크 큐보다 우선순위가 높다.

```js
setTimeout(() => {
  console.log("타임아웃1")
}, 0);

Promise.resolve().then(() => console.log("프로미스 1"));

setTimeout(() => {
  console.log("타임아웃2")
}, 0);

Promise.resolve().then(() => console.log("프로미스 2"));

👉🏽 프로미스 1 프로미스 2 타임아웃1 타임아웃2
```

4. 비동기 작업을 표현하는 자바스크립트 객체
5. 비동기 작업의 진행, 성공, 실패 상태를 표현한다.(new Promise(resolve, reject), fetch(promise 반환))
6. 비동기 처리의 순서를 표현할 수 있다.
7. `then`, `catch`, `finally`, `then(cb1, bc2)` 로 `cb1` 자리에 성공, `cb2` 자리에 실패 메서드를 인자로 넘길 수 있다.
8. `promise method chain`: `then / catch` 메서드가 또 다른 `promise` 를 리턴하여, 비동기 코드에 순서를 부여한다. 동일한 객체에 메서드를 연결할 수 있는 것을 체이닝이라고 한다. 함수를 호출한 주체가 함수를 끝낸 뒤 자기 자신을 리턴하도록 하여 구현한다. (함수의 끝에 `return this`가 생략되어있기 때문에 가능하다.), 비동기 코드의 순서를 쉽게 부여 가능하다.

```js
promise
    .then((data) => {
        return fetchUser(data);
    })
    .then((user) => {
        console.log("user : ", user);
    })
    .catch((e) => {
        console.log("실패 : ", e);
    });
```

9. `Promise.resolve(10).then(console.log)` : 성공한 `Promise` 를 바로 반환한다. 인위적으로 `Promise` 메서드 체인을 만들 수 있다. 비동기 코드로 진행해야 하는 상황 등에 유용하게 사용할 수 있다.
10. `Promise.reject("Error").then(console.log)`: 실패한 `Promise` 를 바로 반환한다.

```js
Promise.resolve(10).then(() => console.log("성공"))
👉🏽 성공

Promise.reject(new Error("에러!")).then(() => console.log("실패"))
👉🏽 (node:24270) UnhandledPromiseRejectionWarning: Error: 에러!
```

11. `promise.all`: 모든 `promise` 가 `settled` 될 때까지 기다린다. 만약, `promise` 의 배열을 받아 모두 성공하면 각 `promise` 의 `resolved` 값을 배열로 반환한다. 하나의 `promise` 라도 실패하면 가장 먼저 실패한 `promise` 의 실패 이유를 반환한다.

```js
Promise.all([
  promise1,
  promise2,
  promise3,
])
  .then((values) => {
    console.log("모두 성공", values)
  })
  .catch((e) => {
    console.log("하나라도 실패", values)
  })
```

12. promise를 리턴하는 값이 같으면 `then` 을 생략할 수 있다

```jsx
// 2개의 API에 모두 then을 사용한 방식
promise
	.then((item) => getUserNameById(item.id))
	.then((id) => id)
  .catch(e => e.message);

// 2개의 API 중 한개만 then을 사용한 방식
promise
	.then((item) => getUserNameById(item.id))
  .catch(e => e.message);
```

---
## 📍 18일차 11.18.목.(실시간 강의)
오늘은 실시간 강의로 `Ajax`, `promise`, `async / await`, `SPA` 에 대해 배웠다. 

### ❏ SPA 만들기
1. SPA로 구현하려면 경로로 접속할 때 같은 파일을 내려줘야 한다.
2. `html` 파일은 웹 서버에서 보관하고 `html` 해석은 웹 브라우저에서 한다. `html` 파일을 가공해서 고객들에게 보여주는 행위를 `client side tech, 혹은 front end` 라고 한다.
3. `header`: 서버에서 클라이언트에게 전달하는 정보
4. `fetch`를 사용하면 `JSON` 형태의 내용이 온다.
5. JS에서 객체를 표현하는 방법을 참고해서 만든 data spec
6. `JSON.parse`: JSON으로 넘어온 데이터를 JS 객체 형태로 바꾼다.
7. `Ajax`: `JS`를 사용하여 브라우저가 서버에게 비동기 방식으로 데이터를 요청하고, 서버가 응답한 데이터를 수신하여 웹페이지를 동적으로 갱신하는 프로그래밍 방식
8. `XMLHttpRequest` 는 크로스브라우징을 고려해야한다. 지금보니까 `fetch`도 꽤나 안되는 브라우저들이 있었다.(`Edge 12-13`, `IE`, `Opera Mini`)
9. `fetch`:  `fetch(url).then(type => type.json())` : `promise`를 `json`타입으로 바꿔준다.
10. `XMLHttpRequest`을 `fetch` 버전으로 바꿔보기

```javascript
// XMLHttpRequest로 JSON 객체 가져오기
function name() {
    var request = new XMLHttpRequest();
    request.open("GET", "https://gorest.co.in/public/v1/users", false); // `false` makes the request synchronous
    request.send(null);

    if (request.status === 200) {
        let text = request.responseText;
        let obj = JSON.parse(text);
        console.log("obj", obj.data[0].name);
        document.querySelector("#name").value = obj.data[0].name;
    } else if (request.status === 200) {
    }
}
```

```javascript
// 타입을 json으로 결정한다
1. let json = fetch("https://gorest.co.in/public/v1/users").then(type => type.json())

👉🏽 Promise {<fulfilled>: {…}}
[[Prototype]]: Promise
[[PromiseState]]: "fulfilled"
[[PromiseResult]]: Object

// 타입을 처리한다
json.then(res => console.log(res))
👉🏽 {meta: {…}, data: Array(20)}
```

### ❏ JSON
1. 데이터를 주고받을 때 사용하기 위해 고안된 데이터 형태
2. `get` 방식은 `data` 를 가져오기
3. 서버로 값을 보낼 때는 `JSON` 형태로 보내고, POST 할 때는 `headers` 설정과  `JSONstringify` 를 사용하기
4. 짝 프로그래밍

```javascript
fetch('/topics', {
    method:'POST', 
    body:JSON.stringify({title:'js', body:'js is ..'}), 
    headers: {
        'Content-Type': 'application/json'
    }})
```

### ❏ async / await
1. `promise` 코드에 `async - await` 문법을 사용하면 비동기적인 코드를 동기적으로 관리할 수 있다.
2. promise로 반환한 객체 앞에 `await` 를 붙이면 비동기적인 동작을 끝낼때까지 기다린다.
3. `await` 는 전역적으로 사용하는 것이 아니라 `async`함수 내에서만 사용할 수 있다.
4. 상황에따라 `promise`, `async` 를 맞춰서 사용하면 된다.
5. `async` 문법은 `promise` 를 리턴한다.
6. `async:`함수 내에서 비동기적으로 실행되면 비동기가 끝나면 다음 비동기가 실행된다

```javascript
// async - await
async function asyncFunc() {
    return "elice";
}

// promise
function promiseFunc() {
    return new Promise((resolve) => resolve("elice"));
}

console.log(asyncFunc());
👉🏽 Promise { 'elice' }

// 인자와 return 값이 인자 한개면 생략할 수 있다.
console.log(asyncFunc().then(console.log));


console.log(promiseFunc());
👉🏽 Promise { 'elice' }
```

```javascript
//async, await으로 변환하는 방법

// 1. Promise 대신 async로 비동기 처리해 'elice'를 반환하도록 fetchUser 함수를 수정하세요.
async function fetchUser() {
    return 'elice';
}

const user = fetchUser();
user.then((res)=>console.log(res));

// 2. delay 함수를 이용해 getCoffee와 getTea 함수를 작성하세요.
function delay(ms) {
    return new Promise(resolve => setTimeout(resolve, ms));
}

async function getCoffee() {
    await delay(1000);
    return 'coffee';
}

async function getTea() {
    await delay(1000);
    return 'tea';
}

// 3. 위 두 개의 함수를 사용해서 coffee와 tea를 한번에 반환합니다.
async function getDrinks() 
{
    const coffee = await getCoffee();
    const tea = await getTea();
    return ${coffee} and ${tea};
}

getDrinks().then((res)=>{console.log(res)});
```

### ❏ REST API
1. 이고잉님의 `REST API`에 관한 짧은 <a href='https://www.youtube.com/watch?v=PmY3dWcCxXI'>영상</a> 강의 보기
2. REST: HTTP를 기반으로 클라이언트에서 서버로 연결할 때 정해진 아키텍쳐에 따라 접근하는 방식
3. RESTAPI: REST를 기반으로 서비스 API를 구현한 것

---
## 📍 19일차 11.19.금.(온라인 강의)
오늘은 `async - await`, `error처리`, `HTTP`, `REST API`에 대해서 배웠다.

### ❏ async / await 문법
1. `Promise` 를 활용한 비동기 코드를 간결하게 작성하는 문법
2. `async / await` 문법으로 비동기 코드를 동기 코드처럼 간결하게 작성할 수 있다.
3. `async` 함수와 `await` 키워드를 이용한다.
4. `await` 키워드는 반드시 `async` 함수 안에서만 사용해야 한다.
5. `async` 로 선언된 함수는 반드시 `Promise` 를 리턴한다.
6. `async` 함수는 `function` 키워드 앞에 `async` 를 붙여 만든다
7. `async` 함수 내부에서 `await` 키워드를 사용한다.
8. `fetchData`, `fetchUser`는 `Promise` 를 리턴하는 함수이다.
9. `then method chain` 시 `then` 을 2번 이상 사용하면 순차적으로 실행된다. 첫번째 `then`을 기다렸다가 완료되면 다음 `then` 으로 이어진다. `async` 도 마찬가지로 `await`가 여러개 있을 때 순차적으로 실행된다.
10. `await` 키워드는, `then` 메서드 체인을 연결한것처럼 순서대로 동작한다.
11. 비동기 코드에 쉽게 순서를 부여한다.

```js
// async 함수
async function asyncFunc1(){
    let data = await fetchData()
    let user = await fetchUser(data)
    return user
}

// await 키워드 실행 순서
async function asyncFunc2(){
	let data1 = await fetchData1()
	let data2 = await fetchData2(data1)
	let data3 = await fetchData(data2)
	return data3;
}

function promiseFunc(){
	return fetchData1()
			.then(fetchData2)
			.then(fetchData3)
}
```

12. `Promise` 를 리턴하는 함수의 경우, 에러가 발생하면 `catch` 메서드를 이용하여 에러를 처리한다.
13. `catch` 메서드를 사용하지 않는다면 `async` 함수에서 `try-catch` 구문을 이용하여 에러를 처리한다.
14. `try` 구절안에 `await` 가 2개 이상 있을 때 `catch` 문에 해당 `error` 가 들어간다. `error` 처리를 세분화 하고 싶으면 한 `try` 구절에 `await` 를 1개씩만 담자.

```js
// promise error handling
function fetchData1(){
	return request()
			.then(response => response.requestData)
			.catch(error => // error)
}

// async - await error handling
async function asyncFunc(){
	try{
		let data1 = await fetchData1()
		return fetchData2(data1)
	} catch (e){
		console.log("error: ", e)
	}
}
```

15. async 함수는 동기적으로 보이지만 비동기적으로 실행됩니다. 단, 내부에서 `await` 키워드가 쓰이지 않았을 경우엔 `Promise.resolve()` 로 처리됩니다.
16. await 키워드는 프로미스를 리턴하지 않는 함수라도 사용할 수 있습니다. 단 이 경우 리턴한 데이터는 `Promise.resolve()`로 감싸집니다.

### ❏ HTTP(HyperText Transfer Protocol)
1. `Web` 에서 서버와 클라이언트 간의 통신하는 방법을 정한 것.
2. 클라이언트는 웹 브라우저 등 서버로 요청을 보내는 대상
3. 서버는 클라이언트가 요청을 보내기 전까지 대응하지 않음
4. 서버와 클라이언트 사이에는 무수히 많은 요소가 존재
5. `HTTP` 는 이런 존재들 사이의 통신 방법을 규정
6. 규약을 통해 통신하지 않으면 복잡해지고 혼란스럽게 된다.
7. `HTTP Message`: 서버 주소, 요청 메서드(POST), 상태 코드(200, 404), `target path`, 헤더 정보, 바디 정보 등이 포함된다. 요청 메시지와 응답 메시지의 모양이 다르다. `HTTP/1.1` 메시지는 사람이 읽을 수 있다.
8. `HTTP header`: 콘텐츠 관련 정보(`content-type: json...`), 인증 관련 정보(`Authorization`), 쿠키 정보(헤더에 들어간다. 가벼운 정보 등), 캐시(페이지 조회정보를 클라이언트에 내릴 때 일정시간 내에는 동일한 페이지를 그대로 사용하는 방법 등...) 관련정보 등 서버과 클라이언트 통신 시 필요한 정보를 담는다. 클라이언트 요청 시, 서버 응답 시 모두 헤더에 정보를 담을 수 있다.
9. `HTTP status` : `HTTP`요청 시, 클라이언트는 요청의 결과에 대한 상태 정보를 얻는다. `200`, `400`, `500` 등 숫자 코드와, `OK NOT FOUND` 등의 텍스트로 이루어진다. 코드를 이용해 각 결과에 해당하는 행위를 할 수 있다.
10. `요청 메서드`: 클라이언트에서 서버로 요청에 의미를 부여할 때 사용하는 명령어(`GET`, `POST`, `PUT`, `PATCH`, `DELETE`)

### ❏ REST API(Representational State Transfer API)
1. HTTP를 이용하여 클라이언트가 서버의 리소스에 접근하는 방식을 규정한 아키텍쳐고 `REST API` 는 `REST` 를 기반으로 서비스 `API` 를 규정한 것
2. API는 사용자가 특정 기능을 사용할 수 있도록 제공하는 함수
3. `REST API` 의 요청 메소드에 응하는 서버API와 클라이언트 간 통신의 구조가 지켜야 할 좋은 방법을 명시한 것이다.
4. 요청 메서드의 의미, URI설계, 클라이언트의 상태에 대한 동작 등을 정의한다.
5. REST API 요청 메서드: GET - 리소스 정보를 얻음, POST  - 리소스를 생성, PUT - 리소르르 생성하거나 업데이트 DELETE - 리소스를 제거

### ❏ Fetch API
1. `HTTP` 를 활용할 수있는 `API` 
2. 기존 `XMLHTTPRequest` 를 대체하는 `HTTP` 요청 `API` (두 함수의 큰 차이점은 `Promise` 리턴 여부)
3. `ES6` 에 추가된 `Promise` 를 리턴하도록 정의 됨
4. 네트워크 요청 성공 시, `Promise` 는 `resolve` 
5. 네트워크 요청 실패 시, `Promise` 는 `reject`
6. `response.` 객체는 결과에 대한 다양한 정보를 담는다.
7. `response.ok` : `200 <= HTTP status code <= 299` : true, 그 외 `false`
8. `response.status`: `HTTP status code` 를 담는다.
9. `response.url` : 요청한 `URL` 정보를 담는다
10.  response.json(): `body` 정보를 `json` 으로 만드는 `Promise` 를 반환한다.
11. `body` 값은 `json()` 값을 `resolve` 해서 나온 값을 `then` 처리를 해줘야 사용가능하다. `json()` 을 한번만 사용하면 `promise` 를 사용하는 꼴이된다.
12. `POST`: `fetch(url, options)` 로 `fetch` 메서드 옵션을 넣는다. `method` 필드로 여러 요청 메서드를 활용한다. `headers`, `body` 필드를 활용해 서버에 추가 정보를 보낸다.

```js
// response 객체 살펴보기
.fetch(URL)
	.then(response => {
		response.ok
		response.status
		response.statusText
		response.url
		response.bodyUsed
	})

// response header
.fetch("https://randomuser.me/api/").then(response => {
    for(let [k,v] of response.header){
        console.log(k,v)
    }}
);

// response body
.fetch(URL)
	.then(response => response.json()
	.then(console.log)

// POST 요청
fetch(serverURL, {
	method: "post",  // method 넣기
	headers: {
			'Content-Type': 'application/json; charset=utf-8',
	Authentication: 'mysecret'
	},
	body: JSON.stringify(formData)
})
	.then(res => res.json())
	.then(console.log)
```

---
## 📍 20일차 11.20.토.(온라인 강의)
오늘은 `JS`기본 내장 라이브러리인 `fetch`와 `HTTP` 비동기 외부 라이브러리인 `Axios`와의 차이점, `API` 그리고 `HTTP methods`에 대해서 배웠다. 본론으로 들어가기 전 `Window`는 `DOM document`를 포함하는 창을 나타내는 창을 말하고, `document`는 브라우저에 로드된 웹 페이지를 나타내는 객체이다. 쉽게말해 `window`는 브라우저 전체를, `document`는 브라우저 내부의 화면을 말한다.

### ❏ Axios
1. `Ajax`는 비동기 `JS`란 의미로 `Asynchronous JavaScript and XML`의 약자입니다. `Ajax`는 브라우저가 가지고 있는 `XMLHttpRequest` 객체를 이용하여 화면 전체를 새로고침하지 않고 변경된 일부 데이터만 로드하는 비동기 처리가 가능합니다. `Axios`는 `Ajax`와 유사하며, `API`를 이용한 통신을 할 때 주로 사용합니다.
2. `Axios`는 웹 브라우저와 `Node.js`를 위한 `HTTP` 비동기 통신 라이브러리입니다. 쉽게 말해 백엔드와 프론트엔드 간 통신을 쉽게 하기 위해 사용되는 것으로, `Ajax`처럼 사용되는 것입니다. 비동기 통신 라이브러리를 사용하지 않으면 모든 코드가 순차적으로 처리되어야 하므로 코드의 순서를 신경 써서 작성해야 합니다. 코드 작성이 매우 복잡해지며, 따라서 비동기 통신을 쉽게 해주는 `Axios`나 `Ajax`같은 것이 자주 사용되는 것입니다.

### ❏ Axios vs Fetch
1. 둘 다 `HTTP` 요청을 처리하기 위한 `JS` 라이브러리지만 몇 가지 차이점이 존재합니다.
2. `Fetch`의 경우 `JS`에 내장되어있기 때문에 별도의 `import`나 설치가 필요하지 않습니다. 하지만, `Axios`의 경우 설치 과정이 필요합니다.
3. `Fetch`는 `IE`에서 사용이 불가하고 `Edge` 14버전 이상부터 사용이 가능합니다.(<a href='https://caniuse.com/?search=fetch'>caniuse</a>) 반면, `Axios`는 `Fetch`보다 많은 브라우저에서 지원하고 있어 크로스 브라우징이 더 뛰어납니다.
4. `Fetch`에서 지원하지 않는 `JSON`자동 변환, 응답 시간 초과 설정 기능 등을 `Axios`에서 지원해줍니다.
5. 무조건 `Axios`를 사용하기보다는 자신의 개발 상황에 맞는 라이브러리를 선택해야 합니다.

### ❏ API
1. 운영 체제나 프로그래밍 언어가 제공하는 기능을 제어할 수 있게 만든 <a href='https://ko.wikipedia.org/wiki/%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4_(%EC%BB%B4%ED%93%A8%ED%8C%85'>인터페이스</a>를 말합니다.
2. 만약 여러분이 밥을 먹기 위해 식당을 갔다고 해봅시다. 손님인 여러분은 요리사에게 음식 주문을 해야 밥을 먹을 수 있습니다. 하지만 직접 요리사에게 말하지는 않죠. 일반적인 경우 점원을 통해 주문을 할 텐데요. 이때 점원 역할이 바로 API라고 생각하시면 됩니다. 즉, 프로그램과 프로그램을 연결해 주는 다리 역할을 하는 것이 API입니다.
3. 나 자신이 URL을 통해 누군가에게 해당 정보를 **요청하면,** 요청한 정보를 누군가가 나에게 다시 **전달해줍니다.**이러한 규칙을 HTTP라고 부릅니다.
4. 요청 받은 데이터를 가져오는 것은 웹 서버의 역할이며 HTTP는 바로 그 클라이언트와 서버 간의 규칙입니다. 이때, 클라이언트의 요청을 `HTTP Request`, 서버의 응답을 `HTTP Response`라고 합니다.
  
![](https://images.velog.io/images/abcd8637/post/392e05c2-4c10-438a-82db-301022524773/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-11-20%2007.15.58.png)

5. `200 <= HTTP status code <= 299` : `true`, 그 외 `false`
6. `CRUD`는 `Create`, `Read`, `Update`, `Delete`의 제일 앞 문자를 하나씩 따와 만든 줄임말로 각각은 아래처럼 매칭이 됩니다. C : Create(생성) - POST, R : Read(조회) - GET, U : Update(수정) - PUT, D : Delete(삭제) - DELETE
7. `PUT` : 데이터의 전체를 바꿀 때 사용
8. `PATCH`: 데이터의 일부만 바꿀 때 사용
9. 예를 들어, `PUT` 으로 넘겨준 객체가 `name` 만 가지고 있다면, `email` 은 `null` 로 바뀌지만, `PATCH` 로 넘겨주면 `name` 이 변경되고, `email` 은 기존의 데이터를 유지합니다. 보통 `openAPI` 에서는 `PUT` 을 지원하지 않습니다. 주로 `API` 를 직접 만들 때 주로 `PUT` 이 사용됩니다.
10. `openAPI` 에 `DELETE` 요청을 보내도 실제 서버에 있는 데이터가 삭제되지는 않습니다. 
11. `HTTP 204`: 요청이 성공했으나, 클라이언트가 현재 페이지에서 벗어나지 않아도 된다는 것을 나타냅니다.

### ❏ Axios 사용법
```javascript
<script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
<script src="https://unpkg.com/axios/dist/axios.min.js"></script>

// POST: 새로운 자원 생성
axios.post(url, data 객체)

// GET: 자원을 요청
axios.get(url)

// PUT: 자원을 갱신
axios.put(url, data 객체)

// DELETE: 자원을 삭제
axios.delete(url)
```

```javascript
// POST
function axiosPost() {
  const token = document.getElementById("token");
  const data =  { "email": "eve.holt@reqres.in", "password": "cityslicka" };
  const URL = "https://reqres.in/api/login";
  
  axios.post(URL, data)
    .then(res => {
        token.innerHTML = res.data.token
    })
}
export default axiosPost;

// GET
function axiosGet() {
  const name = document.getElementById("name");
  const email = document.getElementById("email");
 
  const URL = "https://reqres.in/api/users/2";
  axios.get(URL)
    .then(res => {
        const {data} = res.data;
        const emailData = data.email;
        const nameData = `${data.first_name} ${data.last_name}`
        name.innerHTML = nameData;
        email.innerHTML = emailData;
    })
}
export default axiosGet;

// PUT
function axiosPut() {
  const name = document.getElementById("name");
  const emailEl = document.getElementById("email");
  const updateDate = document.getElementById("update_date");
  
  const data = { "first_name": "White", "last_name": "Rabbit" , "email": "alice@elice.io" };
  const URL = "https://reqres.in/api/users/2";
  
  axios.put(URL, data)
    .then(res => {
        const {email, first_name, last_name, updatedAt} = res.data;
        emailEl.innerHTML = email;
        name.innerHTML = `${first_name} ${last_name}`
        updateDate.innerHTML = updatedAt
    })
}
export default axiosPut;

// DELETE
function axiosDelete() {
  const statusEl = document.getElementById("status");
  const URL = "https://reqres.in/api/users/2";
  
  axios.delete(URL)
    .then(res => {
        const {status} = res;
        statusEl.innerHTML = status;
    })
}
export default axiosDelete;
```

---
## 📍 21일차 11.23.화.(실시간 강의) (클린코드와 타입스크립트)
이번주는 `클린코드`와 `typescript`의 `타입`, `클래스`, `인터페이스`, `Generic`, `Decorator`에 대해서 배웠다. 엘리스 엔지니어 SW트랙을 신청할 당시 제일 기대가 되었던 커리큘럼이 이번주차에 배우는 내용이었는데, 벌써 그 내용을 듣게 된다니.. 이전보다 더욱 열심히 들어야겠다. 여느때와 마찬가지로 이론수업과 실습수업으로 나뉘었는데, 실습수업은 김병철 코치님이 가르쳐주셨다. 처음에는 누군지 잘 몰랐는데 알고리즘계에서 꽤 유명한 분이셨다. 개발자 오픈채팅방에 코딩테스트 대비 순서에 대해 물어보면 항상 <a href='https://github.com/tony9402/baekjoon'>tony9402 - 코딩테스트 대비 문제집</a>부터 풀라는 얘기가 많았는데 그 레포지터리 컨트리뷰터의 2번째(<a href='https://github.com/VSFe'>VSfe</a>)분이셨다. 😲😲 저번 이고잉님이 가르쳐주실때도 신기했는데 이번에도 엄청 신기했다.. 공부 의지가 한껏 솟아오르는 계기가 되었다.

### ❏ 클린코드란
1. 비즈니스 전문가 → 분석가(제품관리자 / 서비스 기획자 / 프로그래머) → 프로그래머 → 컴퓨터
2. 좌측 방향은 목적 / 추상적, 우측 방향은 수단 / 구체적
3. 시간이 갈수록 코드를 쓰는것보다 읽는 비중이 늘어난다.(코드 가독성의 중요성이 늘어남)
4. 코드 재사용(반복되는 문제의 풀이는 재사용 가능, SW 개발 비용 절감)

### 💡 테스트 기법
1. 수동 테스트
 - 품질 담당자가 UI를 사용해 기능 검증
 - 사람의 손으로 일일이 테스트한다.(인건비 증가)
 - 소프트웨어 회귀(시간에 따라 기능이 많아지면, 추가한 기능과 기존의 기능과의 충돌로 인해 기존의 있던 코드조차 실행이 안되는 현상이 발생한다.)

2. 인수 테스트
 - 배치된 시스템을 대상으로 검증
 - 전체 시스템 이상 여부 신뢰도가 높음
 - 높은 비용(작성 / 관리 / 실행 비용)
 - 피드백 품질이 낮음(현상을 드러나지만 원인은 숨겨짐)
 - 테스터가 품질 외부를 살펴본다.

3. 자동 테스트
 - 기능을 검증하는 코드를 작성
 - 테스트 코드 작성 비용이 소비되지만 실행 비용이 낮고 결과의 신뢰도가 높음
 - 테스트 코드 작성과 관리가 프로그래머 역량에 크게 영향을 받는다.

4. 단위 테스트
 - 시스템 일부(하위 시스템)를 대상으로 검증
 - 낮은 비용
 - 높은 피드백 품질
 - 전체 시스템 이상 여부 신뢰도가 낮음
 - 단위끼리 오류가 나는 경우가 있다.
 - 테스터가 프로그램의 기능을 살펴본다.

### ❏ 타입스크립트의 역사
1. ES2015부터 모듈 스펙을 제공하기 시작: 프로젝트의 규모 증가, 개발환경이 복잡해짐, `npm` 의 등장, 번들러 등장(Webpack 등등) 주석제거 / 파일압축 / 어글리파이, 트랜스파일러 등장 (Babel, Typescript 등등)
2. `TS` 는 `JS` 의 모든 기능을 기본으로 제공한다. (슈퍼셋), 명시적인 데이터에 대한 유형 설명
3. 자바스크립트보다 타입에 대한 추가적인 정보를 얻을 수 있다.
4. 안정성 있는 코드를 작성하기 위하여 별도의 타입체크가 필요함
5. 예상치 못한 오류가 발생할 수 있음
6. 타입 체크를 위해 코드가 길어지는 문제 발생
7. 실제 코드를 실행을 해보기 전까지 오류 체크 불가
8. 실제 서비스 단계가 아닌 컴파일러 과정에서 오류를 확인할 수 있다.(디버깅, 새로고침 과정까지 가지 않아도 확인 가능함) 보다 안전한 프로그래밍 환경을 제공받을 수 있다.

```
JS
 - 인터프리터 언어(한줄 한줄 실행)
 - 스크립팅 언어
 - 컴파일러 필요 없음
 - 객체 지향적이지 않음, 프로토타입 기반

TS
 - 컴파일 언어
 - 객체 지향 프로그래밍 언어
 - 컴파일러 필요
 - 클래스 기반, 상속, 인터페이스, 수정자 사용 가능
```

### ❏ typescript의 type알아보기
1. 인터페이스의 경우, 컴파일하는 과정에서 인터페이스끼리 전부 합쳐지고 해당 인터페이스에 대응하는 객체를 생성해주는 과정을 거칩니다. (JS의 호이스팅을 떠올릴 수 있지만, 실제 동작과정은 약간 다릅니다. 일반적으로 인터페이스, 클래스 등의 정의는 최상단에 고정하고 하단에 추가하거나 수정하는 것은 지양하는 편 입니다.)

```typescript
// 타입 유틸리티
// 1. Tuple: 튜플, 보다 엄격하게 타입을 정의하고 싶을 때 사용
let x : [number, string];
x = [27, "AYW"];

// enum
enum Color {
	Red, Green, Blue
}

console.log(Color)
👉🏽 { 0: 'Red', 1: 'Green', 2: 'Blue', Red: 0, Green: 1, Blue: 2 }

 - 값을 할당해주지 않으면 0, 1, 2가 들어간다.

enum Color {
	Red = 2, Green, Blue
  }
  
console.log(Color[2])
👉🏽 Red

// any
let num: any = "123";

// void: 함수가 리턴하는 값이 없을 때 사용하는 타입
function warnUser(): void{
  console.log("This is my warning message")
}

function temp(age: number): number{
  return age;
}

// null
let none: null = null;

// undefined
let done: undefined = undefined;

// never
function error(message: string): never{
  throw new Error(message);
}

function infiniteLoop(): never {
  while(true){
    /* 기능 */  
  }
}

// 타입 별칭
let x: number = 10;
let xPositina: number = 10;

type YesOrNo = string;
type YesOrNoDetail = "Y" | "N";

let sayMe: YesOrNo = "HI";
let sayYou: YesOrNoDetail = "Y"

// 인자가 없고 리턴 값이 string 타입인 type 지정
type FooFunction = () => string;
let temp: FooFunction = () => {
  return "temp"
}

// interface

type Name = "AYW";

interface IUser{
  id: number;
  name: Name;
  email: string;
  age: number;
}

const myInfo: IUser = {
    id: 1,
    name: "AYW",
    email: "any",
    age: 27
}

// interface는 속성 값끼리 합칠 수 있다. 
interface IUser{
  id: number;
  name: Name;
  email: string;
  age: number;
}

interface IUser {address: string}

// type 별칭은 불가능하다.
type IUser{
  id: number;
  name: Name;
  email: string;
  age: number;
}

type IUser {address: string}
👉🏽 Error. Duplicate identifier 'IUser'.

// keyof: 타입에 있는 속성값들을 하나의 타입으로 묶는다.
interface User {
    id: number;
    name: string;
    age: number;
    gender: "male" | "female";
}

type UserKey = keyof User;
// 'id' | 'name' | 'age' | 'gender'

const uk: UserKey = "name"
console.log(uk)
```

### ❏ type utility 알아보기
1. `typescript`는 일반적인 타입 변환을 쉽게 하기 위해서 몇 가지 유틸리티 타입을 제공합니다. 이러한 유틸리티는 전역으로 사용 가능합니다.

```typescript

// Partial<T>: type 집합의 모든 프로퍼티를 선택적으로 타입을 생성한다.
// Partial 대신 ?를 써도 된다.
interface User {
    id: number;
    name: string;
    age: number;
    gender: 'male' | 'female'
}

let admin: Partial<User> = {
    id: 1,
    name: "AYW",
}

console.log(admin);

// Readonly<T>: 처음 설정한 값외에 속성을 수정 할 수 없다. 재할당 금지
interface User {
    id: number;
    name: string;
    age: number;
    gender: 'male' | 'female'
}

let admin: Readonly<User> = {
    id: 1,
    name: "AYW",
    age: 27,
    gender: "male"
}

admin.id = 3;
console.log(admin)

👉🏽 Cannot assign to 'id' because it is a read-only property.

// Readonly
interface User {
    id: number;
    name: string;
    age: number;
    readonly gender: 'male' | 'female'
}

let admin: User = {
    id: 1,
    name: "AYW",
    age: 27,
    gender: "male"
}

admin.id = 3;
admin.gender = "female";  // error
console.log(admin)
👉🏽 Cannot assign to 'gender' because it is a read-only property.

// Record<K, T>: 개체의 속성과 타입을 정의할 때 사용하는 메소드
type Grade = "1" | "2" | "3" | "4";
type Score = "A" | "B" | "C" | "D";

const score: Record<Grade, Score> = {
    1: "A",
    2: "B",
    3: "C",
    4: "D",
}

console.log(score)

// Record<K, T>: 타입의 프로퍼티 키의 집합으로 타입을 생성한다. 개체의 속성과 타입을 정의할 때 사용하는 메소드
interface User {
    id: number;
    name: string;
    age: number;
}

function isValid(user: User){
    const result: Record<keyof User, boolean> = {
        id: user.id > 0,
        name: user.name !== '',
        age: user.age > 0,
    }
    return result;
}

// Pick<T, K>: Type에서의 Key값을 선택하여 새로 type으로 정하는 기능
interface User {
    id: number;
    name: string;
    age: number;
    gender: "male" | "female";
}

const admin: Pick<User, "id"|"name"> = {
    id : 0,
    name: "TED"
}

console.log(admin)

// Omit<T, K>: Type에서의 Key값을 선택하여 사용하지 못하게 한다.
interface User {
    id: number;
    name: string;
    age: number;
    gender: "male" | "female";
}

const admin: Omit<User, "id"|"name"> = {
    age: 27,
    gender: "male"
}

console.log(admin)

// Exclude<T1, U>: 속성 대신 Type의 key 값을 제외한다.
type T1 = string | number | boolean;
type T2 = Exclude<T1, number | string>;

let isNum: T2 = 3;
👉🏽 Type 'number' is not assignable to type 'T2'.

let isNum: T2 = true;

// NonNullable<T>: undefined와 null 타입을 제거한다.
type T1 = string | null | undefined | void;
type T2 = NonNullable<T1>;

let empty: T2 = null;
👉🏽 Type 'null' is not assignable to type 'T2'.
let empty: T2 = "Hi";

// Parameters<T>: 함수 타입을 인자로 받아서 튜플타입으로 리턴해주는 문법
type T0 = Parameters<() => string>;  // []
type T1 = Parameters<(s: string) => void>;  // [string]
type T2 = Parameters<(s: string, i: number) => number>

let T1Arr: T1 = ["123"];

// ReturnType<T>: return type값을 정의하는 문법
type T0 = ReturnType<() => string>;

function returnString(): T0{
    return "123"
}

type T7 = ReturnType<any> // any
type T8 = ReturnType<never> // any

// Required<T>: partial과 반대되는 기능으로 type집합의 모든 프로퍼티를 필수로 설정한다.
interface User {
    id: number;
    name?: string
}

let admin: Required<User> = {
    id: 1,
}

👉🏽 Property 'name' is missing in type '{ id: number; }' but required in type 'Required<User>'.

let admin: Required<User> = {
    id: 1,
		name: "AYW"
}
```

### ❏ 타입스크립트의 함수
1. 일급객체(first-class object): 함수를 변수로 선언하고, 함수에 인자를 함수로 넘길 수 있고, 함수의 리턴값을 함수로 설정할 수 있는 것을 일급객체라 부릅니다. `JS` 와 `TS` 는 모두 일급객체입니다.
2. 일급객체의 특징 때문에 고차함수, 콜백함수를 만들 수 있다.

```ts
// 함수 자체를 값으로 저장한다.
let sum = function(a, b){
  return a + b;
}

function ul(child){
  return `<ul>${child}</ul>`
}

// 함수를 리턴할 수 있다.
function makeLi(container, contents){
  const liList = [];

  for (const content of contents){
    liList.push(`<li>${content}</li>`)
  }

  return container(liList.join(""))
}

// 함수를 함수의 인자로 넣어줄 수 있다.
const htmlUl = makeLi(ul, ['월', '화', '수', '목', '금', '토', '일'])
```

3. 함수의 선언문, 선언식
```ts
// 함수 선언문
function sum(a, b){
	return a+b;
}

// 함수 표현식
const myFunc = function(a, b){
		return a+b;
}
```

4. 함수의 가변인자
```ts
function sum(a, b){
	return a+b;
}

const abcSum = sum(10, 20, 30);

// 가변 인자식
function sum(){
  let s = 0;
	for (let i=0; i< arguments.length; i++){
		s+=arguments[i];
	}
	return s;
}

// arguments
function sum(...args){
  let s = 0;
	for (let i=0; i< args.length; i++){
		s+=args[i];
	}
	return s;
}
```

4. 함수 호출
```ts
// call과 apply는 인자를 하나씩 넘겨주냐 배열로 넘겨주냐의 차이
sum(10, 20, 30, 40);
// 컨텍스트 null
sum.call(null, 10, 20, 30, 40);

arr = [10, 20, 30, 40];
sum.apply(null, arr);
```

5. 함수의 종류
```ts
// 즉시 실행 함수
(function(){
  console.log(123);
})

// 일반함수와 화살표함수의 차이:  컨텍스트의 차이점
const sumV2 = (a, b, ...args) => {

}

const ten = () => 100;
const hundred = x => 100 + x;

// 생성기 함수(generate function): 함수를 한번에 실행시키는 것이 아니라 텀을 두고 실행할 때
function* gen(){
    yield 10;
    yield 20;
    return 30;
}

const g = gen();

console.log(g.next());  // 10
console.log(g.next());  // 20
console.log(g.next());  // 30
```

6. 함수 작성시 반환 타입 명시 권장(필수는 아님, `TS` 컴파일러는 방정식의 한쪽에만 타입이 있더라도 타입을 추론할 수 있다.)
7. 매개변수와 인수의 타입이 호환 가능하게 작성, 인수 타입의 전달이 잘못된 경우 오류 발생

```ts
// 함수를 안전하게 만들 수 있다.
interface MathFn {
    (a: number, b: number): number;
    operator: string;
};

const sum: MathFn = (a, b) => a + b;
sum.operator = "+";

1. void: 반환값이 없는 함수입니다. (그냥 출력하거나, 상태를 바꿀 때 자주 씁니다.)
2. never: 함수가 종료되지 않습니다. (무한루프를 돌거나, Error를 띄울 때 사용합니다.)
```

8. 함수의 매개변수: 함수에 주어진 인자의 개수는 함수가 기대하는 매개변수의 수와 일치해야 함

```ts
function sum(a: number, b:number, type?: string): number{
    return a+b;
}

let sumAge = sum(2, 3, "ted");

function buildName(firstName: string, lastName="Smith") {
    return firstName + ' ' + lastName;
}

let result1 = buildName("Bob");
let result2 = buildName("Bob", undefined);
let result3 = buildName("Bob", 'Ted');
console.log(result1)
👉🏽 "Bob Smith" 


[LOG]: "Bob Smith" 
[LOG]: "Bob Ted"

console.log(result2)
console.log(result3)

undefined가 넘어가면 lastName이 없다고 판단되지만, null이 들어가면 lastName이 있다고 판단을 합니다. 
(undefined는 값 자체가 없다고 판단하나, null은 값은 있는데 의미없는 특별한 값이 들어있다고 보시면 좋을 것 같아요.)
+ undefined는 미리 선언된 global variable이나, null은 키워드입니다.
```

### ❏ 객체 지향 프로그래밍(OOP)
1. `OOP` 는 컴퓨터 프로그램을 객체의 모임으로 파악하려는 프로그래밍 패러다임
2. 프로그램을 유연하고, 변경이 용이하고, 개발과 보수를 간편하게 만든다, 직관적인 코드 분석이 가능해진다.
3. 클래스 요소: 필드(field), 생성자(constructor, 객체가 처음 생성될 때 호출, 멤버 변수 초기화), 메소드(method)
4. 인스턴스: `new` 연산자에 의해서 생성된 객체

```ts
class Person {
    name: string;
    constructor(name: string){
        this.name = name
    }
    say(){
        return `Hello, ${this.name}!`
    }
}

let person = new Person("AYW");
console.log(person.say())
```

### ❏ 클래스 만들기
1. 생성자의 매개변수에 `public` 과 같은 접근 제한자를 붙이면 해당 매개변수의 이름을 가진 속성이 클래스에 선언된 것처럼 동작합니다.

```ts
// public 접근 제한자
class Information {
  constructor(public name: string, public age: number){}
}

const myInfo = new Information("AYW", 27);
console.log(myInfo)
👉🏽 { name: 'AYW', age: 27 }

// this
class Information {
    name: string;
    age: number
  constructor(name: string, age: number){
    this.name = name;
    this.age = age;
  }
}

const myInfo = new Information("AYW", 27);
console.log(myInfo)
👉🏽 { name: 'AYW', age: 27 }
```

### ❏ 클래스 상속받기
1. 부모 클래스를 상속받는 키워드: `extends`

```ts
class AYW extends Information{
  constructor(public name: string, public age: number, gender: "male" | "female"){
    super(name, age)
  }

  sayHello(): void {
    console.log(`제 이름은 ${this.name}입니다.`)
  }
}

const myInfo: AYW = new AYW("AYW", 27, "male")
console.log(myInfo);
👉🏽 AYW { name: 'AYW', age: 27 }

myInfo.sayHello();
👉🏽 제 이름은 AYW입니다.
```

### ❏ 추상 클래스
1. 추상 클래스는 자신의 속성이나 메서드 앞에 `abstract`를 붙여 나를 상속하는 다른 클래스에서 이 속성이나 메서드를 구현하게 합니다.

```ts
abstract class Information {
    name: string;
    age: number;
    constructor(name: string, age: number) {
        this.name = name;
        this.age = age;
    }

    abstract sayHello(): void;
}

class AYW extends Information {
    constructor(
        public name: string,
        public age: number,
        gender: "male" | "female"
    ) {
        super(name, age);
    }

    sayHello(): void {
        console.log(`제 이름은 ${this.name}입니다.`);
    }
}

const myInfo: AYW = new AYW("AYW", 27, "male");
console.log(myInfo);
👉🏽 AYW { name: 'AYW', age: 27 }

myInfo.sayHello();
👉🏽 제 이름은 AYW입니다.
```