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
## 📍 11.3.수(실시간 강의)
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






