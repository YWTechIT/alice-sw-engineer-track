## 📍 엘리스 SW 엔지니어 트랙

## 📍 O.T

1. 주 5일, 총 560시간 동안 온/오프라인 병행하여 진행

-   Part 1: JS 기초(1~4주차)
-   Part 2: `Typescript`, `Node.js`, `SQL(5~9주차)` + 웹 서비스 프로젝트1
-   Part 3: `React` + 웹 서비스 프로젝트2

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
<header>
    <!-- 상단 영역 -->
    <img src="elice_logo.png" alt="엘리스 로고" />
    <nav>
        <!-- 메뉴 버튼 영역 -->
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
<main role="main">
    <!-- 본문 영역 -->
    <article><!-- 정보 영역 --></article>
</main>
```

21. `<footer>`: 웹 사이트의 가장 하단에 들어가는 정보를 표기할 때 사용
22. `<div>`: 임의의 공간을 만들 때 사용

```html
<footer>
    <!-- 하단 영역 -->
    <div>
        <!-- 회사 정보 -->
        <p>주소: 경기도 화성시 동탄공원로</p>
        <p>이메일: ywtechit@gmail.com</p>
    </div>
    <div>
        <!-- 전자상거래소비자보호법 필수 정보 -->
        <p>사업자등록번호: 000-00-00000 | 대표: 안영우</p>
        <p>통신판매업신고번호: 제0000-토끼굴-0000호</p>
    </div>
</footer>
```

23. `display: block`과 `display: inline`의 큰 차이점: 줄 바꿈 현상, `width`, `height`, 상 하 배치
24. `display: block`: `y`축 정렬 형태로 출력(줄 바꿈 현상이 보인다.) `width`, `height`로 공간을 만들고 상하 배치 작업이 가능하다. (`h`, `p`)
25. `display: inline`: `x`축 정렬 형태로 출력(한 줄에 출력) `width`, `height`로 공간을 만들 수 없고 상하 배치 작업이 불가능하다. (`a`, `span`)
26. `CSS` 적용 방법 3가지: 첫번째로 `inline style sheet`로 태그 안에 직접 원하는 스타일을 적용한다. (`<h1 style="color: red;">)coding 101 </h1>`) 두번째는 `internal style sheet`로 `<style>` 태그 안에 넣어서 적용한다. (`<style> h1{ background-color: yellow;}</style>`) 마지막으로 `external style sheet`로 외부에 `css`파일을 저장해두고 `<link>` 태그로 불러오기 (`<head> <link rel="stylesheet" (연결 할 문서의 정보의 성격 지정) href="style.css(경로입력)"></head>`, `link` 태그는 닫힌 태그가 없다. ) 마지막 CSS 방법(`external`)의 장점은 `html`, `css` 각각의 문서 안에서 따로 관리하여 상대적으로 가독성이 높고 유지보수가 쉽다. (실무에서 많이 사용)
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
p {
    color: red;
}
p {
    color: blue;
} // ✅

/* 더 구체적으로 작성된 선택자의 우선순위가 높다. */
header p {
    color: red;
} // ✅ detail
p {
    color: blue;
}

/* `inline style > id > class > type` 순으로 우선순위가 높다. */
<h3 style = "color: pink" id="color" class="color">color</h3>  // 1
#color {
    color: blue;
} // 2
.color {
    color: red;
} // 3
h3 {
    color: green;
} // 4
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
    background: yello url() no-repeat left; // 한번에 입력
}
```

### ❏ 웹 사이트 레이아웃에 영향을 미치는 요소

1️⃣ 박스모델: 공간 크기가 어떤 구조로 구성되어 있는지 확인하는 모델(`margin`, `border`, `padding`, `content`)

1. `top`, `right`, `bottom,left` 순서로 입력가능
2. `margin` : `border`를 기준으로 바깥에 있는 요소
3. `padding`: `border` 와 `content` 사이의 간격

2️⃣ Block요소와 Inline 요소: `block`요소는 `y` 축 정렬(`header`, `p` , `width`, `height`, `margin`, `padding` 요소 사용가능), `inline` 요소는 `x` 축 정렬 (`a`, `span`), `margin-top`, `margin-bottom` 등 상하 배치 작업 속성은 사용 불가, 줄바꿈 없음

3️⃣ 마진 병합 현상

1. 형제지간의 마진 병합: 큰 값을 우선순위로 `space` 를 만든다. 하단의 코드에서는 `250px` 이 아니라 `150px` 로 설정된다.

```html
<div class="box1">Hello World</div>
<div class="box2">Hello World</div>

.box1{ margin-bottom: 150px } .box2{ margin-top: 100px }
```

기존계산으로는 `margin` 이 `250px`이 되어야 하지만 마진의 교집합이 있을때는 더 높은 값에 우선순위가 주어지므로 `150px` 만큼만 차이가 난다.(마진 병합 현상)

2. 부모 자식간의 마진 병합: 부모도 함께 `space` 적용이 된다. 평소처럼 생각하면 자식 `div` 에만 `margin` 이 되어야하는데, 부모도 함께 `space` 적용이 된다.

```html
<main role="main">
    <article></article>
</main>

.article { width: 200px; height: 200px; margin-top: 100px; }
```

![](https://images.velog.io/images/abcd8637/post/f3f010ae-1148-4137-ba50-c6105892ab0b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-27%2020.24.52.png)

tip: 부모는 그대로인데 자식 `div`만 내리려면 자식 `div`에 `position: absolute`를 넣어준다.

![](https://images.velog.io/images/abcd8637/post/43cdd193-481e-427b-8ae5-19d937d48027/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-10-27%2020.26.05.png)

4️⃣ 레이아웃에 영향을 미치는 속성

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

6. `float` 을 마지막으로 사용한 태그 다음 태그에 `clear` 속성을 사용한다. 만약, `float: left` 만 되어있다면 `clear: left` , `float: right` 만 되어있다면 `clear: right` 양쪽은 `clear: both` 를 사용하면 된다. 보통의 경우에는 `clear: both` 를 많이 사용한다.

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
1. 부모 자식 지간에 발생하는 마진 병합 현상(margin-collapse)이 일어나면 2차원
속성이다. 2. `top`, `left`, `right`, `bottom`을 설정 할 수 있는 속성은
3차원이다. 3. 부모가 높이 값을 갖고 있지 않을 때 자식의 높이 값이 부모의 높이
값에 영향을 준다면 2차원 속성이고, 영향을 주지 않는 다면 3차원 속성이다.
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
`background-attachment`: 배경이미지의 스크롤 여부를 결정짓는 요소 1.
`background-attachment: scroll`: 스크롤하면 배경이미지가 고정되지 않음 2.
`background-attachment: fixed`: 스크롤하면 배경이미지가 고정되면서 같이 내려감
```

4. `y`축 정렬 방법: 다음의 공식을 이용한다.

```css
top: 50%; /* position: fixed, relative, absolute */
transform: translateY(
    -50%
); /* Y축으로 -50%만큼 이동한다. 자신의 크기를 기준으로 좌표가 형성된다. */
```

5. `box-sizing: border-box`: `box-model` 중 `padding`을 사용하면 공간의 크기가 바뀌지 않게 안전장치를 걸어준다. 공간에 대한 크기는 그대로인 상태에서 `padding` 값만 적용된다.

### ❏ 메인 페이지 살펴보기

1. `box-shadow`: 공간의 그림자 효과를 만들 때 사용하는 `css` 속성

```css
.box_shadow {
    width: 300px;
    height: 300px;
    box-shadow: 10px 10px 10px 10px red; /* 수평방향(x), 수직방향(y), 흐림의 반경(숫자가 클 수록 그림자의 끝이 흐려지고 0이 될수록 선명하다), 그림자가 확산되는 거리, 그림자의 색상 */
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
        <input type="text" id="topic" name="topic" />
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
    <input type="text" id="title" name="title" />

    <label for="email">이메일 주소</label>
    <input type="email" id="email" name="email" />

    <label for="password">비밀번호</label>
    <input type="password" id="password" name="password" />
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
<input
    type="button"
    value="day"
    onclick="
      document.querySelector('body').style.backgroundColor='white';
      document.querySelector('body').style.color='black';
"
/>

<!-- 야간 모드 -->
<input
    type="button"
    value="night"
    onclick="
      document.querySelector('body').style.backgroundColor='black';
      document.querySelector('body').style.color='white';
"
/>

<!-- 리팩토링 1: 토글기능(한 개의 버튼으로 모드 변경 가능) -->
<input
    id="dn"
    type="button"
    value="night"
    onclick="
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
  "
/>

<!-- 리팩토링 2: this 사용(id값을 설정 할 필요 없이 `this`를 통해 동일한 버튼이 여러개여도 각각의 기능을 보장한다. -->
<input
    type="button"
    value="night"
    onclick="
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
  "
/>
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
document.write('"It\'s all right."');
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
"10" + 2; // 102

// 피연산자가 모두 숫자 타입이어야 하는 문맥
5 * "10"; // 50

// 피연산자 또는 표현식이 불리언 타입이어야 하는 문맥
!0; // true
if (1) {
} // {}

// 숫자 타입
0 +
    "" - // "0"
    0 +
    ""; // "0"
1 +
    "" - // "1"
    1 +
    ""; // "-1"
NaN + ""; // "NaN"
Infinity +
    "" - // "Infinity"
    Infinity +
    ""; // "-Infinity"

// 불리언 타입
true + ""; // "true"
false + ""; // "false"

// null
null + ""; // "null"

// undefined
undefined + ""; // "undefined"
```

7. 숫자 타입으로 변환: `빈 문자열('')`, `null`, `false`는 `0으`로 `true`는 `1로` 반환된다. 객체와 빈 배열이 아닌 배열, `undefined`는 변환되지 않아 `NaN`이 된다는 것에 주의하자.

```javascript
1 - "1"; // 0
1 * "10"; // 10
1 / "one" + // NaN
    // 문자열 타입
    "" + // 0
    "0" + // 0
    "1" + // 1
    "string" + // NaN
    // 불리언 타입
    true + // 1
    false + // 0
    // null 타입
    null + // 0
    // undefined 타입
    undefined; // NaN
```

8. 불리언 타입으로의 변환: 아래의 값들은 `falsy`로 평가되는 `Falsy`값이다. 이 값들 외에 값은 `truthy(참으로 평가되는 값)`라고 보면 된다.

```javascript
// 아래의 조건문은 모두 코드 블록을 실행한다.
if (!"") {
    console.log("execute");
}
if (!false) {
    console.log("execute");
}
if (!undefined) {
    console.log("execute");
}
if (!null) {
    console.log("execute");
}
if (!0) {
    console.log("execute");
}
if (!NaN) {
    console.log("execute");
}
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
for (let i = 0; i < arr.length; i++) {
    console.log(arr[i]);
}

// 배열 타입: object
typeof [1, 2, 3]; // object

// 배열과 객체 순회 속도 비교
const array = [];
console.time("Array Performance Test");

for (let i = 0; i < 10000000; i++) {
    array[i] = i;
}

console.timeEnd("Array Performance Test"); // 약 340ms

const obj = {};
console.time("Object Performance Test");

for (let i = 0; i < 10000000; i++) {
    obj[i] = i;
}

console.timeEnd("Object Performance Test"); // 약 600ms
```

2. `html`에서 `a`태그 모두 선택하기: `document.querySelectAll("a")`

```javascript
// 배열 길이 만큼 li태그에 값 넣기
for (let i = 0; i < names.length; i++) {
    document.write(
        `<li><a href="${i}.html" target="_blank">${names[i]}</a></li>`
    );
}

// `a` 태그의 모든 값 색상 바꾸기
for (let i = 0; i < aTags.length; i++) {
    console.log((aTags[i].style.color = "red"));
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
<input
    type="button"
    value="night"
    onclick="
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
  "
/>

<!-- 리팩토링 후: onclick 기능 코드만 따로 함수로 빼내어 가독성을 높였다. -->
<input type="button" value="night" onclick="toggleDarkMode(this);" />
<script>
    const body = document.querySelector("body");

    function toggleDarkMode(target) {
        if (target.value === "night") {
            body.style.backgroundColor = "black";
            body.style.color = "white";
            target.value = "day";

            let a = document.querySelectorAll("a");
            for (let i = 0; i < a.length; i++) {
                a[i].style.color = "white";
            }
        } else {
            body.style.backgroundColor = "white";
            body.style.color = "black";
            target.value = "night";

            let a = document.querySelectorAll("a");
            for (let i = 0; i < a.length; i++) {
                a[i].style.color = "black";
            }
        }
    }
</script>

<input type="button" value="night" onclick="toggleDarkMode(this)" />
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
var fruit; // 변수 선언: 데이터를 담을 공간을 생성하는 것
fruit = "apple"; // 변수 초기화: 생성된 변수에 공간을 생성하는 것

var fruit = "apple"; // 변수 선언 및 초기화
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
var num4 = Number.MAX_SAFE_INTEGER; // 9007199254740991
var num5 = Number.MIN_SAFE_INTEGER; // 9007199254740991
```

5. 함수(`function`)

```js
// 함수 표현식
var func1 = function () {
    console.log("func1");
}; // 함수 생성

func1(); // 함수 호출

// 함수 선언식
function func2() {
    console.log("func2");
}

// 매개변수: width, height
var area = function (width, height) {
    return width * height;
};

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
str1.length; // 문자열 길이 11
str1.charAt(0); // 문자열 추출
str1.split(" "); // 공백 기준으로 문자를 나누고 배열에 담는 메서드
```

3. 배열 메서드

```js
var fruit = ["사과", "배", "포도"];
fruit.length;
fruit.push("딸기"); // 배열 뒤에 데이터 삽입
fruit.unshift("레몬"); // 배열 앞에 데이터 삽입
fruit.pop(); // 배열 뒤의 데이터 제거
fruit.shift(); // 배열 앞의 데이터 제거
```

4. `math` 의 수학 연산 메서드

```js
Math.abs(-3); // 절대값
Math.ceil(0.3); // 올림
Math.floor(10.9); // 내림
Math.random(); // 임의의 숫자 출력
```

5. 문자를 숫자로 변환하는 메서드

```jsx
parseInt("20.6"); // 정수 형태의 20 변환
parseFloat("20.6"); // 실수 형태의 20.6 변환
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
    console.log(line);
    rl.close(); // close가 없으면 입력을 무한히 받는다.
});
rl.on("close", () => {
    // 입력이 끝난 후 실행할 코드
});

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
console.log(20 + 10); // 30
console.log(20 - 10); // 10
console.log(20 * 10); // 200
console.log(20 / 10); // 2
console.log(20 % 10); // 0
```

2. 증감 연산자: `++`: 1씩 증가, `--`: 1씩 감소 (전치연산자는 먼저 연산을 하고 출력한다. 후치연산자는 먼저 출력을 하고 연산한다.)

```js
let num = 10;

console.log(++num); // 11
console.log(--num); // 10

console.log(num++); // 10
console.log(num--); // 11
```

3. 비교 연산자: 데이터의 대소비교

```js
console.log(10 == 20); // false, 값이 같다
console.log(10 === 20); // false, 데이터 타입도 같고 값도 같다.
console.log(10 !== 20); // true

console.log(10 > 20); // false
console.log(10 >= 20); // false
console.log(10 < 20); // true
console.log(10 <= 20); // true
```

4. 논리 연산자

```jsx
console.log(10 === 10 && 20 === 30); // false, 앞 뒤 조건 모두 참인 경우만 true를 반환하는 AND 연산자
console.log(10 === 10 || 20 === 30); // true, 둘 중 하나만 참이여도 true를 반환하는 OR 연산자
```

### ❏ 조건문

1. `if` 문: `if(조건){수행할 명령}`

```js
let a = 20;
let b = 40;
if (a < b) {
    console.log("a는 b보다 작다.");
}
```

2. `if-else` 문: 조건이 `true` 면 `if`문, `false` 면 `else` 문 실행

```js
let a = 20;
let b = 40;

if (a < b) {
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

if (a > b) {
    console.log("a는 b보다 크다.");
} else if (b > c) {
    console.log("b는 c보다 크다.");
} else if (a < c) {
    console.log("a는 c보다 작다.");
} else if (b < c) {
    console.log("b는 c보다 크다.");
} else {
    console.log("모든 조건을 만족하지 않는다.");
}
```

4. `중첩 if문` : if문 안에 또 다른 if문을 삽일 할 때 사용

```jsx
let a = 20;
let b = 40;

if (a !== b) {
    if (a > b) console.log("a는 b보다 크다");
    else console.log("a는 b보다 작다");
} else {
    console.log("a와 b는 같다.");
}
```

### ❏ 반복문

1. `for` 문: `for( 초기화 한 변수값; 조건; 증감 표시){ 수행할 명령 }`

```js
for (let i = 0; i < 10; i++) {
    console.log(i);
}
```

2. `while` 문: `while( 조건 ) {수행할 명령}`

```js
let num = 0;

while (num < 10) {
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
function isPrime(n) {
    if (n === 1) return false;
    for (let i = 2; i < Math.floor(n / 2) + 1; i++) {
        if (n % i === 0) return false;
    }
    return true;
}
```

3. 문자열 거꾸로 출력하기: 강의에서는 `charAt`메소드를 사용했는데 그것보다 문자열 인덱싱으로 풀었다.

```jsx
// 나의 코드
function reverse(str) {
    var reverStr = "";
    for (let i = str.length - 1; i >= 0; i--) {
        reverStr += str[i];
    }
    return reverStr;
}

document.write(reverse("Nice to meet you"));
```

4. 구구단 출력하기

```js
for (let i = 2; i <= 9; i++) {
    for (let j = 1; j <= 9; j++) {
        document.write(`${i}x${j}=${i * j}`);
        document.write("<br>");
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
        <meta charset="UTF-8" />
        <title>자바스크립트 기초</title>
    </head>
    <body>
        <div name="red" class="fruit" id="apple">apple</div>
        <div name="yellow" class="fruit" id="banana">banana</div>
        <div name="red" class="vegetable" id="carrot">carrot</div>
        <div name="white" class="vegetable" id="onion">onion</div>
        <script src="index.js"></script>
    </body>
</html>
```

```javascript
let $apple = document.getElementById("apple").childNodes[0]; // "apple"
let $appleNodeValue = $apple.nodeValue; // "apple"
let $appleNodeType = $apple.nodeType; // 3(텍스트 노드)
```

### ❏ 이벤트(Event)

1. 이벤트(Event): 웹 브라우저가 알려주는 HTML 요소에 대한 사건의 발생, JS는 발생한 이벤트에 반응하여 특정 동작을 수행할 수 있다. (mouse, scroll, keyboard, window 객체 등)

```javascript
// 마우스 클릭 이벤트 예시
<p onclick="changeText(this)"> 여기를 클릭해주세요</p>;

function changeText(element) {
    element.innerHTML = "내용이 바뀌었읍니다.";
}
```

2. 이벤트 핸들러: 이벤트가 발생했을 때 그 처리를 담당하는 함수. 지정된 이벤트가 발생하면 웹 브라우저에게 등록된 이벤트 핸들러 함수호출을 위임하게 된다.

```js
// HTML 문서가 로드될 때 실행됨
window.onload = function () {
    let text = document.getElementById("text");
    text.innerHTML = "HTML 문서가 로드되었읍니다.";
};
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
            function sayHi(name) {
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
            };
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

            $button.addEventListener("click", function () {
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
        <input type="checkbox" />
        <script>
            const $a = document.getElementsByTagName("a")[0];
            $a.addEventListener("click", function (e) {
                e.preventDefault();
            });

            const $input = document.querySelector("input[type=checkbox]");
            $input.addEventListener("click", function (e) {
                e.preventDefault();
            });
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
            function handleClick(button) {
                console.log(button); // button 요소
                console.log(this); // window
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

            $button.onclick = function (e) {
                console.log(this);
                console.log(e.currentTarget);
                console.log(this === e.currentTarget);
            };
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

            $button.addEventListener("click", function (e) {
                console.log(this);
                console.log(e.currentTarget);
                console.log(this === e.currentTarget);
            });
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

            $button.onclick = (e) => {
                console.log(this);
                console.log(e.currentTarget);
                console.log(this === e.currentTarget);
            };

            const $button = document.querySelector("#btn");

            $button.addEventListener("click", (e) => {
                console.log(this);
                console.log(e.currentTarget);
                console.log(this === e.currentTarget);
            });
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
function outer() {
    a = 3;
}

outer();
console.log(a); // 3
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
console.log(a); // undefined
var a = 1;

// let
console.log(b); // Cannot access 'b' before initialization
let b = 1;

// const
console.log(c); // Cannot access 'c' before initialization
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
function add(a, b) {
    return a + b;
}
```

2. 함수 표현식: 함수 이름을 생략할 수 있는데, 이를 익명 함수라고 한다. 만약, 함수이름을 선언한다면 함수 내부에서만 유효한 식별자이므로 함수 이름으로 함수를 호출할 수 없다. 함수 표현식으로 정의한 함수는 함수 표현식 이전에 호출할 수 없다. 함수의 생성시점이 다르기 때문이다.

```jsx
const add = function (a, b) {
    return a + b;
};
```

3. 화살표 함수: `function`키워드 대신 화살표를 사용해 좀 더 간략한 방법으로 함수를 선언할 수 있다. 화살표 함수는 항상 익명 함수로 정의한다.

```jsx
// 기본 코드
const add = (a, b) => {
    return a + b;
};

// 함수 몸체가 하나의 몸으로 구성된다면 함수 몸체를 감싸는 중괄호를 생략할 수 있다.
const add = (a, b) => a + b;

// 매개변수가 1개인 경우 소괄호를 생략할 수 있다.
const pow = (n) => n * n;
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

function myFunc() {
    let a = 10;
    let b = 20;
    function add(first, second) {
        return first + second;
    }
    return add(a, b);
}

myFunc();

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
function f1() {
    let b = 20;
    function print(v) {
        console.log(v);
    }
    function f2() {
        let c = 30;
        print(a + b + c);
    }
    f2();
}
f1(); // 60
```

```javascript
const o = {
    name: "Kim",
    changeMyName: function (name) {
        this.name = name;
    },
};

const o2 = {
    name: "Song",
};

function callFuncWithArg(f, arg) {
    f(arg);
}

o.changeMyName.bind(o2)("Sam");
console.log("1번 - ", o2.name); // "Sam"

callFuncWithArg(o.changeMyName, "Daniel"); // "Kim"
console.log("2번 - ", o.name);

o.changeMyName("Sam");
console.log("3번 - ", o.name); // "Sam"
```

### ❏ 함수가 호출되는 상황 4가지(`dynamic binding`)

1. 직접 호출: 함수를 직접 호출한다 (myfunc())
2. 메서드 호출: 객체의 메서드를 호출한다.(o.method())
3. 생성자 호출: 생성자 함수를 호출한다. (`const p = new Person()`)
4. 간접 호출: `call`, `apply` 등으로 함수를 간접 호출한다.(`f.call(null, obj)`)
5. 콜백함수(특정 동작 이후에 불려지는 함수), 다른 함수의 인자로 보내지는 함수 등

```javascript
// 직접 호출
function myFunc() {
    console.log("my func called");
}

// 메소드 호출
const o = {
    name: "AYW",
    printName: function () {
        console.log(this.name);
    },
};

o.printName();

// 생성자 호출
function Person(name) {
    this.name = name;
    this.consoleName = function () {
        console.log(this.name);
    };
}

const p = new Person("AYW");
console.log(p);
p.consoleName();

setTimeout(p.consoleName.bind(p), 1000); // AYW
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
    arrowFunc: () => {
        console.log(this);
    },
    generalFunc: function () {
        console.log(this);
    },
};

o.arrowFunc(); // global
o.generalFunc(); // { name: 'TED', arrowFunc: [Function: arrowFunc], generalFunc: [Function: generalFunc] }

setTimeout(o.arrowFunc, 1000); // global
setTimeout(o.generalFunc, 1000); // global
```

7. `setTimeout` 의 `this` 는 `global` 을 가리킨다.
8. `bind`, `apply`, `call` 등의 함수로 `this` 를 조작한다.
9. `setTimeout` 은 함수 호출과는 다른 콜백 호출이다.
10. `printName` 메서드는 `bind` 함수를 이용해 `this` 변수가 `o` 를 가리키도록 컨텍스트를 동적 바인딩한다.

```javascript
const o = {
    name: "TED",
    printName: function () {
        console.log("내 이름은" + this.name);
    },
};

o.printName(); // 내 이름은 TED
setTimeout(o.printName, 1000); // 내 이름은 undefined
setTimeout(o.printName.bind(o), 1000); // 내 이름은 TED
```

### ❏ 화살표 함수와 일반 함수의 this

1. 화살표 함수의 `this` 는 호출된 함수를 둘러싼 실행 컨텍스트를 가리킨다. (선언 당시의 `this` 값을 유지한다. `this` 값을 `bind` , `apply`, `call` 로 바꿀 수 없다.) `this` 가 정해지면 바꿀 수 없다. `setTimeout` 등 `this` 가 바뀌는 상황에서 유용하다.
2. 일반 함수의 `this` 는 새롭게 생성된 실행 컨텍스트를 가리킨다. (`this` 값을 `bind` , `apply`, `call` 로 바꿀 수 있다.), `this` 가 바뀌어야하는 경우는 일반함수를 사용한다.

```javascript
const o = {
    method() {
        console.log(this);
        let f1 = function () {
            console.log(`f1`, this);
        };
        let f2 = () => console.log(`f2`, this);
        f1(); // global
        f2(); // o
    },
};

o.method(); // o
```

```javascript
window.name = "TED";

const o = { name: "AYW" };
const arrow = (prefix) => console.log(prefix + this.name);

arrow("Dr. "); // Dr. TED
arrow.bind(o)("Dr. "); // Dr. TED
arrow.call(o, "Dr. "); // Dr. TED
arrow.apply(o, ["Dr. "]); // Dr. TED
```

### ❏ closure

1. 일급객체란? 다른 변수처럼 대상을 다룰 수 있는것. JS에서 함수는 일급 객체이다. JS에서 함수는 변수처럼 다룰 수 있다.
2. 클로저는 함수의 일급 객체 성질을 이용한다.
3. 함수가 생성될 때, 함수 내부에서 사용되는 변수들이 외부에 존재하는 경우 그 변수들은 함수의 스코프에 저장한다.
4. 함수와 함수가 사용하는 변수들을 저장한 공간을 클로저라 한다.

```javascript
function add(a, b) {
    return a + b;
}

[1, 2, 3].reduce(add, 0);

(() => {
    console.log("익명 함수를 생성한다.");
})();

function outer(a) {
    function inner(b) {
        return a + b;
    }
    return inner(10);
}

// 함수를 변수로 생성한다.
const Person = (name) => {
    const printName = () => console.log(name);
    return { printName }; // 함수를 리턴하며 closure를 생성한다.
};

const person = Person("ted");
person.printName();

function printName(name) {
    console.log(name);
}

// 함수끼리 비교한다.
// ===의 경우, 변수가 같은 객체(함수)를 가리키는지 체크한다.
console.log(printName === person.printName);
```

```javascript
// 클로저 함수 예시
// card1과 card2와 별도의 메모리 공간에 저장된다.

function createCard() {
    let title = "";
    let content = "";

    function changeTitle(text) {
        title = text;
    }
    function changeContent(text) {
        content = text;
    }
    function print() {
        console.log(title), console.log(content);
    }

    return { changeTitle, changeContent, print };
}

const card1 = createCard();
card1.changeTitle("생일 카드");
card1.changeContent("생일 축하해");
card1.print();

const card2 = createCard();
card2.changeTitle("감사 카드");
card2.changeContent("감사합니다.");
card2.print();
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

### ❏ JS 코드 실행

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

function foo() {
    var x = 10;
    bar();
}

function bar() {
    console.log(x);
}

foo(); // 1
bar(); // 1
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

console.log(callMe()); // undefined

var x = 10;

console.log(callMe()); // 10

function callMe() {
    return x;
}
```

```javascript
// let, const 변수는 생성 단계에서 초기화되지 않는다.
// 선언문 이전에 접근 시 Reference Error가 발생한다.
// 이 경계를 TDZ라고 한다.
// 따라서, let, const는 hoisting이 발생하지 않는다.
// 함수는 생성단계에서 값까지 할당하지만 let, const는 생성단계에서 해당 값 이전에 접근하려고 했기 때문에 TDZ에 의해 참조에러가 난다.

console.log(callMe()); // undefined

var x = 10;

console.log(callMe()); // 10

function callMe() {
    return x;
}
```

```javascript
// varFor에서 i는 varFor 함수 범위에 존재하는 변수이다.
// 따라서, setTimeout이 호출될 때, i는 for 블럭이 끝난 시점에 소멸하지 않는다.
// letFor에서 i는 for 블럭안에 존재하는 변수이다.
// 각 for block이 실행되고 i는 소멸한다. 다만, 이 경우 각 화살표 함수의 closure에 저장된다.

function varFor() {
    for (var i = 0; i < 3; i++) {
        setTimeout(() => console.log(i));
    }
}

function letFor() {
    for (let i = 0; i < 3; i++) {
        setTimeout(() => console.log(i));
    }
}

varFor(); // 3 3 3
letFor(); // 0 1 2
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
window.open(targetURL, "target", windowSize);

// globalThis
const windowSize = `height=${globalThis.innerHeight}, width=${globalThis.innerWidth}`;
globalThis.open(targetURL, "target", windowSize);
```

### ❏ Document

1. 브라우저에 로드된 웹 페이지
2. 문서의 `title`, `URL` 등의 정보를 얻는다.
3. `element` 생성, 검색 등의 기능 제공

```js
function printDocumentInfo() {
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
let bigN = 1000000000000n;

// Math.max, Math.min
function getMaxDiff(nums) {
    return Math.max(...nums) - Math.min(...nums);
}

getMaxDiff([-1, -4, -7, 11]);

// Math.random
function getRandomNumberInRange(min, max) {
    return Math.floor(Math.random() * (max - min + 1)) + min;
}

Array.from({ length: 10 }).map(() => getRandomNumberInRange(50, 100));
```

### ❏ Date

1. 특정 시점의 날짜를 표시하기 위한 객체
2. 날짜와 관련된 작업을 하기 위한 여러 메서드를 포함한다.

```js
// Date.getDay()는 요일을 0(일요일)부터 6(토요일)로 구한다.
// 이 외에 년도, 월, 일, 시, 분, 초, 밀리초 등을 구할 수 있다.
// getMonth(), getDate(), getHour()...

function isWeekend(today) {
    let day = today.getDay();
    return day === 0 || day === 6;
}

console.log(isWeekend(new Date("2021/11/13")));

// setDate()등의 메서드로 시간을 설정한다.
// 설정 시 월 변경 등의 시간 변환은 Date 객체가 처리한다.
// toDateString() 메서드는 특정 포맷의 문자열을 반환한다.

function addDays(date, days) {
    date.setDate(date.getDate() + days);
    return date.toDateString();
}

addDays(new Date("2021/9/22"), 100); // Fri Dec 31 2021

// getTime() 메서드는 시간을 밀리초 단위로 반환한다.
// 이때 밀리초는 1970.1.1 시점부터 흐른 시간이다.
// fromNow는 주어진 시간이 현재로부터 며칠이나 흘렀는지를 계산한다
function timeDiff(date1, date2) {
    return date2.getTime() - date1.getTime();
}

let dayTime = 60 * 24 * 60 * 1000;
function fromNow(date) {
    let diff = timeDiff(date, newDate());
    return `${Math.floor(diff / dayTime)} days ago...`;
}

fromNow(new Date("2021/11/13"));
```

### ❏ String, JSON

1. 문자열 원시 타입의 래퍼객체
2. 문자열을 조작하기 위한 여러 메서드를 포함한다.
3. JSON - JSON 객체와 관련된 메서드를 담은 객체

```js
// toUserList는 이름의 배열을 받아 리스트 태그 목록의 문자열을 계산한다.
function toUserList(users) {
    return users
        .fileter((user) => !user.includes("Admin"))
        .map((user) => user.trim().toUpperCase())
        .map((user) => `<li>${user}</li>`)
        .join("");
}

console.log(toUserList(["TED", "AYW", "AYJ"]));
```

```js
// JSON.stringify는 주어진 객체를 JSON 문자열로 만든다.
JSON.stringify({ name: "TED", age: 27 }); // {"name":"TED","age":27}

// JSON.parse()는 주어진 JSON 문자열을 JS 객체로 만든다.
JSON.parse('{"name":"TED","age":27}'); // { name: 'TED', age: 27 }
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

function foo() {
    console.log("foo");
}

function bar() {
    console.log("bar");
}

foo();
bar();

// 비동기 코드: 동시에 실행되는 특징을 갖고 있다.
setTimeout(() => {
    count++;
}, 3000);

function foo() {
    console.log("foo");
}

function bar() {
    console.log("bar");
}

foo();
bar();
```

### ❏ 콜백함수(call back)

1. 콜백함수란 다른 함수의 인자로써 사용되는 함수를 말한다.
2. 우리가 JS에서 비동기 처리를 수행할 때는 콜백함수를 사용하는데, 콜백함수의 단점은 여러개의 콜백 패턴을 사용할 때 가독성이 떨어지고, 비동기 처리 중 발생한 예외 처리가 곤란하며, 여러개의 비동기 처리를 한 번에 처리할 때 한계가 있다.

```javascript
// 1초가 지나고 undefined가 출력된다.
function findUser(id) {
    let user;

    setTimeout(function () {
        console.log("1초 기다림");
        user = {
            id: id,
        };
    });

    return user;
}

let user = findUser(1);

// 콜백으로 넘겨주기: 1초가 지나고 user에 값이 할당된다.
// 단점: 비동기를 또 넘겨주고 싶을 떄는 콜백지옥에 빠진다.
function findUser(id, callbackFunc) {
    let user;
    setTimeout(function () {
        console.log("1초 기다림");
        user = {
            id: id,
        };

        callbackFunc();
    }, 5000);
    return user;
}

findUser(1, function (user) {
    console.log("user:", user);
});

// 이벤트 핸들링
addEventListener("click", function () {
    console.log("HI");
});
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
    .catch(() => console.log("네트워크 요청 실패"));
```

4. 비동기 코드를 처리하는 모듈은 JS 엔진 외부에 있다.
5. `event queue`, `task queue`, `job queue` 등으로 구성된다.
6. API 모듈은 비동기 요청을 처리 후 태스크 큐에 콜백 함수를 넣는다.
7. JS 엔진은 콜 스택이 비워지면, `event Loop`에서 `task queue`의 콜백 함수를 `call stack`으로 `push`한다.
8. `call stack`에 있는 콜백 함수가 실행된다.

```js
// 비동기 처리가 끝나면 콜백 함수를 task queue로 밀어 넣는다.
request("user-data", (userData) => {
    console.log("userData 로드");
    saveUsers(userData);
});

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
Promise.all([promise1, promise2, promise3])
    .then((values) => {
        console.log("모두 성공", values);
    })
    .catch((e) => {
        console.log("하나라도 실패", values);
    });
```

12. promise를 리턴하는 값이 같으면 `then` 을 생략할 수 있다

```jsx
// 2개의 API에 모두 then을 사용한 방식
promise
    .then((item) => getUserNameById(item.id))
    .then((id) => id)
    .catch((e) => e.message);

// 2개의 API 중 한개만 then을 사용한 방식
promise.then((item) => getUserNameById(item.id)).catch((e) => e.message);
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
9. `fetch`: `fetch(url).then(type => type.json())` : `promise`를 `json`타입으로 바꿔준다.
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
3. 서버로 값을 보낼 때는 `JSON` 형태로 보내고, POST 할 때는 `headers` 설정과 `JSONstringify` 를 사용하기
4. 짝 프로그래밍

```javascript
fetch("/topics", {
    method: "POST",
    body: JSON.stringify({ title: "js", body: "js is .." }),
    headers: {
        "Content-Type": "application/json",
    },
});
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
async function asyncFunc1() {
    let data = await fetchData();
    let user = await fetchUser(data);
    return user;
}

// await 키워드 실행 순서
async function asyncFunc2() {
    let data1 = await fetchData1();
    let data2 = await fetchData2(data1);
    let data3 = await fetchData(data2);
    return data3;
}

function promiseFunc() {
    return fetchData1().then(fetchData2).then(fetchData3);
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
5. REST API 요청 메서드: GET - 리소스 정보를 얻음, POST - 리소스를 생성, PUT - 리소르르 생성하거나 업데이트 DELETE - 리소스를 제거

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
10. response.json(): `body` 정보를 `json` 으로 만드는 `Promise` 를 반환한다.
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

-   품질 담당자가 UI를 사용해 기능 검증
-   사람의 손으로 일일이 테스트한다.(인건비 증가)
-   소프트웨어 회귀(시간에 따라 기능이 많아지면, 추가한 기능과 기존의 기능과의 충돌로 인해 기존의 있던 코드조차 실행이 안되는 현상이 발생한다.)

2. 인수 테스트

-   배치된 시스템을 대상으로 검증
-   전체 시스템 이상 여부 신뢰도가 높음
-   높은 비용(작성 / 관리 / 실행 비용)
-   피드백 품질이 낮음(현상을 드러나지만 원인은 숨겨짐)
-   테스터가 품질 외부를 살펴본다.

3. 자동 테스트

-   기능을 검증하는 코드를 작성
-   테스트 코드 작성 비용이 소비되지만 실행 비용이 낮고 결과의 신뢰도가 높음
-   테스트 코드 작성과 관리가 프로그래머 역량에 크게 영향을 받는다.

4. 단위 테스트

-   시스템 일부(하위 시스템)를 대상으로 검증
-   낮은 비용
-   높은 피드백 품질
-   전체 시스템 이상 여부 신뢰도가 낮음
-   단위끼리 오류가 나는 경우가 있다.
-   테스터가 프로그램의 기능을 살펴본다.

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
let sum = function (a, b) {
    return a + b;
};

function ul(child) {
    return `<ul>${child}</ul>`;
}

// 함수를 리턴할 수 있다.
function makeLi(container, contents) {
    const liList = [];

    for (const content of contents) {
        liList.push(`<li>${content}</li>`);
    }

    return container(liList.join(""));
}

// 함수를 함수의 인자로 넣어줄 수 있다.
const htmlUl = makeLi(ul, ["월", "화", "수", "목", "금", "토", "일"]);
```

3. 함수의 선언문, 선언식

```ts
// 함수 선언문
function sum(a, b) {
    return a + b;
}

// 함수 표현식
const myFunc = function (a, b) {
    return a + b;
};
```

4. 함수의 가변인자

```ts
function sum(a, b) {
    return a + b;
}

const abcSum = sum(10, 20, 30);

// 가변 인자식
function sum() {
    let s = 0;
    for (let i = 0; i < arguments.length; i++) {
        s += arguments[i];
    }
    return s;
}

// arguments
function sum(...args) {
    let s = 0;
    for (let i = 0; i < args.length; i++) {
        s += args[i];
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
(function () {
    console.log(123);
});

// 일반함수와 화살표함수의 차이:  컨텍스트의 차이점
const sumV2 = (a, b, ...args) => {};

const ten = () => 100;
const hundred = (x) => 100 + x;

// 생성기 함수(generate function): 함수를 한번에 실행시키는 것이 아니라 텀을 두고 실행할 때
function* gen() {
    yield 10;
    yield 20;
    return 30;
}

const g = gen();

console.log(g.next()); // 10
console.log(g.next()); // 20
console.log(g.next()); // 30
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
    constructor(name: string) {
        this.name = name;
    }
    say() {
        return `Hello, ${this.name}!`;
    }
}

let person = new Person("AYW");
console.log(person.say());
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

---

## 📍 22일차 11.24.수.(온라인 강의)

오늘은 어제 배웠던 내용을 강의를 통해 다시 한번 배우는 시간을 가졌다. 클린코드, 타입스크립트 정의, `type`, `utility` 등등에 대해서 다시 배워보자.

### ❏ 클린코드란

1. 클린 코드란 말 그대로 깨끗하게 작성된 코드를 의미합니다. 깨끗하게 작성된 코드란 직접적이고 단순하여 읽기가 쉽고, 코드 작성자가 아닌 누가 보더라도 의도가 명확히 드러나는 코드입니다. 이러한 코드는 가독성이 좋고, 의존성을 최대한 줄여 유지보수가 쉬운 특징이 있습니다.
2. 프로그래머는 작성 기한을 맞추기 위해서 나쁜 코드를 양산할 수밖에 없다고 생각합니다. 하지만 나쁜 코드를 양산하면 결국 기한을 맞추지 못합니다. 오히려 엉망진창인 코드 때문에 개발 속도가 느려지고 결국 기한을 놓칩니다. 기한을 맞추는 유일한 방법은 언제나 코드를 최대한 깨끗하게 유지하는 것입니다.

### ❏ 클린코드와 타입스크립트

1. 자바스크립트는 타입이 없기 때문에 실행 후에 타입 에러를 확인할 수 있습니다. 반면 타입스크립트는 같은 코드에 대해 아래와 같이 실행을 하기 전에, 미리 에러를 확인할 수 있습니다. 자바스크립트의 런타임 단계에서 발생하는 타입 에러를 타입스크립트에서는 컴파일 단계에서 미리 확인하고 고칠 수 있다. 만약, 런타임 단계에서 발생하는 에러로 인해 프로그램이 멈추면, 운영되는 서비스에 큰 차질이 생길 수 있다. 타입스크립트를 사용하면 에러를 미리 방지할 수 있다.
2. 타입을 정의함으로써 개발자의 실수를 줄일 수 있고, 명시된 타입을 보고 해당 변수의 자료형이 무엇인지 쉽게 이해할 수 있다. 결과적으로 어던 용도로 코드가 작성되었고, 무엇을 의미하는지 파악하기 훨씬 용이하기 때문에 유지보수에 유리하고 자연스럽게 개발 속도도 빨라지게 된다.

### ❏ 타입스크립트란?

1. `microsoft` 에서 개발한 오픈 소스 언어
2. 자바스크립트의 상위 집합, JS의 한계를 해결
3. 타입스크립트를 실행하려면 자바스크립트로 변환하는 컴파일과정이 필요하다.
4. 동적타입을 정적으로 사용가능
5. 타입 유추로 타입 제어 가능
6. 컴파일 시점에 오류 포착 가능
7. JS에서 찾을 수 없는 추가코드 기능 제공

```typescript
// JS
let a;
a = 1;
a = "b";

const sum = (a, b) => {
    return a + b;
};

sum(1, "2"); // 12

// TS
let a: number;
a = 1;
b = "b"; // Error(컴파일 시점)

const sum = (a: number, b: number) => {
    return a + b;
};

sum(1, 2); // 12
```

### ❏ 타입스크립트의 기본 Type

1. JS코드에 변수 함수 등의 type 정의 가능
2. 타입 표기(type annotation)을 사용한다.
3. 기본자료형(primitive type): `string`, `boolean`, `number`, `null`, `undefined`, `symbol(ES6)`

```typescript
// string
let str: string = "hi";

// boolean
let isSucceeded: boolean = true;

// number: 2진수, 8진수, 10진수, 16진수 사용 가능
let decimal: number = 6;
let hex: number = 0xf00d;
let binary: number = 0b1010;
let octal: number = 0o744;

console.log(decimal, hex, binary, octal); // 6 61453 10 484

// null
let n: null = null;

// undefined
let u: undefined = undefined;
```

4. 참조자료형(reference type): object, array, function

```typescript
// 객체, 배열, 함수 등과 같은 Object 형식의 타입, 메모리에 값을 주소로 저장하고, 출력시 메모리 주소와 일치하는 값을 출력
// object
function create(o: object): void {}

create({ prop: 0 }); // object
create([1, 2, 3]); // array
create("string"); // error
create(false); // error
create(42); // error

// array
let arr1: number[] = [1, 2, 3];
let arr2: Array<number> = [1, 2, 33];
```

5. 추가 제공 자료형: tuple, enum, any, void, never

```typescript
// tuple: 길이와 각 요소의 타입이 정해진 배열을 저장하는 타입
let arr: [string, number] = ["Hi", 122];
arr[1].concat("1")  // Error: 'number' does not have 'concat'
arr[3] = "hello"  // Error: Property '3' does not exist on type [string, number]

// enum: 특정 값들의 집합을 저장하는 타입
enum Car {BUS, TAXI, SUV};
let bus: Car = Car.BUS;
let taxi: string = Car[2];

console.log(bus, taxi)
👉🏽 0 "SUV"

enum Car {BUS = 2, TAXI, SUV};
let bus: Car = Car.BUS;
let taxi: string = Car[3];

console.log(bus, taxi)
👉🏽 2 "TAXI"

// any: 모든 타입 저장 가능, 컴파일 중 타입 검사를 하지 않음
let str: any = "hi";
let num: any = 1;
let arr: any = [1, 2, 3];

// void: 보통 함수에서 반환 값이 없을 때 설정하는 타입
let unknown: void = undefined;
function sayHi(): void {
  console.log("hi")
}

// never: 절대 발생할 수 없는 타입, 종료되지 않는 함수, 항상 오류를 발생시키는 함수
function neverEnd():never {
  while(true){}
}

function neverEnd():never {  // Error: A function returning 'never' cannot have a reachable end point.
  while(true){break}
}

function error(message: string):never{
  throw new Error(message)
}
```

### ❏ 타입스크립트의 Utility

1. Typescript는 공통 타입 변환을 용이하게 하기 위해 유틸리티 타입을 제공한다.
2. 유틸리티 타입은 전역으로 사용 가능하다
3. `Partial<T>`, `Readonly<T>`, `Record<T>`, `Pick<T, K>`, `Omit<T, K>`, `Exclude<T, U>`. `Extract<T, U>`, `NonNullable<T>`, `Parameters<T>` , `ConstructorParameters<T>`, `ReturnType<T>`, `Required<T>`
4. 제네릭이란 어떤 함수나 클래스가 사용할 타입을 생성 단계가 아닌 사용 단계에서 정의하는 프로그래밍 기법입니다.

```typescript
// Partial<T>: 프로퍼티를 선택적으로 만드는 타입을 구성한다.
interface Todo {
  title: string;
  description: string;
}

function updateTodo(todo: Todo, fieldsToUpdate: Partial<Todo>){
  return {...todo, ...fieldsToUpdate}
}

const todo1: Todo = {
  title: 'organize desk',
  description: 'clear clutter'
}

const todo2 = updateTodo(todo1, {description: 'throw out trash'})

console.log(todo1, todo2)
👉🏽 { title: 'organize desk', description: 'clear clutter' } { title: 'organize desk', description: 'throw out trash' }

// Readonly<T>: 프로퍼티를 읽기 전용으로 설정한다.
interface Todo {
  title: string;
}

const todo1: Readonly<Todo> = {
  title: 'organize desk',
}

todo1.title = "Hello" // Error: Cannot assign to 'title' because it is a read-only property.

// Record<T>: 프로퍼티의 집합 K로 타입을 구성한다. 타입의 프로퍼티들을 다른 타입에 매핑시키는데 사용한다.
interface PageInfo {
  title: string;
}

type Page = "home" | "about" | "contact";

const x: Record<Page, PageInfo> = {
  about: {title: 'about'},
  contact: {title: 'contact'},
  home: {subTitle: 'home'}  // Error: Type '{ subTitle: string; }' is not assignable to type 'PageInfo'.  Object literal may only specify known properties, and 'subTitle' does not exist in type 'PageInfo'
}

// Pick<T, K>: 프로퍼티 K의 집합을 선택해 타입을 구성한다.
interface Todo {
  title: string;
  description: string;
  completed: boolean
}

type TodoPreview = Pick<Todo, "title" | "completed">;

const todo: TodoPreview = {
  title: 'clean room',
  completed: true,
  description: 'desc'  // Error: Type '{ title: string; completed: true; description: string; }' is not assignable to type 'TodoPreview'. Object literal may only specify known properties, and 'description' does not exist in type 'TodoPreview'
}

// Omit<T, K>: 모든 프로퍼티를 선택한 다음 K를 제거한 타입을 구성한다.
interface Todo {
  title: string;
  description: string;
  completed: boolean
}

type TodoPreview = Omit<Todo, "description">;

const todo: TodoPreview = {
  title: 'clean room',
  completed: true,
  description: 'desc'  // Error: Type '{ title: string; completed: true; description: string; }' is not assignable to type 'TodoPreview'.
}

// Exclude<T, U> : 타입 T에서 U와 겹치는 타입을 제외한 타입을 구성합니다.
// Extract<T, U> : 타입 T에서 U와 겹치는 타입만 포함하여 타입을 구성합니다.
// NonNllable<T> : T 타입에서 null과 undefined를 제외한 타입을 구성합니다.
// Parameter<T> : 함수 타입 T의 매개변수의 타입들의 튜플로 타입을 구성합니다.
// ConstructorParameters<T> : 클래스의 생성자를 비롯한 생성자 타입의 모든 매개변수 타입을 추출합니다.
// ReturnType<T> : 함수 T가 반환한 타입으로 타입을 구성합니다.
// Required<T> : 타입 T의 모든 프로퍼티가 필수로 설정된 타입을 구성합니다.
```

### ❏ 함수 사용하기

1. 함수를 정의 할 때 사용되는 변수는 매개변수이고 호출 할 때 사용되는 값은 인수라고 한다.

```typescript
function add(x, y) {
    // 매개변수
    return x + y;
}

add(2, 5); // 인수
```

2. 일급객체(first-class object): 다른 객체들에 일반적으로 적용 가능한 연산을 모두 지원하는 객체

```typescript
1. 다른 함수에 매개변수로 제공할 수 있다.
2. 함수에서 반환이 가능하다
3. 변수에 함수를 할당할 수 있다.
```

3. 함수 선언식, 함수 표현식

```typescript
// 함수 선언식
function world(name) {}

// 함수 표현식
const hi = function (name) {};

// 함수 생성자는 되도록 사용을 권하지 않는다
let world5 = new Function();
```

4. `TS` 에서 함수 작성시 반환 타입을 추론하도록 하는걸 권장한다.
5. `TS` 컴파일러는 방정식의 한쪽에만 타입이 있어도 타입추론이 가능한데, 이를 `contextual typing` 이라고 부른다. 이를 통해 프로그램에서 타입을 유지하기 위한 노력을 줄일 수 있다.

### ❏ 함수의 매개변수

1. 기본 매개변수: 함수에 주어진 인자의 수는 함수가 기대하는 매개변수의 수와 일치해야 한다.

```typescript
function buildName(firstName: string, lastName: string) {
    return firstName + lastName;
}

let result1 = buildName("a", "b");
let result2 = buildName("a", "b", "c"); // Error: Expected 2 arguments, but got 3.
```

2. 선택적 매개변수: `JS` 에서는 인수가 없으면 `undefined` 로 선언이된다. `TS` 에서는 변수명 뒤에 `?` 를 사용하면 변수를 선택적으로 사용할 수 있다.
3. 기본-초기화 매개변수: `TS` 에서 값을 제공하지 않거나, `undefined` 로 했을 때 매개변수의 값 할당 가능

```typescript
function buildName(firstName: string, lastName: string = "TED") {
    return firstName + lastName;
}

let result1 = buildName("a"); // aTED
let result1 = buildName("a", undefined); // aTED
let result1 = buildName("a", "morning"); // amorning
```

4. 나머지 매개변수: `...` 을 넣어주어 매개변수의 수를 무한으로 취급할 수 있다. 아무것도 넘겨주지 않으면 `[]` 이 할당된다.

```typescript
function buildName(firstName: string, ...lastName: string[]) {
    return firstName + lastName;
}

let result1 = buildName("a", "SON", "Ted"); // aSON,Ted
```

### ❏ OOP

1. 객체 지향 프로그래밍: 컴퓨터 프로그램을 객체의 모임으로 파악하려는 프로그래밍 패러다임이다. 객체들은 서로 메세지를 주고 받으며 데이터를 처리할 수 있다.
2. 장점: 프로그램을 유연하고, 변경이 용이하게 만들어지며, 개발과 보수를 간편하게 만든다, 직관적인 코드 분석을 가능하게 한다.
3. 중요한 특성: 강한 응집력과 약한 결합력을 지향한다.

### ❏ Class

1. 클래스의 요소: 멤버, 필드, 생성자, 메소드
2. 인스턴스: `new` 연산자에 의해 생성된 객체

```typescript
class Person {
    name: string;
    constructor(name: string) {
        this.name = name;
    }

    say() {
        return "Hello, My name is " + this.name;
    }
}

let person = new Person("TED");
console.log(person); // Person { name: 'TED' }
```

### ❏ Class 접근 제어자

1. 속성, 메소드로의 접근을 제한하기 위해 사용한다.
2. `public`, `protected`, `private`
3. `Java` 와 다르게 `package` 개념이 없어 `default` 접근 제어자는 없다.
4. `public`: 프로그램 내 선언된 멤버들이 자유롭게 접근할 수 있다. 기본적으로 `public` 으로 선언된다. 명시적으로 `public` 선언도 가능하다.

```typescript
class Person {
    public name: string;
    constructor(name: string) {
        this.name = name;
    }
}

let a = new Person("TED").name;
console.log(a); // TED
```

5. `private` :멤버가 포함된 클래스 외부에서 접근을 막는다.

```typescript
class Person {
    private name: string;
    constructor(name: string) {
        this.name = name;
    }
}

new Person("TED").name; // Error: Property 'name' is private and only accessible within class 'Person'.
```

6. `protected`: 멤버가 포함될 클래스와 그 하위 클래스 외부에서의 접근을 막는다. (내부에서는 접근이 가능하지만, 외부에서의 접근은 불가하다)

```typescript
class Person {
    protected name: string;
    constructor(name: string) {
        this.name = name;
    }
}

class Employee extends Person {
    private department: string;

    constructor(name: string, department: string) {
        super(name);
        this.department = department;
    }

    public getElevatorPitch() {
        return `good.`;
    }
}

let howard = new Employee("Howard", "sales");
console.log(howard.name); // Error: Property 'name' is protected and only accessible within class 'Person' and its subclasses.
```

### ❏ Class 상속

1. 상속을 이용하여 존재하는 클래스를 확장해 새로운 클래스를 생성할 수 있다. `extends`
2. 파생된 클래스는 하위클래스(subclass), 기초 클래스는 상위 클래스(super class)라고 부른다.

```typescript
class Animal {
    move(distanceInMeters: number) {
        console.log(`Animal moved ${distanceInMeters}m.`);
    }
}

class Dog extends Animal {
    makeSound() {
        console.log(`멍멍`);
    }
}

const dog = new Dog();
dog.move(10);
```

### ❏ Getters & Setters

1. 비공개로 설정하려는 속성은 `private` 로 설정하고, 속성값을 읽고 수정하는 `getter/setter` 함수를 사용한다.
2. `class` 에 직접 적용하는것을 막고, 함수를 사용해 값을 받아오거나 수정한다. 속성에 직접 접근해 수정하면 데이터 무결성이 깨질 수 있다. (캡슐화 권장)
3. 각 객체의 멤버에 접근하는 방법을 세밀하게 제어할 수 있다.

```typescript
class Person {
    private _name: string;

    get name() {
        return this._name;
    }

    set name(name: string) {
        if (name.length > 10) {
            throw new Error("name too long");
        }
        this._name = name;
    }
}

let person = new Person();
console.log(person.name); // undefined

person.name = "TED";
console.log(person.name); // TED

person.name = "TEDTEDTEDTEDTED"; // throw Error
```

### ❏ Readonly

1. 읽기만 가능한 속성을 선언하기 위해 사용한다. (변경 할 수 없다.)
2. 선언될 때나 생성자에서 값을 설정하면 이후 수정할 수 없다.

```typescript
class Person {
    readonly age: number = 20;
    constructor(age: number) {
        this.age = age;
    }
}

let person = new Person(10);
person.age = 30; // Error: Cannot assign to 'age' because it is a read-only property
```

### ❏ static

1. 전역 멤버를 선언할 때 사용한다. (전역멤버: 객체마다 할당되지 않고, 클래스의 모든 객체가 공유하는 멤버)
2. 인스턴스가 아닌 클래스 자체에서 보이는 전역 멤버를 생성한다.
3. 범용적으로 사용되는 값에 설정한다.
4. `클래스명.` 을 앞에 붙여 `static` 멤버에 접근할 수 있다.
5. `ES6` 에서 메소드 전용 속성에는 선언이 안되었으나, `TS` 에서는 사용가능하다.

```typescript
class Grid {
    static origin = { x: 0, y: 0 };
    calculateDistanceFromOrigin(point: { x: number; y: number }) {
        let xDist = point.x - Grid.origin.x;
        let yDist = point.y - Grid.origin.y;
        return Math.sqrt(xDist * xDist + yDist * yDist) / this.scale;
    }
    constructor(public scale: number) {}
}

let grid1 = new Grid(1.0); // 1x scale
let grid2 = new Grid(5.0); // 5x scale

console.log(grid1.calculateDistanceFromOrigin({ x: 10, y: 10 })); // 14.142135623730951
console.log(grid2.calculateDistanceFromOrigin({ x: 10, y: 10 })); // 2.8284271247461903
```

### ❏ 추상클래스

1. 다른 클래스들이 파생될 수 있는 기초클래스
2. 직접 인스턴스화 될 수 없다.
3. `abstract` 키워드는 추상 클래스나 추상 메소드를 정의하는데 사용된다.
4. 추상 메소드는 클래스에는 구현되어 있지 않고, 파생된 자식 클래스에서 구현해야 한다.

```typescript
abstract class Animal {
    protected name: string;

    constructor(name: string) {
        this.name = name;
    }

    abstract makeSound(): void;
    move(): void {
        console.log("move !!");
    }
}

class Dog extends Animal {
    constructor(name: string) {
        super(name); // 파생된 클래스의 생성자는 반드시 super()를 호출
    }

    makeSound(): void {
        console.log(this.name + "멍멍");
    }
}

const animal = new Animal("animal"); // Error: Cannot create an instance of an abstract class.
const dog = new Dog("진돗개"); // Dog { name: '진돗개' }
```

### 💡 추상 클래스를 활용한 디자인 패턴

1. 프로그램의 일부분을 서브 클래스로 캡슐화해 전체 구조를 바꾸지 않고 특정 단계의 기능을 바꾸는 것
2. 전체적인 알고리즘은 상위 클래스에서 구현하고, 다른 부분은 하위 클래스에서 구현한다.
3. 전체 구조는 유사하지만, 부분적으로 다른 구문에서 작성된 메소드의 코드 중복을 최소화 할 수 있다.

```typescript
abstract class Parent {
  public do(){
    console.log("Parent에서 실행 - 상") ;
    this.hook();
    console.log("Parent에서 실행 - 하");
  }

  abstract hook(): void;
}

class Child extends Parent {
  hook(): void {
    console.log("child")
  }
}

const child = new Child();
child.do();

👉🏽
Parent에서 실행 - 상
child
Parent에서 실행 - 하
```

---

## 📍 23일차 11.25.목(실시간 강의)

오늘은 `interface`, `generic` 문법에 대해서 배웠다.

### ❏ Interface

1. 타입 체크를 위해 사용되며 변수, 함수, 클래스에 사용 가능
2. 직접 인스턴스를 생성할 수 없음. 모든 메소드는 추상 메소드다. (이때 `abstract` 키워드를 사용하지 않는다)
3. 선언만 존재한다. (JS로 변환되면 인터페이서는 사라진다.)
4. `interface` 간에 `extends` 를 사용하여 다중 상속 가능(class와 비슷)
5. 추상 클래스와 다른점: 추상 `class`는 전체적인 구조, `interface`는 프로그래머 간의 협업 개발을 할 때 사용
6. 함수의 매개변수(파라미터로)로 사용
7. `API` 응답에서 데이터의 구조를 결정할 때 사용

```typescript
// 키 값을 다음처럼 정해주면 키 값은 제한이 없다.
interface User {
    [grade: number]: "A" | "B" | "C" | "D";
}

let user: User = {
    1: "A",
    2: "B",
    5: "D",
};
```

8. 선택적 프로퍼티(?): `?`가 붙는 경우는 반드시 구현되지 않고 선택가능

```typescript
// 키 값을 다음처럼 정해주면 키 값은 제한이 없다.
interface User {
    1: string;
    2?: string;
    5: string;
}

let user: User = {
    1: "A",
    5: "D",
};
```

9. 클래스 선언문의 `implements` 를 붙여서 사용 가능(인터페이스를 구현하는 클래스의 일관성을 유지할 수 있는 장점을 가짐)

```typescript
// 모든 메소드는 추상 메소드여야 한다.
// 인터페이스에서 정의한 타입은 클래스 안에서도 모두 적용해야한다.
interface ITodo {
    id: number;
    content: string;
    completed: boolean;
    sayHello(): void;
}

class Todo implements ITodo {
    constructor(
        public id: number,
        public content: string,
        public completed: boolean
    ) {}

    sayHello() {
        console.log(`안녕하세요!!`);
    }
}

const today = new Todo(1, "TED", true); // 인스턴스
console.log(today); // Todo { id: 1, content: 'TED', completed: true }
today.sayHello(); // 안녕하세요!!
```

9. 함수와 변수에서도 덕타입이 적용된다.(덕 타이핑: 타입 체크에서 중요한 것은 값을 실제 가지고 있느냐에 관한 것, 인터페이스에서 정의한 프로퍼티나 메소드를 가지고 있다면 그 인터페이스를 구현한 것으로 여김 덕 타이핑 또는 구조적타이핑이라 부름)

```typescript
type IPerson = {
    name: string;
};

function sayHello(person: IPerson): void {
    console.log(`Hello ${person.name}`);
}

const me = { name: "TED", age: 27 };
sayHello(me);
```

### ❏ 디자인패턴

1. 생성패턴: 객체를 생성하는데 관련한 패턴
2. 구조패턴: 프로그램의 구조에 관련한 패턴
3. 행위패턴: 반복적으로 사용되는 객체들의 상호작용 패턴

```typescript
// 전략 패턴
interface Weapon {
    attack: () => void;
}

class Sword implements Weapon {
    public attack() {
        console.log("검 공격");
    }
}

class Spear implements Weapon {
    public attack() {
        console.log("창 공격");
    }
}

class Bow implements Weapon {
    public attack() {
        console.log("활 공격");
    }
}

class GameUser {
    private weapon: Weapon | null = null;

    public setWeapon(weapon: Weapon) {
        this.weapon = weapon;
    }

    public attack() {
        if (this.weapon === null) {
            console.log("맨손 공격");
        } else {
            this.weapon.attack();
        }
    }
}

const testUser = new GameUser();
testUser.setWeapon(new Spear());
testUser.attack(); // 창

testUser.setWeapon(new Bow());
testUser.attack(); // 활 공격

testUser.setWeapon(new Sword());
testUser.attack(); // 검 공격

testUser.setWeapon(null);
testUser.attack(); // 맨손 공격
```

### ❏ 제네릭(Generic)

1. 데이터타입을 일반화 함
2. 자료형을 정하지 않고 여러 타입을 사용할 수 있게 한다.(범용적인 함수를 쓰고 싶을 때?, 여러가지 타입을 사용하고 싶을 때)
3. 재사용성이 높은 함수를 만들어줄때 사용됨
4. 한가지 타입보다 여러가지 타입에서 동작하는 함수를 생성한다.

```typescript
// class 문법에서의 제네릭
class Stack<T> {
    private data: T[] = [];

    constructor() {}

    push(item: T): void {
        this.data.push(item);
    }

    pop(): T | undefined {
        return this.data.pop();
    }
}

// 인스턴스의 타입을 유연하게 설정할 수 있다.
const numberStack = new Stack<number>();
const stringStack = new Stack<string>();
numberStack.push(1);
stringStack.push("a");

// 함수에서의 제네릭
function getSize<T>(arr: T[]): number {
    return arr.length;
}

const arr1 = [1, 2, 3];
getSize<number>(arr1);

const arr2 = ["a", "b", "c"];
getSize<string>(arr2);
```

5. 제네릭한 변수를 추가하고 싶을 때 `<T, U>`

```typescript
// 1
function toPair<T, U>(a: T, b: U): [T, U] {
    return [a, b];
}

toPair<number, string>(1, "1");
toPair<string, boolean>("Hello", true);

// 2
function logText<T>(text: T[]): number {
    return text.length;
}

// 3
interface Mobile<T> {
    name: string;
    price: number;
    option: T;
}

let myInfo: Mobile<boolean> = {
    name: "TED",
    price: 6000,
    option: true,
};

let yourInfo: Mobile<object> = {
    name: "TED",
    price: 6000,
    option: {
        age: 28,
        color: "orange",
    },
};

// 함수에서의 제네릭
// <T>는 text의 인자는 T로 받고 리턴값도 T 타입으로 해준다.
interface GenericLogTextFn {
    <T>(text: T): T;
}

interface GenericLogTextFn<T> {
    (text: T): T;
}

function logText<T>(text: T): T {
    return text;
}

let myString: GenericLogTextFn<string> = logText;
console.log(myString);

interface Mobile<T> {
    name: string;
    price: number;
    option: T;
}

interface OptionType {
    color: string;
    coupon: boolean;
}

const m1: Mobile<OptionType> = {
    name: "s21",
    price: 1000,
    option: { color: "red", coupon: false },
};

// 제네릭 상속
interface User {
    name: string;
    age: number;
}

interface Book {
    price: number;
}

let user: User = { name: "a", age: 10 };
let book: Book = { price: 3000 };

function showName<T extends { name: string }>(data: T) {
    return data.name;
}
```

### ❏ Non-null assertion operator

1. `Null` 이 아닌 어선셜 연산자는 피연산자가 `null` 이 아니라고 컴파일러에게 전달하여 일시적으로 `Null` 제약조건을 완화합니다. 권장하지 않는 문법이고 대신 `&&` 을 사용한다.

### ❏ Union type

```typescript
// example1
function getAge(age: number | string) {
    return typeof age === "number" ? age.toFixed() : age;
}

const myAge = getAge(28);
console.log(myAge);

const yourAge = getAge("25");
console.log(yourAge);

// union 기호
interface Person {
    name: string;
    age: number;
}

interface Developer {
    name: string;
    skill: string;
}

// 겹치는 속성만 사용 가능
function introduce(someone: Person | Developer) {
    someone.name;
    someone.age; // Error
    someone.skill; // Error
}

// 모든 속성 사용 가능
function introduce(someone: Person & Developer) {
    someone.name;
    someone.age; // 사용 가능
    someone.skill; // 사용 가능
}
```

### ❏ 제약 조건(constraints / keyof)

1. 제네릭 타입에 어느정도 힌트를 주고 제약을 걸기 위해 사용, 최소한 `length` 속성이 있어야 에러가 나지 않는다

```typescript
interface LengthWise {
  length: number;
}

interface Rect {
  length: number;
  area: number;
}

function logText1<T extends LengthWise | Rect>(text: T){
  console.log(text.length);
  console.log(text.area);  // 공통되는 속성이 아니므로 Error가 난다.
}

function logText1<T extends LengthWise & Rect>(text: T){
  console.log(text.length);
  console.log(text.area);  // 모든 속성 사용 가능하므로 Error가 나지 않는다.
```

### ❏ keyof를 사용한 제약

1. 객체의 속성을 제약하고 싶을 때 사용

```typescript
// 객체 안에서의 속성만 사용하는 문법
function getProperty<T, O extends keyof T>(obj: T, key: O) {
    return obj[key];
}

let obj = { a: 1, b: 2, c: 3 };
// 'a' | 'b' | 'c'
console.log(getProperty(obj, "c"));
```

### ❏ 기타 기능 및 개념

1. Type Assertion: 타입 추론기능은 강력하지만 한계 존재, 타입단언(type assertion)은 타입스크립트가 추정하지 못하는 부분까지 개발자가 선언하는것
2. as

```typescript
let a;
a = 10;
a = "abc";
let b = a;

b = a as string;

interface Person {
    name: string;
    age: number;
}

interface Developer {
    name: string;
    skill: string;
}

function introduce(someone: Person | Developer) {
    someone.name;
    (someone as Person).age;
    (someone as Developer).skill;
}
```

3. typeGuard

```typescript
// 함수
function doSomeThing(id: string | number) {
    if (typeof id === "string") {
        console.log(id.trim());
    } else {
        console.log(id);
    }
}

// 클래스
class Diner {}
class Merchant {}

function doSomething(user: Diner | Merchant) {
    if (user instanceof Diner) {
    } else {
    }
}

// 메소드
interface Bird {
    fly(): string;
}

interface Fish {
    swim(): number;
}

function doSomething(animal: Fish | Bird) {
    if ("swim" in animal) {
        console.log((animal as Fish).swim());
    } else {
        console.log((animal as Bird).fly());
    }
}

doSomething({
    swim: () => {
        return 82;
    },
});

doSomething({
    fly: () => {
        return "Hello";
    },
});

// 타입 확인
function isFish(animal: Fish | Bird): animal is Fish {
    return (animal as Fish).swim !== undefined;
}

function doSomething(animal: Fish | Bird) {
    if (isFish(animal)) {
        animal.swim();
    } else {
        animal.fly();
    }
}
```

### ❏ 실습

1. 클래스 vs 추상클래스: 어떤 메서드는 그냥 구현해도 되고, 어떤 메서드는 정의 되지 않은 메서드 일 수 있다.(사용하려면 상속이 필요하다)
2. 인터페이스: 추상클래스와 달리 `abstract` 를 사용하지 않음. 구성되는 것의 타입만 명시해서(생성자나 메서드 구현을 작성할 필요가 없다.) (하나의 interface에 여러 데이터가 뭉치지 않도록 분산시킬 수 있기 때문에 다중상속이 가능하다.)
3. `interface` vs `type` vs `abstract`

```typescript
// 인터페이스: 상속이 가능하며, 다중 상속도 가능하다. 내부에서 메서드 구현을 할 수 없다.
interface Test {
	name: string;
	id: number;
	introduce(): void;
}

// 상속이 불가능하다. 내부에서 메서드 구현을 할 수 없다.
type Test {
	name: string;
	id: number;
	introduce(): void;
}

// 클래스이기 대문에 상속은 가능하지만, 다중 상속은 불가하다. 원하는 메서드는 구현을 할 수 있다.
abstract class Test {
	name: string;
	id: number;
  abstractintroduce(): void;
}
```

4. `T extends number | string` : 2개 이상 상속이 가능함.
5. `interface` 활용 예시: 데이터베이스 조작(로그인, 게시물, 등등)
6. ORM: SQL문을 대신해서 내가 알고있는 프로그래밍 언어로 DB로 조작하는 방법(나중에 SQL문으로 변환된다)

### ❏ Generic

1. 선언한 시점에 타입을 사용하는것이 아니라 사용 할 때 모든 타입을 마음대로 넣을 수 있다.
2. 타입에 제한을 걸기 위해 `<T extends string | number>` 처럼 사용할 수 있다.

### ❏ 자바스크립트의 동적인 타입 예시

1. `true == "true"`: `false` abstract equality composition (피연산자에 `number` 씌우고 비교한다)
2. `010-03=5`, 0붙어서 8진수가 된다. (16진수는 ox, 2진수는 ob)
3. `1+'1' = '11'`(`+` 는 문자열 우선순위), `11-'1' = 10`(`-` 는 `Number`만 지원한다.)
4. `0/0=NaN` , 숫자로 취급하지 않는다.
5. `1 / 0 > 10 * 1000 = true` : True, infinity는 표현 범위를 넘어서면 취급한다
6. `true++=>Error` : 값에다가 붙이는게 아니라 변수에다 선언해야한다.
7. `1+2+"3" = 33`

---

## 📍 24일차 11.26.금(온라인 강의)

오늘은 `interface`와 `generic`에 대한 개념을 강의로 배웠다.

### ❏ Interface란?

1. 일반적으로 변수, 함수, 클래스에 타입 체크를 위해 사용된다.
2. 직접 인스턴스를 생성할 수 없고, 모든 메소드가 추상 메소드이다.
3. 추상 클래스의 추상 메소드와 달리 `abstract` 키워드는 사용할 수 없다.
4. `ES6` 는 인터페이스를 지원하지 않지만, `Typescript` 는 인터페이스를 지원한다.
5. 정의한 프로퍼티 값을 누락하거나, 정의하지 않는 값을 인수로 전달하면 컴파일시 에러가 발생한다.

### ❏ interface를 사용하는 이유

1. 타입의 이름을 짓고 코드 안의 계약을 정의한다.
2. 프로젝트 외부에서 사용하는 코드의 계약을 정의하는 강력한 방법이다.

```typescript
interface Person {
    name: string;
}

function sayName(obj: Person) {
    console.log(obj.name);
}

let person = { name: "june" };
sayName(person);
```

### ❏ Properties

1. 컴파일러는 프로퍼티의 두 가지 요소를 검사한다. (필수요소 프로퍼티의 유무, 프로퍼티 타입)
2. 아래 예약어로 프로퍼티를 세밀하게 컨트롤 할 수 있다.(?, readonly)

### ❏ Optional Properties

1. 프로퍼티 선언 시 이름 끝에 `?` 를 붙여 표시한다.
2. 인터페이스에 속하지 않는 프로퍼티의 사용을 방지하면서, 사용 가능한 프로퍼티를 기술할 때 사용한다.
3. 객체 안의 몇 개의 프로퍼티만 채워 함수에 전달하는 `option bags` 같은 패턴에 유용하다.

### ❏ Readonly Properties

1. 객체가 처음 생성될 때만 값 설정이 가능하고, 이후 수정이 불가능하다.
2. 프로퍼티 이름 앞에 `readonly` 를 붙여 사용한다.

```typescript
interface Point {
    readonly x: number;
    readonly y: number;
}

let point: Point = { x: 10, y: 20 };
point.x = 5; // Error: Cannot assign to 'x' because it is a read-only property.
```

3. readonly 와 const 의 공통점: 생성 후 배열을 변경하지 않음을 보장한다. 변수에는 const, 프로퍼티에는 readonly 를 사용한다.

### ❏ interface Type

1. TS에서 인터페이스는 함수, 클래스에서 사용할 수 있다.

```typescript
// function type: 함수의 인자 타입, 반환값 타입 정의
interface CountStar {
    (star: string[]): number;
}

const myStars = ["*", "*", "*"];

const getCountStar: CountStar = (stars) => {
    return stars.length;
};

console.log(getCountStar(myStars));

// class type: 클래스가 특정 계약을 충족하도록 명시적으로 강제한다.
interface Animal {
    makeSound(): void;
}

class Dog implements Animal {
    makeSound(): void {
        console.log("멍멍");
    }
}
```

2. 인터페이스와 클래스는 인터페이스간의 확장이 가능하다.

```typescript
interface Animal {
    makeSound(): void;
}

interface Dog extends Animal {
    speed: number;
}

class Bulldog implements Dog {
    makeSound(): void {
        console.log("멍멍");
    }
}
```

3. hybrid type: JS 의 클로저를 TS 로 구현한 문법

```typescript
interface Counter {
    (start: number): string;
    interval: number;
    reset(): void;
}

function getCounter(): Counter {
    let counter = function (start: number) {} as Counter;
    counter.interval = 123;
    counter.reset = function () {};
    return counter;
}

let c = getCounter();
c(10);
c.reset();
c.interval = 5.0;
```

### ❏ 디자인패턴

1. 객체가 할 수 있는 행위들을 전략으로 만들어두고, 동적으로 행위의 수정이 필요한 경우 전략을 바꾸는 것만으로 수정이 가능하도록 만든 패턴이다.
2. 하단의 코드를 살펴보면 메소드를 직접 변경하는것이 아니라 새로운 `interface` 를 생성하고 해당 `interface` 를 적용하면 `Pay` 메소드를 구현할 수 있다.

### ❏ 제네릭이란?

1. 정적 `type` 언어는 클래스나 함수를 정의 할 때 `type` 을 선언해야 한다.
2. `Generic` 은 코드를 작성할 때가 아니라 코드가 수행될 때 타입을 명시한다. 코드를 작성할 때 식별자를 써서 아직 정해지지 않은 타입을 표시한다. (일반적인 식별자는 `T`, `U`, `V` 를 사용한다.)

### ❏ 제네릭을 사용하는 이유

1. 재 사용성이 높은 함수와 클래스를 생성할 수 있다.(여러 타입에서 동작가능, 코드의 가독성 향상)
2. 예상치 못한 오류를 쉽게 포착한다. (`any` : 타입을 체크하지 않아 관련 메소드의 힌트를 얻지 못한다. 컴파일 시 컴파일러가 오류를 찾지 못한다.)
3. `Generic` 은 타입을 체크해 컴파일러가 오류를 찾을 수 있다.
4. `any` 를 지양하고 다양한 타입을 사용하려면 `Generic` 혹은 `Union` 문법을 권장한다.

### ❏ Generic으로 함수와 클래스 만들기

```typescript
// function
function sort<T>(items: T[]) {
    return items.sort();
}

const numbers: number[] = [1, 3, 2];
const strings: string[] = ["a", "b", "c"];

sort<number>(numbers);
sort<string>(strings);

// class
// stack
class Stack<T> {
    protected data: T[] = [];

    push(item: T) {
        this.data.push(item);
    }

    pop(): T | undefined {
        return this.data.pop();
    }
}

const stack = new Stack();
console.log(stack);
stack.push(1);
stack.pop();

// queue
class Queue<T> {
    private data: Array<T> = [];
    // 제네릭을 활용하여 push()와 pop() 메소드를 구현해주세요.
    push(item: T) {
        this.data.push(item);
    }

    pop(): T | undefined {
        return this.data.pop();
    }
}

const numberQueue = new Queue<number>(); // nunberQueue안에 구성된 타입은 number 형이다.

numberQueue.push(0);
console.log(numberQueue.pop());
```

### ❏ Union

1. `|` 을 사용하여 두 개 이상의 타입을 선언하는 방식
2. `union` 과 `generic` 은 모두 여러 타입을 다룰 수 있다. (`union` 은 공통된 메소드만 사용가능하다, 리턴값은 선언된 `union` 타입으로 지정된다.)

```typescript
// Union
const printMessage = (message: string | number) => {
    return message;
};

const message1 = printMessage(1322);
const message2 = printMessage("hellow");

// Generic
const printMessage = <T>(message: T) => {
    return message;
};

const message1 = printMessage<number>(1322);
const message2 = printMessage<string>("hellow");
```

### ❏ 제약조건(constraints / keyof)

1. 원하지 않는 속성에 접근하는 것을 막기 위해 `Generic` 에 제약조건을 사용한다.
2. `Constraints`: 특정 타입들로만 동작하는 `Generic` 함수를 만들 때 사용한다.
3. `Keyof`: 두 객체를 비교할 때 사용한다.

```typescript
// constraints: Generic T에 제약 조건을 설정한다.(string | number)
// 제약 조건을 벗어나는 타입을 선언하면 에러가 발생한다
const printMessage = <T extends string | number>(message: T) => {
    return message;
};

printMessage<number>(1322);
printMessage<string>("hello");
printMessage<boolean>(true); // Error: Type 'boolean' does not satisfy the constraint 'string | number'

// keyof: 두 객체를 비교할 때 사용한다.
// U의 값인 `not in obj` 가 `T`의 키 값 중 존재하지 않기 때문에 오류가 발생한다.
const printMessage = <T extends object, U extends keyof T>(obj: T, key: U) => {
    return obj[key];
};

console.log(printMessage({ a: 1, b: 2, c: 3 }, "a"));
console.log(printMessage({ a: 1, b: 2, c: 3 }, "not in obj")); // Error: Argument of type '"not in obj"' is not assignable to parameter of type '"a" | "b" | "c"'.
```

### ❏ 디자인 패턴

1. `Factory Pattern`: 객체를 생성하는 인터페이스만 미리 정의하고 인스턴스를 만들 클래스의 결정은 서브 클래스가 내리는 패턴
2. 여러개의 서브 클래스를 가진 슈퍼 클래스가 있을 때, 입력에 따라 하나의 서브 클래스의 인스턴스를 반환한다.

---

## 📍 25일차 11.27.토(온라인 강의)

오늘은 `typescript` 심화 그리고 `decorator`에 대해서 배웠다. 지금까지의 프로젝트를 하면서 많이 접해보지 않아 내용이 어렵게 느껴졌다. 나중에 기억에 잘 남으려면 실전에서 많이 사용해야겠지??

### ❏ Union Type, Intersection type

1. 기존 타입, 인터페이스의 변경은 이미 그 타입을 사용하고 있는 코드에 똑같은 변경을 가해줘야 한다. 만약, 해당 타입을 쓰는 모든 코드에 변경을 가하지 않고 특정 코드만 자유롭게 타입을 확장하고 싶을 땐 어떻게 해야할까?

```typescript
// Animal 인터페이스에 메소드를 추가하게 되면 해당 인터페이스를 implements하는 다른 class들에도 동일한 메소드를 추가해야 한다.
interface Animal {
    eat: () => void;
    sleep: () => void;
}

class Dog implements Animal {
    eat() {}
    sleep() {}
}

class Cat implements Animal {
    eat() {}
    sleep() {}
}
```

2. 그럴때는 `Intersection(And)`, : A타입이면서 B타입 `Union(Or)` A타입, B타입 둘 중 하나를 사용한다.

### ❏ Union

1. `|` 부호를 사용한다.

```typescript
// one의 타입은 string과 number 둘 중 하나
let one: string | number;
```

2. 여러 타입 중 하나가 올 것이라고 가정할 때 사용한다. 단, 인터페이스에 유니온 타입을 사용하는 경우 인터페이스는 유니온 타입을 확장하지 못함. 이럴 때는 `type` 과 `&` 를 사용해야 한다.

```typescript
// 에러 케이스
type A = string | number;

interface StrOrNum extends A {
    // Error: An interface can only extend an object type or intersection of object types with statically known members.
    a: string;
}

// 정상 케이스(유니온 타입의 확장)
type A = { a: string & (string | number) };

interface StrOrNum extends A {
    a: string;
}
```

3. Union Type 주의할 점: 동시에 여러 타입이 될 수 없다.

```typescript
// Human인지 Dog인지 확신할 수 없어서 컴파일 단계에서 에러
type Human = {
    think: () => void;
};

type Dog = {
    bark: () => void;
};

declare function getEliceType(): Human | Dog;

const elice = getEliceType();
elice.think(); // Error: Property 'think' does not exist on type 'Human | Dog'. Property 'think' does not exist on type 'Dog'.
elice.bark(); // Error: Property 'bark' does not exist on type 'Human | Dog'. Property 'bark' does not exist on type 'Human'.
```

### ❏ Intersection type

1. `&` 사용
2. `A` 타입이면서 `B` 타입이라는 의미

```typescript
type Human = {
    think: () => void;
};

type Developer = {
    work: () => void;
};

const elice: Human & Developer = {
    think() {
        console.log("I'm thinking");
    },
    work() {
        console.log("I'm working");
    },
};
```

3. `Intersection type` 은 기존 타입을 대체하지 않으면서, 기존 타입에 새로운 필드를 추가하고 싶을 때 사용한다.

```typescript
// Student 메서드를 추가하고 싶을 때
// 전
type Human = {
    think: () => void;
};

type Developer = {
    work: () => void;
};

const elice: Human & Developer & Student = {
    think() {
        console.log("I'm thinking");
    },
    work() {
        console.log("I'm working");
    },
};

// 후
type Student = {
    study: () => void;
};

const elice: Human & Developer & Student = {
    think() {
        console.log("I'm thinking");
    },
    work() {
        console.log("I'm working");
    },
    study() {
        console.log("I'm studying");
    },
};
```

4. 각 타입에 겹치는 필드가 있다면 어떨까?

```typescript
// 타입이 같을 때
type Developer = {
    output: string;
    develop: () => void;
};

type Designer = {
    output: string;
    design: () => void;
};

const 개자이너: Developer & Designer = {
    output: "띠용",
    develop() {
        console.log("I'm working");
    },
    design() {
        console.log("I'm working");
    },
};

// 타입이 다를 때
type Developer = {
    output: number;
    develop: () => void;
};

type Designer = {
    output: string;
    design: () => void;
};

const 띠용: Developer & Designer = {
    output: "며용", // Error: Type 'string' is not assignable to type 'never'.
    develop() {
        console.log("I'm working");
    },
    design() {
        console.log("I'm working");
    },
};

// 타입이 포함관계 일 때
type Developer = {
    output: number;
    develop: () => void;
};

type Designer = {
    output: number | string;
    design: () => void;
};

const 띠용: Developer & Designer = {
    // output : "며용",  Error: Type 'string' is not assignable to type 'number'.
    output: 28,
    develop() {
        console.log("I'm working");
    },
    design() {
        console.log("I'm working");
    },
};
```

### ❏ Type Guard

1. 데이터의 타입을 알 수 없거나, 될 수 있는 타입이 여러 개라고 가정할 때 조건문을 통해 데이터의 타입을 좁혀나가는 것
2. 데이터의 타입에 따라 대응하여 에러를 최소화 할 수 있음. 타입을 통해 가드하는 코드, 방어적인 코드를 짤 수 있음

```typescript
// Human인지 Dog인지 확신할 수 없어서 컴파일 단계에서 에러
type Human = {
    think: () => void;
};

type Dog = {
    bark: () => void;
};

declare function getEliceType(): Human | Dog;

const elice = getEliceType();
elice.think(); // Error: Property 'think' does not exist on type 'Human | Dog'. Property 'think' does not exist on type 'Dog'.
elice.bark(); // Error: Property 'bark' does not exist on type 'Human | Dog'. Property 'bark' does not exist on type 'Human'.

// 타입스크립트가 타입을 추론할 수 있도록 단서를 줘보면 어떨까
type Human = {
    think: () => void;
};

type Dog = {
    tail: string;
    bark: () => void;
};

declare function getEliceType(): Human | Dog;

const elice = getEliceType();

if ("tail" in elice) {
    elice.bark();
} else {
    elice.think();
}
```

3. 구별된 유니온으로 타입 가드하는 방법: 조건문을 통해 어떤 타입인지 추론한다.

```typescript
// 서버에서 오는 응답 또는 함수의 결과가 여러 갈래로 나뉠 때 사용
type SuccessResponse = {
    status: true;
    data: any;
};

type FailureResponse = {
    status: false;
    error: Error;
};

type CustomResponse = SuccessResponse | FailureResponse;

declare function getData(): CustomResponse;

const response: CustomResponse = getData();

if (response.status) {
    console.log(response.data);
} else if (response.status === false) {
    console.log(response.error);
}
```

4. `instanceof`: `TS` 에서 클래스도 타입이다. 객체가 어떤 클래스의 객체인지 구별할 때 사용하는 연산자

```typescript
class Developer {
    develop() {
        console.log("I'm working");
    }
}

class Designer {
    design() {
        console.log("I'm working");
    }
}

const work = (worker: Developer | Designer) => {
    if (worker instanceof Designer) {
        worker.design();
    } else if (worker instanceof Developer) {
        worker.develop();
    }
};
```

5. `typeof` : 데이터의 타입을 반환하는 연산자 (`data==null` 동등연산자를 사용하면 `null`, `undefined` 둘다 체크한다. 그러나, `null` 과 `undefined` 는 따로 체크하는 습관을 기르자, )

```typescript
const add = (arg?: number) => {
    if (typeof arg === "undefined") {
        return 0;
    }
    return arg + arg;
};
```

6. `in` : 오브젝트의 `key`중에 문자열 `A` 가 존재하는지 확인할 때

```typescript
// 문자열 A는 key(field, property 이름)을 의미한다.
type Human = {
    think: () => void;
};

type Dog = {
    tail: string;
    bark: () => void;
};

declare function getEliceType(): Human | Dog;

const elice = getEliceType();

if ("tail" in elice) {
    elice.bark();
} else {
    elice.think();
}
```

7. `switch-case`, `else-if`

```typescript
type Action = "click" | "hover" | "scroll";

// switch
const doPhotoAction = (action: Action) => {
    switch (action) {
        case "click":
            showPhoto();
            break;
        case "hover":
            zoomInPhoto();
            break;
        case "scroll":
            loadPhotoMore();
            break;
    }
};

// if
const doPhotoAction = (action: Action) => {
    if (action === "click") {
        showPhoto();
    } else if (action === "hover") {
        zoomInPhoto();
    } else {
        loadPhotoMore();
    }
};
```

8. `type-guard` 에 유용한 오픈소스

```typescript
// yarn add @sindersorhus/is
import is from "@sindresorhus/is";

const getString = (arg?: string) => {
    if (is.nullOrUndefined(arg)) {
        return "";
    }

    if (is.emptyStringOrWhiteSpace(arg)) {
        return "";
    }

    return arg;
};
```

### ❏ Optional Chaning

1. 접근하는 객체의 프로퍼티가 `null` 또는 `undefined` 일 수 있는 `optional property` 인 경우 `if` 문을 사용하지 않고 넘어가게 하는 체이닝 방법
2. `es2020` 에서 추가된 문법이며, 객체가 `null` 또는 `undefined` 이면 `undefined` 를 리턴, 그렇지 않은 경우 데이터 값을 리턴
3. `&&` 와 `?.` 의 차이점: `&&` 는 `falsy` 한 값 체크, `?.` 는 `null` 과 `undefined` 만 체크

```typescript
// 값이 있을 때만 반환한다.
type Cat = {
	sitDown?: () => void;
}

function trainCat(cat: Cat){
	cat.sitDown?.();
}

// 분기처리 optional Chaining
type Tail = {
	살랑살랑: () => void;
}

type Human = {
	call: (dogName: string) => void;
]

type Dog = {
	name: string;
	tail?: Tail;
	주인?: Human;
}

function petDog(dog: Dog){
	dog.주인?.call(dog.name);
	dog.tail?.살랑살랑();
}

// optional chaining refactory
// 전
function petDog(dog?: Dog) {
  if (dog && dog.tail && dog.tail.살랑살랑) {
    dog.tail.살랑살랑();
  }
}

// 후
function petDog(dog?: Dog) {
	dog?.tail?.살랑살랑?.();
}
```

### ❏ Nullish Coalescing Operator

1. `es2020` 에서 추가된 문법이며, 좌항이 `null`, `undefined` 인 경우에만 `B` 를 리턴
2. `A ?? B`: `falsy` 값을 그대로 리턴하고 싶은 경우 사용

```typescript
// price가 0인 경우 -1 반환
function getPrice1(product: { price?: number }) {
    return product.price || -1;
}

// price가 0인 경우 0 반환
function getPrice2(product: { price?: number }) {
    return product.price ?? -1;
}

console.log(0 ?? -1); // 0
console.log(0 || -1); // -1
```

3. falsy한 값(false로 평가되는 값) 0과 empty string(‘’)이 올 수 있는 변수에 **`||`** 를 쓰면 0, ‘’를 false로 인식하기 때문에 의도치 못한 결과를 초래할 수 있습니다. 실무에서 흔하게 저지르는 실수이기도 합니다. default 값을 지정해줄 때는 **`||`** 이 아니라 **`??`**을 쓰는 것을 권장합니다.

### ❏ Function overloading

1. 파라미터의 타입만 다르고 비슷한 코드가 반복되고 있는 상황, 코드의 중복을 줄이고 재사용성을 높일때 사용
2. 파라미터의 형태가 다양한 여러 케이스에 대응하는 같은 이름을 가진 함수를 만드는 것, 함수의 다형성을 지원하는 것
3. 함수의 이름이 같아야한다. 매개변수의 순서는 같아야한다. 반환 타입이 같아야 한다. `function` 키워드로만 가능하다,
4. 함수 오버로딩의 타입 선언부는 런타임에서 제거되고 구현부만 남기때문에, 실제 구현, 정의하는 함수는 하나여야만 한다.

```typescript
// 매개변수가 같을 때
class User {
    constructor(private id: string) {}

    setId(id: string): void;
    setId(id: number): void;
    setId(id: string | number): void {
        this.id = typeof id === "number" ? id.toString() : id;
    }
}

// 매개변수의 개수가 다를 때(순서만 지켜주면 된다.)
class User {
    constructor(private id: string) {}

    setId(id: string): void;
    setId(id: number, radix: number): void;
    setId(id: string | number, radix?: number): void {
        this.id = typeof id === "number" ? id.toString(radix) : id;
    }
}
```

제네릭은 사용하는 시점(제네릭, 인터페이스, 클래스 등등), 함수 오버로딩은 타입을 선언하는 시점(함수, 메서드)

### ❏ Type assertion

1. 타입스크립트가 추론하지 못하는 타입을 `as keyword` 를 통해 명시해주는 것
2. `type casting`: 데이터의 타입을 변환, `type assertion` : 데이터의 타입을 명시

```typescript
let someValue: unknown = "this is a string";

// 꺽쇠괄호는 react JSX가 인식을 잘 못함.
let strLength: number = (<string>someValue).length;

// as태그
let strLength: number = (someValue as string).length;
```

3. 타입단언: 타입스크립트가 개발자의 말만 믿고 `Duck` 타입으로 인식하여 빈 객체임에도 에러를 뱉지 않음
4. 타입선언: 객체 프로퍼티를 모두 채우도록 강제하기 대문에 실수를 저지를 위험이 낮음

```typescript
type Duck = {
	quack: () => void;
}

const duck: {} as Duck;

function add(x: string, y: string) {
  return (x as unknown as number) + (y as unknown as number)
}

const result = add('1', '2')
console.log(result)
```

### ❏ Index Signatrue

1. 객체의 특정 `value` 에 접근할 때 그 `value` 의 `key` 를 문자열로 인덱싱해 참조하는 방법
2. 객체의 프로퍼티들을 명확하게 알 수 없을 때 사용한다.
3. 어떤 타입이 올지 알 수 있다면 정확하게 타입을 정의하는것이 실수를 방지할 수 있다.
4. 인덱스 시그니처만 사용할 시, 타입을 표시해준 빈 객체에 에러가 나지 않습니다.

```typescript
type ArrStr = {
    [key: string]: string | number;
};

// HTTP headers
type HttpHeaders = {
    [key: string]: string;
};

type HttpHeaders = Record<string, string>;

const headers: HttpHeaders = {
    Host: "elice.io",
    Connection: "keep-alive",
    Accept: "*/*",
    "Access-Control-Request-Method": "GET",
    "Access-Control-Request-Headers": "authorization",
    "User-Agent":
        "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.69 Safari/537.36",
    "Sec-Fetch-Mode": "cors",
    "Sec-Fetch-Site": "same-site",
    "Sec-Fetch-Dest": "empty",
    "Accept-Language": "ko-KR,ko;q=0.9,en-US;q=0.8,en;q=0.7",
};

console.log(headers["Host"]); // elice.io
```

### ❏ Decorator

1. 함수가 한 가지 일만하면서 가독성을 높이고 반복되는 코드를 줄일 때 사용한다.
2. 함수를 감싸는 함수: 기존 함수를 바꾸지 않고 함수를 관찰, 수정, 재정의(오버라이딩)할 수 있는 함수
3. `babel` 플러그인을 사용해서 데코레이터 기능을 사용한다. `tsconfig.json` 에 `experimentDecorator` 옵션을 `true` 로 설정해줘야 한다.
4. 단일책임원칙 하에 함수의 기능을 확장할 수 있다.
5. `JS` `stage2` 에 있는 기능이므로, `TS` 에서는 실험적 기능으로써 사용 가능.

### ❏ 데코레이터를 쓰기 전 알아야 할 자바스크립트 개념

1. 일급객체
2. 클로저: 외부함수의 실행이 끝나도 내부함수에서 외부함수의 `context` 에 접근할 수 있는 것
3. 고차함수: 함수를 파라미터로 받아 반환하는 함수.

### ❏ 고차 함수의 용도

1. 커링: 함수의 매개변수를 받는 시점을 늦출 때
2. 함수의 실행 시점을 미룰 때(`jest - expect`, `react - onClick`)
3. 팩토리 함수(인스턴스 객체나 함수를 생성하여 반환하는 함수)를 만들 때
4. 훅, 데코레이터를 만들 때
5. 반복되는 코드를 줄일 때
6. 클래스 메서드는 고차 함수의 파라미터로서 전달했을 때 메서드는 인스턴스에 대한 `this` 바인딩을 잃어버린다. 따라서 `higher order`함수를 호출할 때 인스턴스와 메서드를 함께 인자로 전달해줘야 함

### ❏ Decorator Factory

1. 데코레이터를 사용하려면 `tsconfig.json - experimentalDecorators: true`, `emitDecoratorMetadata: true` `yarn add reflect-metadata` 설정
2. 고차함수: 함수를 반환하는 함수
3. 팩토리: 어떤 인스턴스를 사용하여 반환하는 함수, 메서드
4. 데코레이터 팩토리: 데코레이터 함수를 반환하는 함수
5. 특정 인자만 받는다. 추가적인 인자를 주고 싶다면 고차함수에 매개변수를 추가하여 데코레이터 함수 내부에서 사용할 수 있다.

```typescript
function enumerable(value: boolean) {
    return function (
        target: any,
        propertyKey: string,
        descriptor: PropertyDescriptor
    ) {
        descriptor.enumerable = value;
    };
}

class Greeter {
    @enumerable(false)
    greet(name: string) {
        return "Hello, " + name;
    }
}

// decoratorFacotry 함수를 선언해주세요.
function decoratorFactory(value: string) {
    return function (
        target: any,
        propertyKey: string,
        propertyDescriptor: PropertyDescriptor
    ) {
        console.log(value);
    };
}
// string 타입이고 이름이 value인 매개변수를 받습니다.
// 메서드 데코레이터 함수를 반환합니다.
// 메서드 데코레이터 함수의 매개변수 'target: any, propertyKey: string, propertyDescriptor: PropertyDescriptor'
// 메서드 decorator 함수 내부에서 value를 출력해주세요.

class ExampleClass {
    @decoratorFactory("룰루랄라 퇴근이다")
    static method() {}
}

ExampleClass.method();
```

### ❏ 클래스 데코레이터

1. 생성자 함수를 관찰, 수정, 오버라이딩(재정의) 한다.
2. 기존 클래스의 코드를 변경하지 않고 `property` 를 추가하거나, 생성자 함수에서 기능을 추가하고 싶을 때 사용한다.
3. 클래스 선언 직전에 선언된다.
4. 런타임에 함수로서 호출된다. `class` 에 `property`를 추가해도 `type system` 에서는 알지 못 함
5. 생성자 함수에 적용된다.
6. `target` 매개변수는 생성자 함수이다.
7. `d.ts` 파일(타입 선언 파일), `declare class`에는 데코레이터를 사용하지 못함(`experimentalDecorators: true`)를 해도 안된다.

```typescript
declare type ClassDecorator = <TFunction extends Function>(
    target: TFunction
) => TFunction | void;
```

### ❏ method Decorator

1. 메서드를 관찰, 수정, 오버라이딩 할 수 있다.
2. 메서드의 `property descriptor` 를 수정하거나 기존 메서드 앞 뒤로 기능을 추가하고 싶을 때 사용한다.

```typescript
import { UserGroup, User, Context } from "./types";

function permission(group: UserGroup) {
    return function (
        target: any,
        propertyKey: string,
        descriptor: PropertyDescriptor
    ) {
        const originFn = descriptor.value;

        // decorator function을 작성해주세요.
        descriptor.value = function (this: any, ...args: any[]) {
            // viewer의 group이 매개변수의 group보다 높은 경우(권한이 없는 경우) 함수를 실행하지 않고 에러메시지를 출력해주세요.
            const user = this.context.viewer;
            if (user.group > group) {
                console.log(
                    "permission is denied. viewer group is " + user.group
                );
                return;
            }
            // viewer의 group이 매개변수의 group 이하인 경우 원래 함수를 그대로 실행해주세요.
            return originFn.apply(this, args);
        };

        return descriptor;
    };
}

class UserService {
    constructor(public context: Context) {}

    @permission(UserGroup.NORMAL)
    updateName(user: User, name: string) {
        user.name = name;
    }

    @permission(UserGroup.ADMIN)
    deactivateUser(user: User) {
        user.status = "deactivate";
        return user;
    }
}

const normal: User = {
    id: "1",
    name: "normal",
    status: "activate",
    group: UserGroup.NORMAL,
};

const userService = new UserService({ viewer: normal });
// "permission is denied. viewer group is 2" 출력
userService.deactivateUser(normal);
userService.updateName(normal, "elice");
console.log(normal.name);
```

### ❏ Accessor Decorator

1. 접근자(`getter`, `setter`) 데코레이터는 접근자를 관찰, 수정, 오버라이딩 할 수 있다.
2. 접근자의 프로퍼티 설명자에 적용된다. 전달받는 매개변수가 메서드 데코레이터와 똑같다.(`target`, `propertyKey`, `propertyDescriptor`)
3. `method decorator` 와 같이 `ES5` 보다 낮으면 `undefined` 이 된다. 또한 반환값도 무시된다.
4. 같은 프로퍼티에 대한 접근자 `get`, `set` 중 하나에만 데코레이팅 가능

```typescript
function validate(regexp: string | RegExp) {
    return function (
        target: any,
        property: string,
        descriptor: PropertyDescriptor
    ) {
        const actualFunction = descriptor.set;

        const decoratorFunc = function (this: any, value: string) {
            const regexpTarget =
                typeof regexp === "string" ? new RegExp(regexp) : regexp;
            if (!regexpTarget.test(value)) {
                throw new Error("invalid value");
            }
            return actualFunction?.call(this, value);
        };

        descriptor.set = decoratorFunc;
    };
}
```

```typescript
function max(maximum: number) {
    return function (
        target: any,
        property: string,
        descriptor: PropertyDescriptor
    ) {
        // setter 함수를 교체하려면 descriptor의 어떤 프로퍼티에 적용해야할까요?
        const actualFunction = descriptor.set!; // 느낌표는 타입스크립트에 set함수가 있다고 가정한다. (option )

        const decoratorFunc = function (this: any, value: number) {
            // value가 maximum보다 커지면 `exceed the maximum number: ${maximum}`를 메시지로 메시지로 하는 Error를 throw해주세요
            if (value > maximum) {
                throw new Error(`exceed the maximum number: ${maximum}`);
            }

            // maximum 이하일 때는 함수를 정상적으로 실행해주세요
            return actualFunction.call(this, value);
        };

        descriptor.set = decoratorFunc;
    };
}

class Pagination {
    constructor() {}

    private _page: number = 0;

    get page() {
        return this._page;
    }

    @max(10)
    set page(step: number) {
        console.log();
        this._page = step;
    }
}

const pagination = new Pagination();

// Error: exceed the maximum number: 10
try {
    while (true) {
        pagination.page += 1;
    }
} catch (error) {
    console.log(error);
}
```

### ❏ Property Decorator

1. 프로터피를 관찰, 수정, 오버라이딩 할 수 있다.
2. 프러퍼티의 `property Descriptor` 를 수정할 때 사용할 수 있따.
3. 프로퍼티 선언 직전에 선언된다.
4. 인스턴스가 아닌 클래스 프로토타입의 프로퍼티에 적용된다.
5. `taget`, `propertyKey` 두가지 인자를 받는다.
6. `property Descriptor` 를 사용하지 않는이유: 프로퍼티의 경우, 인스턴스화 되기 전까 지 프로퍼티가 초기화되는 것을 관찰하거나 수정할 수 없음. 때문에 프로퍼티 데코레이터는 프로퍼티가 `클래스` 에 선언되었음을 관찰하는데만 사용할 수 있다.

```typescript
declare type PropertyDecorator = (
    target: Object,
    propertyKey: string | symbol
) => void | PropertyDecorator;

// 프로토타입 공유
function 영혼교환식(target: any, propertyKey: string) {
    let name: string;

    const getter = function () {
        return name;
    };

    const setter = function (value: string) {
        name = value;
    };

    return {
        get: getter,
        set: setter,
        enumerable: true,
        configurable: true,
    } as any;
}

class Human {
    @영혼교환식
    public name: string;

    constructor(name: string) {
        this.name = name;
    }
}

const 햄스터 = new Human("햄스터");
const 그녀 = new Human("그녀");

그녀.name = "민석씨";
console.log(햄스터.name); // 민석씨: 인스턴스가 아닌 클래스 프로토타입의 프로퍼티에 적용되기 때문에 값이 공유된다.

// 프로토타입 Symbol
function 영혼교환식(target: any, propertyKey: string) {
    const uniqueKey = Symbol(); // 매번 unique값을 생성

    const getter = function (this: any) {
        return this[uniqueKey];
    };

    const setter = function (this: any, value: string) {
        this[uniqueKey] = value;
    };

    return {
        get: getter,
        set: setter,
        enumerable: true,
        configurable: true,
    } as any;
}

class Human {
    @영혼교환식
    public name: string;

    constructor(name: string) {
        this.name = name;
    }
}

const 햄스터 = new Human("햄스터");
const 그녀 = new Human("그녀");

그녀.name = "민석씨";
console.log(햄스터.name); // 햄스터
```

1. 프로퍼티가 `null` 또는 `undefined` 일 때 기본값을 반환하는 `Default` 데코레이터만들기

```typescript
function Default(initalValue: any) {
    return function (target: any, propertyKey: string) {
        // 내부 함수에서 쓰일 value를 선언해주세요.
        let value: any;
        // value의 타입을 any로 설정해주세요

        // getter, setter 함수를 작성해주세요
        // getter: value가 null 또는 undefined면 initalValue를 반환해주세요
        function getter() {
            return value ?? initalValue;
        }

        // setter: setter 함수의 매개변수 _value를 그대로 value에 할당해주세요
        function setter(_value: any) {
            value = _value; // this를 붙이지 않아도 됨.
        }

        // propertyDescriptor를 반환해주세요
        // enumerable, configurable을 함께 설정해주세요
        const propertyDescriptor = {
            get: getter,
            set: setter,
            enumerable: true,
            configurable: true,
        };
        return propertyDescriptor as any;
    };
}

class Post {
    @Default(["짱이에요", "멋져요"])
    public comments?: any[];
}

const post = new Post();
console.log(post.comments);
```

### ❏ Parameter Decorator

1. 클래스의 생성자 함수 또는 메서드 선언 함수에 적용된다.
2. 매개변수가 메서드에서 선언되었다는 것을 관찰하는데에만 사용 가능. 그 이상은 `reflect-metadata` 라이브러리를 사용해야 한다.
3. 매개변수 선언 직전에 사용된다.
4. 3가지 인자를 받는다. 반환값은 무시된다.
5. `reflect-metatdata` 를 통해 파라미터에 대한 메타데이터 수집, 저장.
6. 메서드 데코레이터나 클래스 데코레이터와 함께 사용할 수 있음
7. 파라미터 데코레이터 함수에서 반환하는 값은 무시됩니다. (반환값이 void)
8. 파라미터 데코레이터는 메서드에서 매개변수가 선언되었다는 것만 알 수 있습니다.

```typescript
// target은 method(any, object), propertyKey는 메서드의 이름(string, symbol), 매개변수의 인덱스(순서)
declare type ParameterDecorator = (
    target: Object,
    propertyKey: string,
    parameterIndex: number
) => void;

function watch(target: Object, propertyKey: string, parameterIndex: number) {
    console.log(
        `메서드 이름: ${propertyKey}, 데코레이터 인덱스: ${parameterIndex}`
    );
}

class Human {
    constructor(public name: string) {}
    hello(@wath name: string) {}
}

declare type ParameterDecorator = (
    target: Object,
    propertyKey: string | symbol,
    parameterIndex: number
) => void;
```

1. reflect-metadata

```typescript
import { immutableKey } from "./immutable";

export function validateImmutable(
    target: any,
    propertyName: string,
    descriptor: PropertyDescriptor
) {
    const method = descriptor.value!;

    descriptor.value = function () {
        // Reflect.getOwnMetadata를 사용해 메타데이터를 가져와주세요
        const immutableParams: number[] = Reflect.getOwnMetadata(
            immutableKey,
            target,
            propertyName
        );
        // 메타데이터에는 paramIndex가 저장되어있습니다.

        const args = Array.from(arguments as any);
        // 자바스크립트 함수 내부에서 제공되는 arguments에서 메타데이터의 paramIndex만 필터링 해주세요. 그런 뒤 params 변수에 할당해주세요.
        const params = args.filter((val, idx) => immutableParams.includes(idx));

        // params 배열을 순회하며 Object.freeze로 객체를 수정하지 못하게 막아주세요.
        // map: 배열의 item을 변환하여 배열을 반환
        // forEach: 배열을 반환하지 않고 각 item에 함수를 적용할 때
        params.forEach((param) => Object.freeze(param));
        return method.apply(this, arguments);
    };
}
```

### ❏ Decorator의 동작

1. 여러 개의 데코레이터를 한 번에 쓰는 것(합성 함수 `g(fx))` 와 같은 매커니즘
2. `Reflect.decorate` 를 쓸 수 있으면 호출, 없으면 인자의 개수에 따라 매개변수를 다르게 주어 데코레이터를 호출한다.(이때 호출은 아래에서 위로, 합성함수의 매커니즘처럼 작용하기 때문)

```typescript
// 평가(선언): 위에서 아래로, log -> timer
// 적용(호출): 아래에서 위로, timer -> log
class Human {
	constructor(){}
	@log()
	@timer()
	hello(name: string){}

	const elice = new Human();
	elice.hello("elice")
}
```

3. 여러개의 데코레이터의 실행 순서

```typescript
/**
 * code source: https://www.typescriptlang.org/docs/handbook/decorators.html#decorator-composition
 */
function first() {
  console.log("first(): factory evaluated"); // #1
  return function (
    target: any,
    propertyKey: string,
    descriptor: PropertyDescriptor
  ) {
    console.log("first(): called"); // #2
  };
}

function second() {
  console.log("second(): factory evaluated"); // #3
  return function (
    target: any,
    propertyKey: string,
    descriptor: PropertyDescriptor
  ) {
    console.log("second(): called"); // #4
  };
}

class ExampleClass {
  @first()
  @second()
  method() {}
}

// 순서: 1 -> 3 -> 4 -> 2
first(): factory evaluated
second(): factory evaluated
second(): called
first(): called
```

---

## 📍 26일차 11.30.화(실시간 강의)

오늘부터는 `FE`가 아닌 `BE`에 대해서 간략하게 배운다. 여러 프레임워크 중 `Node.js`에 대해서 배우는데 한번 알아보자. 실시간 강의 때는 주로 실습을 하느라 이론을 많이 배우지 못했다. 내일 온라인 강의에서 더 자세하게 알아봐야겠다.

### ❏ Node.js

1. Chrome V8 javscript 엔진으로 빌드된 `javascript` 런타임입니다.
2. `Node.js`의 메인스레드는 하나이다. `JS`가 단일쓰레드인것처럼 `node.js`도 한 번에 한줄씩 실행한다.
3. `Docker`, `Auto scaling` 등을 이용해 `node.js`의 단일 스레드의 단점을 보완 할 수 있다.
4. `offLoading`: 메인스레드와 이벤트 루프는 서로 영향을 받지 않고 계속 실행된다.(저수준의 오래 걸리는 일은 `node.js`에게, 고수준의 로직은 메인스레드에서 실행한다.)
5. `LinkedIn`, `NETFLIX`, `UBER` 등에서 `node.js`를 사용한다.
6. <a href='https://glitch.com/'>Glich</a> 사이트를 통해 온라인에서 무료로 `node.js` 환경을 구축할 수 있다.
7. 예전의 `JS`는 퍼포먼스가 굉장히 떨어졌다. -> 이상한 코드를 집어넣으면 홈페이지가 느려진다. -> `firefox - spidermonkey`로 인해 성능이 매우 좋아졌다. > `microsoft - node.js`는 해당 환경을 브라우저가 아닌 로컬환경에서 작동시키기 위해 만들었다.
8. 런타임 환경: 컴퓨터가 실행되는 동안 프로세스나 프로그램을 위한 소프트웨어 서비스를 제공하는 가상 머신 상태
9. 컴파일 에러: 프로그램 동작 전에 발생하는 에러
10. 런타임 에러: 프로그램이 잘 동작하다가 중간에 발생하는 에러
11. `prettier`: 개발자가 작성한 코드를 통일시키는 방법
12. `eslint`: 자잘한 문법을 잡아준다. 코드를 분석하여 문법적인 오류, 안티 패턴ㅇ르 찾아준다.
13. `npm init`: `package.json` 생성
14. `npm init`: `package.json` 생성
15. `npm i eslint --save-dev`: eslint 설치
16. 라이브러리 ESLint 설치
17. `npm i -g npm`
18. `./node_modules/.bin/eslint --init` : eslint 환경설정
19. `npm i prettier`: 프리티어 설치
20. `./node_modules/.bin/prettier filename`
21. `./node_modules/.bin/prettier filename write`
22. `format`: format on save
23. `formatter`: 어떤 문법규칙으로 정리할지 선택하는 기능
24. `npm i eslint-plugin-airbnb`: airbnb 문법 사용

```javascript
const http = require("http"); // http 모듈 호출
const port = 9999;

http.createServer((req, res) => {
    res.end("Hello, world!"); // end: 담길데이터 다 담겼으니까 요청 글자를 보낸다.
}).listen(port, () => {
    console.log("서버가 켜졌어요!!!");
});

// 이후 F5 -> node.js실행
// res.end("<p style='color:red'>gimotti!!!</p>");처럼 innerHTML와 같은 코드로도 보낼 수 있다.
```

25. `commonJS` 방식은 `Node.js`에서 사용하는 방식으로 ES2015 의 모듈 개념이 나오기 전부터 사용됨. 기본은 `CommonJS` 이나, `package.json`을 수정하면 사용할 수 있음

```javascript
// CommonJS(default)
const http = require("http");

// ES2015, but 실질적인 사용은 2019년부터
import http from "http";
```

26. 동일한 `IP주소` 여도 포트번호를 통해 다르게 연결 할 수 있다.(default: 80)
27. `JS: Express.js` , `TS: Nest.js + Typescript` (해외에서 많이 쓰이고, 국내에서는 스프링을 많이 쓴다. 스프링은 전자정부에서 권장하는 프레임워크라서 많이 사용된다. 러닝커브가 상당히 빡세다.)
28. docker: 서버에 무엇인가를 설치할 때 오류가 발생함. 이런 문제를 줄이기 위해 나왔다. 설치가 이미 완료된 컨테이너를 가지고 잇다. 서비스에 올리기만 하면 바로 사용가능함. 모든 기술은 필요에 의해 나왔기 때문에 왜 기술을 사용하는지에 대해 알아두자.
29. 요즘 개발은 서버와 프론트를 컨테이너 안에 두고 깃허브에서 작성한 코드 커밋 → 테스트 → 빌드 → 자동으로 서버에 올린다. 이러한 과정을 `CI/CD` 라고 부른다.

### ❏ 내장 모듈

1. `node.js` 내부에서 제공하는 모듈
2. 모듈명이 같으면 현재 폴더를 기준으로 가장 가까운 모듈을 먼저 가져온다.
3. `require('fs').readFileSync`: 동기적으로 파일을 불러온다. (아무런 인코딩을 하지 않으면 `byte` 형태로 값을 불러온다. `Buffer`: 16진수 형태)

```javascript
const fs = require("fs");
const result = fs.readFileSync("./test");
const buf = Buffer.from([97, 98, 99, 100, 101]);
console.log(buf.compare(result)); // 0: 서로 같으면 0을 반환, 1이면 `buf` 가 더 크고, -1이면 `result`가 더 크다.

// 에러처리는 try-catch문으로 실행
```

4. `node.js` 데이터 구조: `stream` : 데이터를 작은 청크로 쪼개 처리한다. 큰 데이터를 처리하거나 비동기적으로 얻을 수 있는 데이터를 처리할 때 유용하다.

```javascript
const fs = require("fs");
const stream = fs.createReadStream("src/test");
stream.pipe(process.stdout);
```

5. `__filename`, `__dirname`: 파일 경로, 폴더 경로 표시하는 명령어

```javascript
console.log("__dirname", __dirname);
cosnole.log("__filename", __filename);
```

6. `dns`: `dns` 정보접근

```javascript
// family: verson(IPv4, IPv6...)
const dns = require("dns");
dns.lookup("google.com", (err, address, family) => {
    console.log(address, family);
});
```

7. `path`: 경로설정

```javascript
const path = require("path");
const fs = require("fs");

// 절대 경로 넣기
const filePath = path.resolve(__dirname, "./test.txt");
const fileContent = fs.readFilSync(filepath, "utf-8");
```

---

## 📍 27일차 12.1.수(온라인 강의)

오늘은 2021년 마지막 해의 첫 날이다. 그날 배운 내용들을 복습하는 글도 27번째 쓰고있는데, 22년 2월까지 하루도 빠짐없이 복습하는 글을 작성했으면 좋겠다. 현업에 뛰어들어서 볼 지금의 글들이 밤톨이나마 도움이 된다면 나의 목표는 달성한 것이다. 강의에서는 어제 실시간 강의로 간략하게 배웠던 `node.js`, `express.js`, `module` 등에 대해서 조금 자세하게 배웠다.

### ❏ node.js의 등장 배경

1. 웹의 발전에 의해 등장함. 단방향 통신 위주였던 `WEB1.0` 에서 사용자와 상호작용하는 `WEB2.0` 으로 발전하게 되면서 웹페이지의 동작은 더욱 복잡해졌고, 복잡한 `JS` 를 실행하기위해 고성능의 `JS` 실행기가 필요해졌다. 크롬에서는 웹브라우저를 위한 `V8` 엔진을 만들게 됨 `V8` 엔진으로 인해 `JS` 속도가 상당히 빨라지게 됐고, `V8` 엔진을 이용해서 웹 브라우저에서만 사용하는것이 아닌 어느 환경에서나 동작시킬 수 있도록 만들어진것이 `node.js` 이다. 즉, `js` 를 어느환경에서나 실행할 수 있게 해주는 실행기라고 할 수 있다.
2. 브라우저에서의 `JS`: 브라우저에서 실행, 웹 내부 제한된 동작, 웹 프론트 개발자의 언어
3. `node.js`: 크로스 플랫폼 실행, 제한 없는 동작, 다양한 어플리케이션 개발, 모든 개발자의 언어가 되었다.
4. `FE` : React.js, `BE`: Express.js,(최근 가장 인기 있는 웹서비스 구성), `Mobile`: React-native,(한가지 코드로 IOS와 Android 개발), `Desktop-app`: Electron(discord, slack 등 앱개발), `Machine-Learning`: Brain.js (JS로 구현하는 딥러닝)

![](https://images.velog.io/images/abcd8637/post/ad5ca1e3-ba08-42f4-83a8-47bf8ff67d4b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2009.20.00.png)

### ❏ node.js의 특징

1. 싱글 스레드 - 비동기 - 이벤트 기반
2. 스레드: 명령을 실행하는 단위, 싱글스레드는 한 번에 한 가지 동작만 실행 가능, 멀티쓰레드는 동시에 여러 동작 수행 가능하다.
3. 장점: 스레드가 늘어나지 않기 때문에 리소스 관리에 효율적
4. 단점: 스레드 기반의 작업들의 효율이 떨어짐(CPU 연산 작업)
5. 그래서 `node.js` 는 비동기 동작으로 스레드 기반의 작업을 최소화한다.
6. 비동기: 동작을 실행한 후 완료가 되길 기다리지 않는 방식, 동작의 완료를 기다리지 않기 때문에 다른 동작을 바로 실행 가능, `node.js` 는 싱글 스레드이기 때문에 비동기 방식을 사용함.
7. 멀티스레드는 한번에 여러가지 동작을 수행하기 때문에 동작을 수행하고 완료를 기다리는 동안 `CPU` 리소스가 낭비되는 반면, 싱글스레드는 한번에 여러가지 동작을 수행할 수 없지만 동작의 완료를 기다리지 않기 때문에 `CPU` 리소스를 효율적으로 사용할 수 있다.
8. 이벤트 기반: 비동기 동작의 완료를 처리하는 방법. 비동기 방식은 특정 동작을 실행한 후, 해당 동작을 전혀 신경쓰지 않음. 대신 해당 동작이 완료될 경우 실행 할 함수를 미리 등록함. 비동기 동작이 완료되면 미리 등록된 함수를 실행한다.
9. `node.js` 는 싱글 스레드기 때문에 비동기 동작이 필요하고 비동기 동작을 구현하기 위해 이벤트 기반의 동작 방식을 사용한다.

![](https://images.velog.io/images/abcd8637/post/099e18f8-03f5-482c-a601-06272f907e33/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2009.27.01.png)

### ❏ node.js 시작하기

1. `node.js` 는 빠르게 개발 중이므로 보안 이슈 및 버그 수정, 최신기술을 빠르게 적용한다. 급변하는 기술은 가장 안정적인 최신 버전을 선택하는 것이 최선이다.
2. `LTS(Long-term support)`: `node.js` 의 안정적이고, 오래 지원하는 버전 명
3. 가장 최신의 기술보다 안정적이고 최신의 버전을 선택하자.

### ❏ ES6

1. `ECMA6` 버전 이후를 통틀어 일반적으로 `ES6` 라고 부름
2. `ECMAScript`: 계속해서 발전해가는 `JS` 의 표준문법, 2015년 `ES6` 이후 많은 현대적인 문법이 추가됨
3. `let`, `const`: 상수와 변수 구분 가능
4. `Template String`: 기존에는 줄 바꿈은 `\n` 를 사용했으나 `backtick` 사용시 `\n`을 사용하지 않아도 된다. 변수는 `${}` 와 같이 사용할 수 있다.
5. `arrow-function`: 기존 함수는 `function` 으로 선언했으나, `()=>{}` 와 같이 간결하게 표현 가능하다.
6. `class`: 기존에는 객체 지향을 구현하기 위해 `function` 과 `prototype` 을 사용했다. `class` 는 `function` 으로 선언하고 클래스의 멤버나 메소드를 구현할 때는 `prototype` 을 사용했다. 이는 직관적이지 않고 가독성이 떨어졌다. `ES6` 에서 `class` 형태로 객체 지향적인 코드를 작성할 수 있다.
7. `destructing`: `Object` 에서 값을 꺼낼 때 일일이 작성하지 않고 `{} = obj` 처럼 변수를 꺼낼 수 있다.

### ❏ 비동기 코딩

1. 비동기: 이벤트 기반 동작을 코드로 구현하는 방법
2. `callback`: 전통적인 `JS` 의 이벤트 기반 코딩 방식

```javascript
// callback
// getUsers로 넘기는 함수가 이벤트 함수이고, 이러한 형태를 콜백이라 부른다.
// 쿼리가 완료되면 오류가 있는지, 혹은 성공했는지 여부를 인자형태로 받는다.
// 에러와 결과를 같이 전달하는 것이 표준으로 자리잡혀 있음

db.getUsers((err, users) => {
	console.log(users)
});

// callback-hell
// async1, async2, async3...을 동기적으로 실행해야 하는 경우, node.js는 기본적으로 비동기 동작을 callback으로 처리하기 때문에 콜백지옥 현상이 일어난다.
db.getUsers((err, users) => {
	if (err) {
		return;
	}
	async1(users, (r1) => {
		async2(r1, (r2) => {
			async3(r2, (r3) => {
				...
			});
		});
	});
});
```

3. `Promise`: callback 의 단점을 보완한 비동기 코딩 방식

```javascript
// promise: 함수의 동작이 완료되면 then에 등록된 callback을 실행한다. 오류가 발생한 경우 catch문의 callback 실행
// promise.chaning으로 코드를 간결하게, short-hand 표현으로 더욱 간결하게 표현 가능
db.getUsersPromise()
	.then((users) => {
		return promise1(users);
})
	.then(r1 => promise2(r1))
	.catch(... );

// callback을 promise 함수로 변경하기
// async1 함수의 실행 결과에 따라 resolve, reject로 분리
// reject는 catch에 등록된 callback 실행, resolve는 then에 등록된 callback 실행
function getUsersPromise(params){
	return new Promise((resolve, reject) => {
		getUsers(params, (err, users) => {
			if(err){
				reject(arr);
				return;
			}
			resolve(users);
		});
	});
}
```

4. `Async-await`: `promise` 의 단점을 보완한 비동기 코딩 방식, `promise` 의 다른 문법

```javascript
// async-await: 리턴 값은 promise
// await 한 promise 함수가 완료될 때까지 다음 라인으로 넘어가지 않음
// 순차적 프로그래밍처럼 작성 가능하다.
async function doSomething() => {
	const r1 = await promise1();
	const r2 = await promise2(r1);
	const r3 = await promise3(r1, r2);
	...
	return r3;
}

doSomething().then(r3 => {
	console.log(r3);
});

// err처리
async function doSomething(msg) => {
	try {
		const r1 = await promise1();
		console.log(r);
	}catch(e){
		console.log(e)
	}
}

// parallel run: promise 함수를 동시에 실행시키고 등록된 모든 함수가 마무리되면 결과값을 한꺼번에 반환
// 총 2초의 시간 소요
async function parallel(){
	const [r1, r2] = await Promise.all([
		promise1(),
		promise2(),
	]);
	console.log(r1, r2);
}

// 총 3초의 시간 소요
async function doSomething() => {
	const r1 = await promise1();
	const r2 = await promise2();
	console.log(r1, r2)
}
```

5. `callback-hell` : `promise chaining` 으로 해결
6. `promise-hell`: `async-await` 으로 해결
7. 대부분 가독성이 좋은 `async-await` 을 사용하지만, 상황에 따라 `callback`, `promise` 를 구사할 줄 알아야 한다.

### ❏ 이벤트 루프

1. 이벤트를 처리하는 반복되는 동작(loop)
2. `node.js` 가 비동기 - 이벤트 동작을 처리하는 일련의 반복 동작이며, 비동기 코딩이 어떤 순서로 수행되는지에 대해 이해할 수 있다.
3. 브라우저와 `node.js` 의 이벤트 루프는 기본적인 동작방식에 큰 차이가 없음. 이벤트루프의 기본적인 동작 원리를 이해하는 것이 중요하다.
4. `call stack`: `LIFO` 스택, 이벤트 루프는 콜스택이 비어있을 때까지 스택의 함수를 실행한다.
5. `message queue`: `setTimeout` 같은 지연실행 함수를 등록하는 `FIFO` 큐, 콜스택이 비어있을 경우 이벤트 루프에 의해 등록된 함수를 콜 스택에 추가한다.(setTimeout은 콜스택이 비어있을 때 실행)
6. `job queue`: `Promise` 에 등록된 콜백을 등록하는 `FIFO` 큐, 상위 함수가 종료되기 전에 콜스택이 비어있지 않더라도 잡큐에 등록된 콜백을 콜스택에 추가한다.(promise는 상위함수가 종료되기 전 실행)

### ❏ npm

1. `npm(node package manager)`: `node.js` 프로젝트를 관리하는 필수적인 도구(온라인 저장소 + 커맨드라인 도구)
2. `npm 저장소`: 필요한 라이브러리나 도구를 손쉽게 검색 가능. `node.js` 의 인기로, 거대한 생태계를 보유
3. 커맨드라인 도구: 프로젝트 관리를 위한 다양한 명령어 제공(프로젝트 설정 / 관리, 프로젝트 의존성 관리)
4. `npm init`: 해당 디렉토리 안에서 `package.json` 이라는 파일을 만들고, 이 디렉터리는 `node.js` 프로젝트가 된다.
5. `package.json`: 프로젝트 관련 정보들이 저장되는 파일. 이 파일을 직접 수정하거나 `npm` 명령어를 사용하여 프로젝트의 정보를 수정할 수 있음
6. 의존성: 프로젝트 내에서 라이브러리를 관리하는 방법, 프로젝트가 실행되기 위해 라이브러리에 의존하기 때문에 이러한 라이브러리들을 `dependency(의존성)` 이라고 부른다.
7. 라이브러리: 특정 기능을 수행하는 코드의 묶음, 복잡한 기능을 직접 작성하지 않고, 다른 사람이 구현한 것을 사용하는 방법(`node.js` 에서는 패키지라고도 부른다.)
8. `npm install`(약어 `npm i`): 프로젝트 의존성 관리 가능(의존성 추가, 의존성 내려받기, 개발용 의존성 추가, 전역 패키지 추가)
9. `npm install [package-name]`: 필요한 패키지를 프로젝트에 추가한다. 추가된 패키지는 `package.json` 의 `dependencies` 안에 추가되며, `node_modules` 디렉터리에 저장된다.
10. `npm install [package-name] --save-dev`: 개발용 의존성은 배포 전까지만 사용하느 의존성(유닛 테스트 라이브러리 등)인데, `--save-dev` 옵션을 이용하면 개발용 의존성을 추가할 수 있다. 개발용 의존성은 `package.json-devDependencies` 에 추가된다. 기본적으로 `node_modules` 디렉터리는 코드 관리나 배포시에 업로드 하지 않는데, 의존성이 많아지면 용량이 너무 커지고 운영체제별로 실행되는 코드가 다른 경우가 존재하기 때문이다.
11. `npm install --production`: 프로젝트 배포시 개발용 의존성을 포함하지 않고 내려받는다. `package.json-dependencies` 만 `node_modules` 에 내려받는다.
12. `npm install [package-name]@[version]`: `~1.13.0`: 1.13.x버전 설치, `~^1.13.0`: 1.x.x 버전 설치, 가장 왼쪽의 0이 아닌 버전을 고정, `0.13.0`: 0.13.0 버전만 설치(버전이 달라 오류가 날 때 주로 사용)
13. 프로젝트에 의존성을 추가하면 `package-lock.json` 이라는 파일이 생성됨. 프로젝트에 의존성을 추가하면 자동으로 `^`최신버전으로 추가가 되는데, 의존성 버전이 갑자기 변경되지 않도록, 설치된 버전을 고정하는 역할을 한다.
14. `npm install [package-name] —global`: 패키지를 전역 패키지 디렉토리에 내려받는다. 커맨드라인 도구들을 주로 전역 패키지로 추가해서 받음(`express-generator,pm2`)
15. 로컬 패키지: `package.json` 에 선언되어 있고, `node_modules` 에 저장된 패키지
16. 전역 패키지: `npm install -g` 를 통해 내려받아, 전역 패키지 저장소에 저장된 패키지
17. 전역 패키지도 프로젝트에서 사용할 수 있으나, 프로젝트의 의존성이 `package.json` 내에 명시적으로 선언되어 있는 것이 프로젝트 관리의 좋은 방향이다.
18. `npm remove [package-name]`: 의존성 패키지를 삭제한다. `dependencies`, `devDependencies` 에서 삭제하고 `node_modules` 에서도 삭제한다.
19. `npm run [script-name]` : 스크립트(간단한 동작을 수행하는 코드)를 실행한다.
20. `npm script` : 의존성 패키지를 사용할 수 있음
21. `npm test`: 코드 유닛테스트 등에 사용
22. `npm start`: 프로젝트 실행
23. `npm stop`: 프로젝트 종료
24. `run` 을 제외하고 사용할 수 있을뿐, `npm` 내부적으로 코드를 제공해 주는것은 아니다.

### ❏ npx

1. `npm` 패키지를 설치하지 않고 사용할 수 있게 해주는 도구, 프로젝트에 추가하거나 전역 패키지로 추가하지 않고 `npx` 를 이용하여 바로 실행할 수 있음
2. `gist` 코드를 다운받지 않고 바로 실행 가능(코드를 잘 확인하고 실행해야 함)

```javascript
// npm
npm i cowsay -g
cowsay hi

// npx
npx cowsay hi
npx node@12 index.js
```

### ❏ module

1. 간단한 프로그램이라면 파일 하나로도 가능, 프로젝트가 커지면 기능에 맞게 코드를 분리하는 것이 중요하다. 모듈은 코드를 분리하기 위한 방법
2. 반복되는 코드는 모듈로 분리하여 사용(재사용성 증가)
3. 패키지는 모듈의 모음, `npm` 패키지들은 많은 모듈을 포함하고 있는 코드 모음
4. `process`: 현재 실행프로세스 관련 기능 제공(`arch`, `argv`, `env`, `abort`, `kill`, `exit`)
5. `fs`: 파일 입출력을 하기 위해 사용(`readFile`, `writeFile`, `watch` 로 파일 / 디렉터리 변경 이벤트 감지)
6. `http`: `http` 서버, 클라이언트를 위해 사용, `createServer` 함수로 서버 생성, `request` 함수로 `http` 요청 생성
7. 기타 기본제공 모듈 확인하기: <a href='https://nodejs.org/dist/latest-v14.x/docs/api/'>node.js/doc</a>

### ❏ 모듈의 작성과 사용

1. `require` 함수를 통해 모듈을 `load` 할 수 있음
2. 의존성 패키지, 직접 작성한 모듈 사용 가능
3. `node.js` 의 모듈은 첫 `require` 시 `cache` , 두 번 실행하지 않음
4. 모듈 코드를 여러 번 실행하기 위해선 함수 모듈로 작성
5. 의존성 패키지들은 `require('package-name')` 로 `load` 가능하다. 패키지를 사용하려면 `node_modules` 에 내려받아져 있어야 함

```javascript
const name = "elice";
const age = 5;
const nationality = "korea";

// 모듈의 기본적인 사용법
// 모듈이 load 될 때 사용될 값을 module.exports로 내보냄
module.exports = {
    name,
    age,
    nationality,
};

// 변수명으로 export 하는 모듈 작성하기
// 모듈을 object로 만들고, 각 key - value를 지정해서 내보냄
exports.name = name;
exports.age = age;
exports.nationality = nationality;

const student = require("./elice"); // { name: "alice", age: 5, nationality: "korea" }

// 함수를 export하는 모듈
module.exports = (name, age, nationality) => {
    return {
        name,
        age,
        nationality,
    };
};

// npm 패키지 모듈
const dayjs = require("dayjs");
console.log(dayjs());

// 직접 작성한 모듈
const myModule = require("./my-module");
console.log(myModule);

// 함수형 모듈: 함수형은 load한 즉시 실행되지 않음
const myFunctionModule = require("./my-function-module");
console.log(myFunctionModule(name, age, nationality));

// json 모듈: json파일도 load가능, object로 자동파싱
const myData = require("./my-data");
console.log(myData);
```

### ❏ ES Module

1. ES6에서 등장한 JS의 공식적인 표준 모듈
2. JS는 기본적으로 모듈을 제공하지 않았다.
3. `node.js` 는 독자적인 방식을 통해 모듈을 지원하고 있었다(common js)
4. ES module의 등장으로 `node.js` 에서는 2가지 모듈을 지원해야한다.
5. `commonjs` 는 `module.exports`, `require` 로 모듈을 사용, `ES module` 은 `export` 와 `import` 로 모듈을 만들고 사용
6. 현재 `ES Module` 은 `node.js` 에서 기본적으로 사용하기에 제약이 많다.(프로젝트 타입을 `module` 로 변경, `commonjs` 모듈 `import` 시 문제 발생 등)

### ❏ 웹의 이해

1. 웹 서비스는 기본적으로 `HTTP` 요청과 응답의 반복으로 이루어짐. `HTTP` 요청은 사용자가 어떤 데이터가 필요한지를 서버에게 알리는 역할, `HTTP` 응답은 `HTTP` 요청에 해당하는 적절한 데이터를 전달하는 역할

![](https://images.velog.io/images/abcd8637/post/8709385a-0f67-4f2c-9cb0-b856268bea83/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2013.54.35.png)

2. 정적 웹(Web 1.0): 사용자와 상호작용하지 않는 페이지 - 단방향 통신, `Link` 를 통한 페이지 이동 정도만 가능, 일반적으로 변하지 않는 `html` 파일로 제공
3. 동적 웹(Web 2.0): 사용자와 상호작용을 함 - 양방향 통신, 구글 맵, 웹, 채팅 등 사용자가 다양한 기능을 수행할 수 있음, `FE` 와 `BE` 가 유기적으로 통신하며 동작한다. 현대적인 웹은 대부분 동적 웹이다.
4. `CSR` : 프론트엔드에서 사용자가 페이지에서 보는 동적인 부분을 대부분 처리하는 방식(사이트가 변하는 부분을 프론트엔드에서 처리, 페이지 리소스들이 미리 정의, `API` 통신이용, `API` 호출이 완료된 후에 보여준다. 복잡한 프로젝트 구성, 개발 사이즈가 커진다.)
5. `SSR`: 백엔드에서 페이지 대부분의 영역을 처리해서 프론트엔드로 전달하는 방식(프론트엔드는 `HTTP` 응답을 받아 화면에 표시, 백엔드에서 필요한 데이터가 포함된 페이지를 만들어서 `HTTP` 응답에 전달, 백엔드에서 `HTML` 파일을 작성해서 프론트로 전달, 쉬운 구성, 작은 개발사이즈, 로딩이 느려보이고, 페이지가 이동하면 페이지가 깜빡인다.)
6. 웹서버는 `HTTP` 요청과 `HTTP` 응답으로 이루어지는데 클라이언트는 서버로 `HTTP` 요청을 보내고, 서버는 `HTTP` 응답을 보낸다.

### ❏ 웹 프레임워크

1. 웹 서비스에 필요한 기능들을 제공해주는 다양한 도구들의 모음, 필요한 부분만 집중해서 개발 할 수 있음
2. `HTTP 요청`, `HTTP 응답`, `라우팅`, `HTML Templating`
3. 라우팅: `HTTP` 요청에 따라 알맞은 응답을 보내주는 경로를 설정하는 일
4. `HTML Templating`: `SSR` 을 구현하기 위한 방법, `SSR` 에서 응답으로 보낼 `HTML` 을 서버에서 작성하기 위해 `HTML Template` 를 통해 미리 페이지의 뼈대를 작성 가능
5. `node.js` 의 다양한 웹 프레임워크: `Express.js`, `Koa.js`, `Nest.js`, `Hapi`, `Sails.js`, `Meteor.js` 등등

### ❏ Express.js 시작하기

1. `node.js` 웹 프레임워크 중 가장 유명한 웹 프레임워크
2. 필요에 따라 유연하게 구조 설정 가능
3. 다양한 미들웨어를 통해 필요한 기능을 간단하게 추가 기능
4. 모든 동작이 명시적으로 구성되기 때문에, 웹 프레임워크의 동작 방식을 이해하기 가장 좋은 프레임워크
5. `npm init express`
6. `express-generator`: 프로젝트 생성기, 리액트의 `CRA` 와 비슷함

```javascript
// npm 시작
npm i -g express-generator
express my-web
cd my-web
npm i
npm start

// npx 시작
npx express-generator
cd my-web
npm i
npm start
```

### ❏ Express.js 구조

![](https://images.velog.io/images/abcd8637/post/0d5266c7-d607-4288-8b5a-0b8863ae3cfe/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2014.21.14.png)

### ❏ Express.js 동작방식

1. `express-generator` 로 만들어진 프로젝트 디렉토리에 접근하여, `npm start` 로 `Express.js` 프로젝트를 실행할수 있고 `[localhost:3000](http://localhost:3000)` 에 접속하여 페이지를 확인할 수 있다.

```javascript
1. localhost:3000 접속
2. app.js -> app.use('/', indexRouter);
3. routes/index.js -> router.get('/', ...)
4. routes/index.js -> res.render('index', ...)
5. views/index.jade
```

2. app.js: `express()` 로 생성되는 `app` 객체를 확인할 수 있다. `Express.js` 의 기능을 담은 객체
3. 라우팅: `app라우팅`, `express 라우팅`
4. `path parameter`: 주소의 일부를 변수처럼 사용할 수 있다.

```js
1. /users/:id - /users/123, /users/456 등으로 접속했을 때 라우팅 적용
2. /messges/:from-:to /message/123-456/ 등으로 접속했을 때 라우팅 적용
```

5. `request handler - request`: 라우팅에 적용되는 함수, `HTTP` 요청과 응답을 다룰 수 있는 함수로, 설정된 라우팅 경로에 해당하는 요청이 들어오면 `Request handler` 함수가 실행됨

![](https://images.velog.io/images/abcd8637/post/c0917c7f-e341-426f-9d3d-47833c4ec7e5/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2015.02.32.png)

```javascript
// 설정된 라우팅 경로에 해당하는 요청이 들어오면 `request handler` 함수를 실행한다.
router.get("/:id", (req, res) => {
    const id = req.params.id;
    res.send(`hello ${id}`);
});
```

6. `resquest-handler - response`: HTTP 응답을 처리하는 객체, HTTP 응답의 데이터를 전송하거나, 응답 상태 및 헤더를 설정할 수 있음

![](https://images.velog.io/images/abcd8637/post/491ccb9e-2905-4a01-97df-f766b09f0b0f/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2015.03.04.png)

```javascript
// path parameter
const express = require("express");

const app = express();

app.get("/", (req, res) => {
    res.send("hi");
});

// path parameter 사용하기
app.get("/say/:greeting", (req, res) => {
    const { greeting } = req.params;
    res.send(greeting);
});

app.listen(8080);

// router 연결
const express = require("express");
const userRouter = require("./routes/users");

const app = express();

app.get("/", (req, res) => {
    res.send("OK");
});

/* 라우터를 '/users' 경로에 연결 */
app.use("/users", userRouter);

app.listen(8080);
```

---

## 📍 28일차 12.2.목(실시간 강의)

바쁘게 살면 시간이 빨리 가는것처럼 느껴지는 특징이 있는데, 지금의 내가 그렇다. 엄청 많이 한것같지도 않은데 벌써 목요일이다. 얼른 수료하고 취업전선에 뛰어들고 싶다. 오늘은 `npm`, `API`, `RESTAPI`, `express.js`, `middleware`에 관한 내용을 배웠다.

### ❏ npm

1. `npm init`: `package.json` 파일 생성
2. `package.json`: 모듈을 관리하는 파일
3. `package.json - dependencies`: 내가 설치한 라이브러리를 보여준다. 버전 앞에 `^`는 버전을 대략적으로 보여준다. 업데이트 부분에서 자세하게 다룬다.
4. `npm cache clean -f`: 캐쉬 강제로 비우기
5. `node_modules`: 내가 설치한 모듈의 자세한 정보(내 컴퓨터 - programfiles라고 생각하면 편하다.)
6. 다른 개발자들과 협업할때는 `package.json`에 있는 모듈의 버전말고 `package-lock.json` 파일에 있는 모듈의 버전을 알려줘야 에러를 방지할 수 있다. `package.json`은 버전이 대략적으로만 나와있다.
7. `npm install [package-name] --save-dev`: 개발용으로 모듈을 설치한다.
8. `npm install \ yarn install`: `node_modules`가 없을 때 `package.json` 파일을 참고하여 `node_modules`를 설치해준다. (git clone 하고나서 사용하면 된다.)
9. `npm install --production`: 개발용 의존성(`devDependencies`) 모듈은 제외하고, `dependencies`에만 설치한다.
10. `sementic versioning`: 0.0.0(앞에서부터 `major`, `minor`, `patch` 순서로 부른다.)
11. `npm update [package-name]`: 버전 앞에 `^`가 붙어있으면 두번째 자리인 `minor`한 최신 버전을 업데이트한다. 버전 앞에 `~`가 붙어있으면 세번째 자리인 `patch` 를 최신 버전으로 업데이트 한다.
12. `npm install -g [package-name]`: 글로벌로 모듈을 설치한다.
13. `yarn add [package-name]`: 모듈 설치
14. `yarn add -D [package-name]`: 개발용 모듈 설치
15. `yarn remove [package-name]`: 모듈 제거
16. `scripts`: `CLI` 명령어 설정

### ❏ API

1. 내장 라이브러리로 사용하다 외부에 데이터를 저장해서 서버와 통신기기간에 정보를 주고받는 값을 말한다.
2. `soap`, `rest`: 정보 교환의 표준성 개발을 의미하는데, `soap`는 `xml` 기반으로 `html`처럼 코드가 복잡해서 이를 보완하기 위해 나온 것이 `rest`다. `rest`는 `json` 기반으로 코드가 간결하다.
3. `--print=hHbB`: 헤더를 통해 보낸값과 받은 값을 보여주는 명령어
4. `npm install --save-dev nodemon`: `node.js`의 코드가 바뀔 때마다 자동으로 새로고침해주는 라이브러리, 개발용으로만 사용하고 배포할때는 사용하지 않는 것을 권장한다.
5. `?`: 매개변수(쿼리끼리는 `&`로 구분한다.)

```json
http://localhost:9999/routes/is_odd_2?number=13&number3=1
```

6. `RESTAPI`: `API`지만, 웹을 통해 원하는 요청을 보내고, 그 요청을 받는 것. `URL`로 요청을 보내면 `HTTP` 상태 코드와 함께 결과값을 보낸다. 요청을 명세에 맞추어 보내야 `FE`, `BE`간에 원활한 통신이 가능하다. (`swagger`: RESTAPI 명세 작성 사이트)

```javascript
// GET
1. 데이터를 읽거나 검색할때 사용하는 메서드 (성공시 200 return)
2. GET 요청은 읽을 때만 사용, 수정될 때는 사용지 않아야 한다.

// POST
1. 주로 새로운 리소스를 생성할 때 사용 됨(일반적으로 성공 시 201return)
2. POST는 HTMl body나 JSON으로 전달 함
```

7. `.dotenv`: 함부로 노출할 수 없는 값(APIKEY, password 등)을 `env` 폴더에 저장해서 사용한다. (`gitignore`를 꼭 적용하자.)

### ❏ MiddleWare

1. `서버`와 `클라이언트`사이에 존재, 각기 분리된 2개 이상의 프로그램 사이에서, 매개역할을 하거나 연합시켜주는 프로그램. `next()`를 작성하지 않으면 해당 미들웨어에서만 실행하고 다음 미들웨어로 넘어가지 않는다.
2. `Express.js`에서 미들웨어는 순차적으로 코드를 실행한다.
3. 인증파트에서 `middleware`를 사용하고 인증이 되었으면, 내 주문, 선물함, 결제내역 등을 보는데 사용 될 수 있다.
4. `html form methods="POST"`로 설정하면 `URI` 뒤에 `?`형태로 쿼리값이 넘어온다

```javascript
// middle ware의 절차적인 프로세스1
app.use('/', (req, res, next) => {
	console.log('middelware 1');
	next();  // next가 없으면 넘어가지 않는다.
}

app.use('/', (req, res, next) => {
	console.log('middelware 2');
}

// middle ware의 절차적인 프로세스2: middleware2, hello, express
app.use('/', (req, res, next) => {
	console.log('middelware 2');
	res.send("hello, express!');
}

app.use('/', (req, res, next) => {
	console.log('middelware 1');  // 위 app에서 next가 없기때문에 실행되지 않는다.
}

// middleware에서 값을 넘겨주기
app.use('/', (req, res, next) => {
	console.log('middelware 1');
	const requestdAt = new Date();
	req.requestdAt = requestdAt;
	next();
}

app.use('/', (req, res, next) => {
	console.log(req.resquestedAt);  // Date
}

// promise 사용하기
app.use('/', (req, res, next) => {
	console.log('middelware 1');
	const fileContent = await fs.promises.readFile(".gitignore");
	req.fileContent = fileContent;
	next();
}

// 경로 설정
const express = require('express');
const app = express();
const PORT = 5000;

const fs = require('fs');

app.get('/',(req, res) => {
	res.send("Root - GET")
})

app.post('/',(req, res) => {
	res.send("Root - POST")
})

// ?: 앞의 값이 있어도 되고 없어도 된다.(option)
app.get('/ab?cd',(req, res) => {
	res.send("Root - GET")
})

// +: 앞의 값이 여러개가 와도 된다.
app.get('/ab+cd',(req, res) => {
	res.send("Root - GET")
})

// *: *자리에 아무문자나 와도 된다.
app.get('/ab*cd',(req, res) => {
	res.send("Root - GET")
})

// ()?: ()안의 값은 묶어서 사용한다.
app.get('/a(bc)?cd',(req, res) => {
	res.send("Root - GET")
})

// $: $앞의 값을 포함해야 한다
app.get('/abcd$/',(req, res) => {
	res.send("Root - GET")
})

// []: 배열 안의 값이 매칭될때
app.get(['/abc', '/xyz'],(req, res) => {
	res.send("Root - GET")
})

// 분기처리 전
app.get('/users',(req, res) => {
	res.send("Root - GET")
})

app.get('/users/:id',(req, res) => {
	res.send("Root - GET")
})

// 분기 처리 후
const userRouter = express.Router();
app.get('/',(req, res) => {
	res.send("Root - GET")
})
app.get('/:id',(req, res) => {
	res.send("Root - GET")
})
app.use('/users', userRouter);

// path parameter
userRouter.param('id', (req, res, next, value) => {
	req.user = USERS[value];
	next()
})

userRouter.get('/:id', (req, res) => {
	res.send(req.user);
})

// path parameter2
userRouter.post('/:id/nickname', (req, res) => {
	const { user } = req;
	const { nickname } = req.body;
	user.nickname = nickname;
})
```

5. 에러핸들링

```javascript
const user = USERS[value];

if (!user) {
    const err = new Error("User not found");
    err.statusCode = 404;
    throw err;
}

req.user = user;
next();

// express에서 4개의 인자를 준다. error 핸들링 미들웨어로 인식
app.use((err, req, res, next) => {
    res.statusCode = err.statusCode || 500;
    res.send(err.message);
});
```

---

## 📍 29일차 12.3.금(온라인 강의)

어제에 이어서 `express.js` 사용법 그리고 `middleware`, `postman`을 이용한 `RESTAPI`실습을 배웠다. 실습을 하면서 느낀건 <a href='https://velog.io/@abcd8637/%EC%B5%9C%EC%A2%85%EB%A9%B4%EC%A0%91-SW-%EC%A0%95%EA%B8%80%EC%82%AC%EA%B4%80%ED%95%99%EA%B5%90-%ED%9B%84%EA%B8%B0'>예전</a>에 정글사관학교 면접보기 전 과제 시험에서 게시판 `CRUD` 구현하는 과제가 있었는데, `R, U` 기능을 해결하지 못했었다. 이전의 기억을 트라우마로 갖고있어 `CRUD`를 조금 회피(?)하게 되었지만, 이번에 완전히 정복하겠다는 의지로 공부했다. 나중에 백엔드 엔지니어와 협업할 때 서버에 관해 대화를 할 때 말이 잘 통할정도로 성장하고 싶다.

### ❏ middleWare

1. 미들웨어는 `Express.js`동작의 핵심이다. `HTTP` 요청과 응답 사이에서 단계별 동작을 수행해주는 함수를 뜻한다.
2. `HTTP` 요청이 들어온 순간부터 `express.js` 가 실행된다. 미들웨어는 `HTTP` 요청과 응답 객체를 처리하거나, 다음 미들웨어를 실행 할 수 있다.(순차적으로 처리한다.) `HTTP` 응답이 마무리 될때까지 미들웨어 동작 사이클이 실행된다.
3. `req`, `res`, `next` 를 가진 함수를 작성하면 해당 함수는 미들웨어를 동작할 수 있다.

```javascript
1. req: HTTP 요청을 처리하는 객체
2. res: HTTP 응답을 처리하는 객체
3. next: 다음 미들웨어를 실행하는 함수
```

4. `RouteHandler`: 미들웨어의 한 종류, 라우팅 함수(get, post, put, delete 등)에 적용된 미들웨어, 일반적인 미들웨어와는 다르게 path parameter를 사용할 수 있다. next 함수가 호출되지 않으면 미들웨어 사이클이 멈추기 때문에 주의할것

```javascript
const logger = (req, res, next) => {
    console.log(`Request ${req.path}`);
    next();
};

const auth = (req, res, next) => {
    if (!isAdmin(req)) {
        res.send("Not Authorized");
        return;
    }
    next();
};
```

5. `middleware`는 적용되는 위치에 따라 어플리케이션 미들웨어, 라우터 미들웨어, 오류처리 미들웨어로 분류가능하다. 필요한 동작 방식에 따라 미들웨어를 적용할 위치를 결정한다.

```javascript
// 애플리케이션 미들웨어
// use나 http method 함수를 사용하여 미들웨어를 연결 할 수 있다.
app.use((req, res, next) => {
	console.log(`Request ${req.path}`);
	next();
)

app.use(auth);

app.get('/', (req, res, next) => {
	res.send('Hello express!')
})

// 라우터 미들웨어
// 특정경로의 라우팅에만 미들웨어를 적용하기 위한 방법
router.use(auth);

router.get('/', (req, res, next) => {
	res.send('Hello Router!')
})

app.use((req, res, next) => {
	console.log(`Request ${req.path}`);
	next();
)

app.use('/admin', router)

// 미들웨어 서브스택
// 여러개의 미들웨어를 동시에 적용할 수 있음. 주로 한개의 경로에 특정해서 미들웨어를 적용하기 위해 사용
app.use(middleware1, middleware2...);

app.use('/admin', auth, adminRouter);

app.get('/', logger, (req, res, next) => {
	res.send('Hello Router!')
})
```

6. 오류처리 미들웨어: 일반적으로 가장 마지막에 위치하는 미들웨어, 다른 미들웨어와 달리 err, req, res, next 네가지 인자를 가지며, 앞선 미들웨어에서 next 함수에 인자가 전달되면 실행됨

```javascript
// next에 인자로 넘기면 중간을 건너뛰고 마지막 오류처리 미들웨어가 실행된다.
app.use((req, res, next) => {
    if (!isAdmin(req)) {
        next(new Error("Not Authorized"));
        return;
    }
    next();
});

app.get("/", logger, (req, res, next) => {
    res.send("Hello Router!");
});

app.use((err, req, res, next) => {
    res.send("Error Occurred!");
});
```

7. 함수형 미들웨어: 하나의 미들웨어를 작성하고, 작동모드를 선택해서 사용하고 싶을 경우, 미들웨어를 함수형으로 작성하여 사용한다. (예, API 별로 사용자의 권한을 다르게 제한하고 싶은 경우)

```javascript
const auth = (memberType) => {
	return (req, res, next) => {
		if(!checkMember(req, memberType)){
			next(new Error(member not ${memberType}));
			return;
		}
		next();
	}
}

app.use('/admin', auth('admin'), adminRouter);
app.use('/users', auth('member'), userRouter);
```

8. 요약: 미들웨어는 HTTP 요청과 응답 사이에서 작동하는 함수, req, res, next 를 인자로 가질 수 있다. app 혹은 router 객체에 연결해서 사용가능하다. next 에 인자로 넘기면 오류처리 미들웨어가 실행된다. 미들웨어에 값을 설정하고 싶다면 함수형 미들웨어로 설정하라.

### ❏ REST API

1. `REST` 아키텍쳐를 준수하는 웹 `API`, `RESTFul` 이라고도 부른다.
2. `API` : 서비스나 프로그램간에 미리 정해진 기능을 실행할 수 있도록 하는 규약
3. `REST`: 웹에서 자료를 전송하기 위한 표현 방법의 아키텍쳐, 기본적인 REST 가이드를 따르면 조금 더 좋은 구조의 API를 구성할 수 있음
4. API의 동작을 `HTTP method + 명사형 URL` 으로 표현함. `/posts` `url` 은 게시글 자원을 가리킨다고 할 때 http method(get, post, put, delete)와 결합하여 api 동작을 정의한다.
5. `url` 표현법: 자원을 복수형으로 표현하고 하나의 자원에 접근은 복수형 + 아이디를 통해 특정 자원에 접근한다. 예를 들어 `/posts` 가 게시글 전체라고 한다면, `/posts`은 1번 게시글이라는 자원을 표현함
6. `rest api` 는 `url` 을 통해 자원을 계층적으로 표현한다. `/users/1/posts` 라는 `URL` 은 1번 유저의 게시글 전체라는 자원을 나타낸다
7. restapi는 rest 아키텍쳐를 준수하는 웹 api를 의미하며, rest 아키텍쳐를 준수하는 간단한 방법으로 url을 통한 자원의 표현 방법과 http method를 통한 api 동작의 정의 정도만 사용해도 훌륭한 rest api를 구현할 수 있다.

### ❏ JSON

1. JS에서 객체를 표현하는 표현식으로 시작했다. 데이터를 표현하는 방법이 단순하고 이해하기 쉬워서 데이터를 전송할 때 많이 사용한다.
2. 웹 api는 데이터를 문자열로 전송한다. 어떤 객체를 웹 api를 통해 문자열로 전달하기 위해 json을 사용한다.
3. `value` 에는 어떤 값이라도 사용 될 수 있다.

### ❏ Express.js로 REST API 구현하기

1. 간단한 메모의 작성, 삭제, 확인기능 api 구현
2. express-generator를 사용하지않고 MVC패턴 구현

### ❏ MVC 패턴

1. 프로젝트의 기능들을 어떻게 분리할지에 대한 하나의 구성 방법
2. model: 데이터에 접근하는 기능, 데이터 그 자체, 데이터의 읽기 쓰기는 `model` 을 통해서만 표현
3. view: 데이터를 표현하는기능, controller에 의해 데이터를 전달받고 화면에 표시하는 기능
4. controller: model을 통해 데이터에 접근하여 처리 결과를 view에 전달하는 기능, 라우팅 함수가 controller기능을 수행한다.
5. `express.js` 는 기본적으로 `HTTP body` 에 전달되는 `JSON` 데이터를 처리하지 못함. `express` 에서 기본적으로 제공해주는 `express.json()` 미들웨어를 사용해야 `JSON` 데이터를 사용할 수 있 `a pp.use(express.json())`
6. 가장 마지막 미들웨어로 오류 처리 미들웨어를 적용하면 모든 라우팅에 공통적인 오류처리 로직을 적용할 수 있음

```javascript
// 이전에 next()에 인자로 넘겨줌
app.use((err, req, res, next) => {
    res.status(500);

    res.json({
        result: "fail",
        error: err.message,
    });
});
```

7. 모든 라우팅이 적용 된 이후 사용되는 미들웨어는 설정된 경로가 없는 요청을 처리하는 Route Handler 로 동작한다. Express.js 는 기본적으로 404 페이지를 가지고 있지만, 직접 처리가 필요할 때 Route Handler 를 추가한다.

```javascript
app.use((req, use, next) => {
    res.status(404);
    res.send({
        result: "fail",
        error: `Page not found ${req.path}`,
    });
});
```

### ❏ postman

1. API 테스트 도구로 HTTP 요청을 손쉽게 작성하여 테스트해볼 수 있게 도움을 준다.

### ❏ 미들웨어 작성과 사용

이하 실습 코드 생략

---

## 📍 30일차 12.4.토(온라인 강의)

오늘은 `mongoDB`와 `express.js`를 연동하여 `CRUD`하는 법을 배웠다. 예전에 `mongoDB`를 이용하여 최신 기사를 한눈에 보여주는 <a href='https://blog.naver.com/abcd8637/222152180429'>지금 뉴스!</a> 프로젝트를 진행했으나, `AWS` 무료 티어기간이 끝나서 취소하는 바람에 서버를 닫았다. 그때는 `Robo 3T` 프로그램으로 `mongoDB`를 조작했는데 이번에는 <a href='https://www.mongodb.com/ko-kr'>mongoDB</a> 홈페이지에 `cloud` 기능과 연동하는 법을 배웠다. mongoDB 홈페이지에서 다루니까 훨씬 `UX`가 좋았다.

### ❏ MongoDB

1. 대표적인 `NoSQL`, `Document DB` mongo는 Humongous에서 따온 말로, 엄청나게 큰 DB, 대용량 데이터를 처리하기 좋게 만들어짐
2. `NoSQL` (Not Only SQL): 구조화된 질의어를 사용하지 않는 데이터베이스, 자료간의 관계에 초점을 두지 않음. 데이터를 구조화하지 않고 유연하게 저장함
3. `RDB` (Relational Database): 관계형 데이터 베이스, 자료들의 관계를 주요하게 다룸, SQL 질의어를 사용하기 위해 데이터를 구조화 해야함
4. 왜 `NoSQL`을 사용하는가? `SQL`을 사용하기 위해서는 데이터를 구조화하는 것이 필수이다.(`DDL`) 스키마에 정의된 데이터가 아니면 저장할 수 없는 제약이 따르는데, `NoSQL` 을 사용하면 사전작업 없이 DB 를 사용할 수 있다.(DB크기에 관여하지 않고 프로젝트를 빠르게 진행할 수 있음)

```SQL
// MySQL
CREATE DATABASE simple_board

CREATE TABLE posts (
	id NOT NULL AUTO INCREAMENT
	title VARCHAR(30),
	content TEXT,
	PRIMARY KEY(id)
)

INSERT INTO posts (title, content)
VALUES
('first title', 'first content'),
('second title', 'second content')

// MongoDB
use simple_board
db.posts.insert([
	{
		title: 'first title',
		content: 'first content'
	},
	{
		title: 'first title',
		content: 'first content'
	}
])
```

5. NoSQL은 다양한 종류가 있지만, 대표적으로 자료를 문서로 저장하는 `DocumentDB` 가 일반적, 이 외에, `key-value`, `Graph`, `large collection` 등의 `NoSQL DB` 가 존재한다.
6. `mongoDB` 를 직접 설치하거나 `Cloud` 서비스를 사용할 수 있음. 직접 설치하면 귀찮고 어렵지만, 원하는 만큼 얼마든지 데이터를 사용할 수 있음. `Cloud` 를 사용하면 쉽고 빠르게 시작 가능하지만, 사용량에 따라 요금이 부과된다.
7. 직접 설치하기: 직접 모든 DB 관련 설정을 해야한다. sharding 이나 replication 등의 작업이 필요할 때 운영지식과 노하우가 요구된다. 무료로 제공하는 community version 을 제공함
8. `mongoDB cloud`: 모든 DB 기능을 웹에서 관리 가능하다. 특별한 노하우없이 DB 운용 가능하고 `512MB`까지는 평생 무료로 사용가능
9. `mongoDB compass`: mongoDB에 접속하여 Database, collection, document 등을 시각화하여 관리할 수 있게 도와주는 도구, MySQL workbench 와 유사

### ❏ MongoDB의 기본 개념

1. `Database`: 하나 이상의 `collection` 을 가질 수 있는 저장소, `SQL`에서의 `database` 와 유사
2. `Collection`: 하나 이상의 `Document`가 저장되는 공간. SQL 에서의 table 과 유사하다. 하지만, collection 이 document 의 구조를 정의하지 않음
3. `Document`: `mongoDB` 에 저장되는 자료, SQL 에서 row 와 유사하지만, 구조제약 없이 유연하게 저장 가능, JSON 과 유사한 BSON 을 사용하여 다양한 자료형을 지원한다.
4. `document - objectID` : 각 document 의 유일한 키 값, SQL 의 primary key 와 유사하다. 하나씩 증가하는 값이 아닌 document 를 생성할 때 자동으로 생성되는 값(timestamp + random value + auto increament)

### ❏ Mongoose ODM

1. `ODM(Object Data Modeling)`: MongoDB의 collection에 집중하여 관리하도록 도와주는 패키지 Collection 을 모델화하여, 관련 기능들을 쉽게 사용할 수 있도록 도와줌
2. `MongoDB` 는 기본 `Node.js` 드라이버는 연결상태를 관리하기 어려움 이때, `Mongoose` 를 사용하면 간단하게 데이터베이스와의 연결상태를 관리해줌.
3. 스키마 관리: 스키마를 정의하지 않고 데이터를 사용하는 것은 NoSQL 의 장점이지만, 데이터 형식을 미리 정의 해야 코드 작성과 프로젝트 관리에 유용함. `Mongoose` 는 `Code-level` 에서 스키마를 정의하고 관리할 수 있게 해줌, 중간단계에서 체크해주고 관리함
4. `populate`: `mongoDB`는 `join` 을 제공하지 않음. `join` 과 유사한 기능을 사용하기 위해서 `aggregate` 라는 복잡한 쿼리를 사용하지만 `Mongoose` 에서 `populate` 를 사용하여 간단하게 구현할 수 있음

### ❏ Mongoose ODM 사용순서

1. 스키마 정의 → 모델 만들기 → 데이터베이스 연결 → 모델 사용
2. 스키마 정의: `Collection` 에 저장될 `Document` 의 스키마를 `Code-level` 에서 관리할 수 있도록 `schema` 를 작성할 수 있음. 다양한 형식을 미리 지정하여 생성, 수정 작업 시 데이터 형식을 체크해주는 기능을 제공함. `timestamps` 옵션을 사용하면 생성, 수정 시간을 자동으로 기록해 줌

```javascript
const { Schema } = require("mongoose");

const PostSchema = new Schema(
    {
        title: String,
        content: String,
    },
    {
        timestamps: true,
    }
);

module.exports = PostSchema;
```

3. 모델 만들기: 작성된 스키마를 `mongoose` 에서 사용할 수 있는 모델로 만들어야 함. 모델의 이름을 지정하여 `populate` 등에서 해당 이름으로 모델을 호출 할 수 있음

```javascript
const mongoose = require("mongoose");
const PostSchema = require("./schemas/board");
exports.Post = mongoose.model("Post", PostSchema);
```

4. 데이터베이스 연결하기: `connect` 함수를 이용하여 간단하게 DB 에 연결할 수 있음. `mongoose` 는 자동으로 연결을 관리해주기 때문에 직접 연결 상태를 체크하지 않아도 모델 사용 시 연결 상태를 확인하여 사용이 가능할 때 작업을 실행 함

```javascript
const mongoose = require("mongoose");
const { Post } = require("./models");
mongoose.connect("mongodb://localhose:27017/myapp");
```

### ❏ 모델 사용하기 - 간단한 CRUD

![](https://images.velog.io/images/abcd8637/post/5f2948d4-a672-49e9-bcd5-92c2d5ba714d/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-04%2012.09.12.png)

1. `CREATE`: create 함수를 사용하여 Document생성, create 함수에는 Document Object 나 (단일 Document) Document Object 의 Array 전달 가능(복수Document), create 는 생성된 Document 를 반환해줌

```javascript
const { Post } = require("./models");

async function main() {
    const created = await Post.create({
        title: "first title",
        content: "second title",
    });

    const multipleCreated = await Post.create([item1, item2]);
}
```

2. `FIND(READ)`: find 관련 함수를 사용하여 document 를 검색, query 를 사용하여 검색하거나 findById 를 사용하면 objectID 로 document 를 검색할 수 있음

```javascript
const { Post } = require("./models");
async function main() {
    const listPost = await Post.find(query);
    const onePost = await Post.findOne(query);
    const postById = await Post.findById(id);
}
```

3. `query` : MongoDB 에도 SQL where 와 유사한 조건절 사용 가능. MongoDB 의 query 는 BSON 형식으로 기본 문법 그대로 mongoose 에서도 사용 가능, {key: value}로 `exact match`

```javascript
Person.find({
    name: "AYW",
    age: {
        $lt: 20, // less then: 미만(and)
        $gte: 10, // grater then equal: 이상(and)
    },
    languages: {
        $in: ["ko", "en"], // in: 존재하면(and)
    },
    $or: [
        // or: acive이거나 true인 값 중 하나
        { status: "ACTIVE" },
        { isFresh: true },
    ],
});
```

4. `mongoose` 는 쿼리 값으로 배열로 전달하면 자동으로 `$in` 쿼리를 생성해준다.

```javascript
Person.find({ name: ["elice", "ted"] }); // { name: { $in: ['elice', 'ted' ]}}
```

5. `UPDATE`: update 관련 함수를 사용하여 document 를 수정, find~ 함수들은 검색된 document를 업데이트를 반영하여 반환해준다. 반면, update 는 기본적으로 $set operator 를 사용하여 document 를 통째로 변경하지 않는다.

```javascript
async function main() {
    const updateResult = await Post.updateOne(query, {});
    const updateResults = await Post.updateMany(query, {});
    const postById = await Post.updateOne(query, {});
    const onePost = await Post.findOneAndUpdate(query, {});
}
```

6. `DELETE` : delete 관련 함수들을 사용하여 document 삭제결과를 리턴한다. find~ 함수들은 검색된 document 를 반환해준다.

```javascript
async function main() {
    const deleteResult = await Post.deleteOne(query, {});
    const deleteResults = await Post.deleteMany(query, {});
    const onePost = await Post.findOneAndDelete(query, {});
    const postById = await Post.findByIdAndDelete(query, {});
}
```

7. `populate`: document 안에 document 를 담지 않고 objectID 를 가지고 reference 하여 사용할 수 있는 방법, document 에는 reference 되는 ObjectID 를 담고, 사용할 때 populate 하여 하위 Document 처럼 사용할 수 있게 해줌

```javascript
const Post = new Schema({
    user: {
        type: Schema.Types.ObjectId,
        ref: "User",
    },
    comments: {
        type: Schema.Types.ObjectId,
        ref: "Comment",
    },
});

const post = await Post.find().populate(["user", "comments"]);
```

### ❏ Express.js + Mongoose ODM

1. `Express.js` 는 프로젝트 구조를 자유롭게 구성할 수 있기 때문에 어느 부분에 `Mongoose ODM` 을 위치시키면 좋을지 적절한 위치를 결정하는 것이 중요
2. 일반적으로 `models` 디렉터리에 `Schema` 와 `Model` 을 같이 위치시킨다. `app` 객체는 어플리케이션 시작을 의미하는 부분으로 해당 부분에 데이터베이스 연결을 명시하는 `mongoose.connect` 를 위치한다. 특별한 제약이 있는것은 아니다.

![](https://images.velog.io/images/abcd8637/post/015977e8-b060-4a36-876b-28414b573f3c/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-04%2016.34.38.png)

3. `Express.js` 어플리케이션은 종료되지 않고 동작하기 때문에, 계속해서 DB 가 정상적으로 동작하는지 파악하기 위해 동작 중에 발생하는 DB 연결 관련 이벤트에 대한 처리를 하는 것이 좋음

```javascript
// connection events
mongoose.connect("----");
mongoose.connection.on("connected", () => {}); // 연결완료
mongoose.connection.on("disconnected", () => {}); // 연결끊김
mongoose.connection.on("reconnected", () => {}); // 재연결 완료
mongoose.connection.on("reconnectFailed", () => {}); // 재연결 시도 횟수 초과
```

### ❏ Sequelize ORM

1. `ORM`(Object-Relational Mapping): `MySQL`, `PostgreSQL` 등의 `RDBMS` 를 이용하는 간단한 방법 `ODM` 이 단순히 모델에 집중하여 관리하는 것에 반해, `ORM` 은 테이블 관계와 쿼리 등의 기능을 더욱 단순화하는 용도로 주로 사용
2. `sequelize` 도 연결을 관리하는 간단한 방법을 제공, `mongoose` 가 `mongoDB` 만 연결이 가능한데에 반해, `sequelize` 는 `MySQL`, `PostgreSQL` , `SQLite` 등 다양한 `RDBMS` 에 연결가능하다.
3. 나중에 `node.js`로 관계형 데이터베이스를 구현하고 싶으면 `Sequelize`를 공부하자.

```javascript
// connect db
const sequelize = new Sequelize("database", "usename", "password", {
    host: "localhost",
    dialect: "mysql",
});
```

4. 스키마 작성: `define` 을 통해 `Schema` 생성, `sequelize` 는 `Schema`가 `DDL도` 생성해준다.

```javascript
const User = sequelize.define(
    "User",
    {
        name: {
            type: DataTypes.STRING(10),
            allowNull: false,
        },
        age: {
            type: DataTypes.Integer,
        },
    },
    {}
);
```

5. 관계 정의: 테이블 간의 관계를 `Code-level` 로 관리 할 수 있다. 이를 이용하면 외래키 설정과 제약조건까지 `DDL` 로 생성한다. 또한 다대다 관계 설정을 통해 `relation table` 도 자동으로 생성한다.

```SQL
User.hasMany(Post);
Post.belongsTo(User);
Foo.belongsToMany(Bar);
Bar.belongsToMany(Foo);
```

6. 쿼리: Operator 를 이용해 SQL 쿼리를 코드로 작성 가능, 스키마의 관계 설정을 한 경우 include 를 사용하여 자동으로 join 쿼리 생성 가능

```SQL
User.findAll({
	where: {
		name: 'elice',
		age: {
			[Op.lt]: 20,
			[Op.gte]: 10.
		},
	},
	include: User,
})
```

7. `Synchronization`: `define`된 model 데이터를 바탕으로 DDL 을 자동으로 실행해줌. 직접 데이터베이스에 접속하여 테이블 생성 및 관리를 할 필요가 없음. 자동으로 생성된 DDL 을 따르지 않으면 테이블 관리가 어려워 짐

```javascript
sequelize.sync();
```

8. `Sequelize ORM` 를 사용하면 데이터베이스에 직접 DDL 을 사용하지 않고, JS 코드로 테이블 및 관계를 관리할 수 있다. 또한 RDB 의 어려운 점 중 하나인 join 을 includes 옵션을 통해 간단하게 사용할 수 있다.

---

## 📍 31일차 12.7.화 데이터 베이스 연동(실시간 강의)

이번주는 `node.js`를 바탕으로 `mongoDB`를 이용하여 데이터베이스를 연동하여 회원가입과 로그인 기능을 구현한다. 프론트엔드를 준비하고 있어 `DB`를 많이 공부하진 않았지만 이번 기회를 계기로 `DB`와 친해져보고 게시판 `CRUD`와 페이지네이션을 구현해보고 싶다.

### ❏ DataBase

1. 여러 사람이 공유하여 사용 할 목적으로 체계화하여 관리되는 데이터의 집합(`DBMS`에 의해 제어 됨)
2. 데이터 공유: 여러명이 동시에 공유하더라도 안정성, 정확성을 갖춤
3. 데이터 중복 최소화: 하나의 데이터베이스에 여러 테이블을 나누어 데이터 중복 최소화
4. 지속성: 데이터가 여러 군데에 산재해 있으면 동시에 관리하기 어렵고, 무결성 유지도 어려움, 데이터베이스는 `DBMS`에 의해 중앙집중적으로 관리되어 무결성 유지가 용이
5. 보안성: 중앙집중적으로 관리되기에 한 군데만 보안을 유지하면 됨
6. `ACID`: 원자성(Atomicity) - 트랜잭션 관련 작업이 모두 수행됐는지 확인, 일관성(Consistency) - 데이터가 언제나 일관성 있는 상태인지 확인, 고립성(Isolation) - 한 작업 수행시 다른 작업이 끼어들지 못하게 보장, 지속성(Durability) - 성공적으로 수행된 작업은 영원히 반영 즉 `ACID`는 데이터베이스 트랜젝션이 안전하게 수행된다는 것을 보장하기 위한 성질이다.
7. `SQL`은 `ACID`가 있는 대신 프로그램이 무겁지만 안전하다. 반대로 `NoSQL`은 `ACID`가 없는 대신에 프로그램이 `SQL`보다 가볍고 빠르다. 대신 어플리케이션단에서 보안을 강화시켜야 한다.
8. 수직확장: `SQL`에서 한 인스턴스를 키워 더 큰 로드를 감당한다. 이는 한계가 있다.
9. 수평확장: `NoSQL`에서 더 많은 인스턴스를 만들어 더 큰 로드를 감당한다. `NoSQL`은 데이터 구조가 정해져 있지 않아 인스턴스를 무제한 늘릴 수 있다.(운영비용이 받쳐준다면..)

### ❏ DBMS

1. Oracle: 가장 먼저 상업용으로 발표된 관계형 데이터베이스, DB시장 점유율 1위지만, 비용이 많이들고, 대기업에서 주로 사용한다.
2. MySQL: `MySQL`사에서 만든 오픈소스 데이터베이스, `Oracle`에 비해 대용량 데이터 처리는 어려움
3. PostgreSQL: 객체 관계형 데이터베이스 시스템, 오픈소스, 다양한 데이터베이스 객체를 사용자가 임의 생성가능
4. MariaDB 등등..
5. 열 = 필드 = 속성
6. 행 = 튜플 = 레코드

### ❏ NoSQL

1. `key-value`: `Redis`, `AWS DynamoDB`, `value`는 어떤 값이든 가능, 가장 단순한 형태
2. `doucment`: `DynamoDB`, `CouchDB`, 각 레코드가 하나의 문서가 됨, 문서는 데이터베이스에 따라 `XML`, `YAML`, `JSON`, `BSON` 등을 사용한다.
3. `graph-based`: `Neo4j`, `AWS Neptune`, 그래프 이론을 바탕으로 데이터베이스를 그래프로 표현한다. 관계기반문제에 유리함

### ❏ mongoDB CRUD

```javascript
// create
const users = client.db('fc21').collection('users')
    // delete, users collection은 항상 비워짐
await users.deleteMany({})

    // insert
await users.insertMany([
    {
        name: 'Foo'
    },
    {
        name: 'Bar'
    },
    {
        name: 'Baz'
    }
    ])
const cursor = users.find({})
await cursor.forEach(console.log)

// update
await users.updateOne(
    {
        name: 'Baz'
    },
    {
        $set: {
            name: 'Boo'
    }
}

// read
await users.insertMany([
    {
        name: 'Foo',
        birthYear: 2000,
    },
    {
        name: 'Bar',
        birthYear: 1995,
    },
    {
        name: 'Baz',
        birthYear: 2000,
    },
])

const cursor = users.find({ birthYear: 1995 });

// delete
await users.deleteOne({
    name: 'Baz',
})
```

### ❏ 관계형 데이터베이스(RDB)

1. 가장 고전적이고 널리 알려진 데이터베이스 모델
2. 데이터의 규격인 스키마(테이블)와 각종 제약 조건을 정하고, 그에 맞게 데이터 저장
3. 대부분의 경우 `SQL`로 상호작용한다.

```SQL
SELECT id, name FROM cities
INSERT INTO users (name, 'cityId') VALUES ('Bobo', 1)
UPDATE users SET name = 'Coco' WHERE name = 'bobo'
DELETE FROM users WHERE name = 'Coco'
```

4. `ORM(Object-relation-mapping)`: 객체와 관계형 데이터베이스의 데이터를 자동으로 매핑해주는 것(JPA, Hibernate 등)
5. `SQL injection`: 악의적인 사용자가 보안상의 취약점을 이용하여, 임의로 `SQL`문을 주입하고 실행하여 `DB`가 비정상적인 동작을 하도록 조작하는 행위

```javascript
// postgres - SQL injection
program.command('remove').action(async () =>
    {
        const client = await connect()
        const userName = await prompts({
            type: 'text',
            name: 'userName',
            message: 'Provide a user name to delete.'
 })
 // SQL injection이 가능한 지점
 const inserted = `' OR '' = '`

 // 모든 row 삭제
 const query = `DELETE FROM users WHERE name = '${inserted}'`
 console.log(query)

 // await client.query(query)
 await client.end()

 // prevent SQL injection
 await client.query(`DELETE FROM users WHERE name = $1::text`, [
 userName.userName])
```

6. `Sequelize`: 객체의 메서드를 활용하는 것처럼 쿼리 로직을 작성가능, Node.js 의 대표적인 ORM, Promise 기반으로 구현되었기 때문에 비동기 로직을 편리하게 작성할 수 있다.

### ❏ CRUD 사용자 추가하기

1. 웹의 성능을 포기해도 사용자가 편리하게 끔 만들자.
2. 데이터를 넣고 지우는것보다 전체를 새로 그려내는경우가 빠를 때가 있다.
3. `app.use(express.json())`: req.body에 값을 넣어준다. ()
4. `app.use(express.urlencoded({extended: false}))`: js 내부 모듈 중 `query-string` 모듈이 있는데 우리가 사용하기 편하게 분석해서 `req.body` 에 넣어주고. `extended: true` 를 사용하면 `qs` 모듈을 이용해서 `req.body` 에 넣어준다. (`query-string` 에 비해 보안성에서 뛰어나다?정도의 차이, 단점은 버전관리)
5. POST로 한글(유니코드)을 넘길때 몇몇 프록시에서 한글이 깨지는 경우가 있다. (대부분은 지원함)
6. 개발시 귀찮더라도 범용성있게 작성해야한다. (안되는 브라우저를 위해서)

---

## 📍 32일차 12.8.수. 온라인 강의

오늘은 `CRUD를 이용하여 게시판 만들기`,` Template Engine`, `Pug`, `PM2`을 배웠다. `node.js`의 기본언어는 `JS`인데, 한가지의 언어로 프론트와 백을 다룬다고 생각하니까 가슴이 웅장해졌다. (아직은 어색하지만..) 자주 살펴보며 눈에 익히는 것이 아무래도 좋겠지??

### ❏ 게시판 만들기

1. 웹 서비스 개발의 기본을 학습하기 좋다. 게시판을 통해 기본기를 잘 다지면 무엇이든 응용 가능
2. 게시판 목록, 보기, 수정, 작성, 삭제
3. 회원가입, 로그인, 비밀번호 찾기, pagination, 구글 로그인, 유저 작성글 모아보기

### ❏ Template Engine

1. 서버에서 클라이언트로 보낼 `HTML` 형태를 미리 템플릿으로 작성하고 동작시에 미리 작성된 템플릿에 데이터를 넣어 완성된 `HTML`을 생성한다.
2. 템플릿 엔진은 템플릿 작성 문법과 템플릿을 `HTML` 형태로 변환하는 기능을 제공한다.

![](https://images.velog.io/images/abcd8637/post/87224629-659a-4550-ac3d-4e76a6144652/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-08%2009.10.41.png)

3. `Express.js`의 템플릿엔진: `EJS`(html과 유사한 문법), `Mustache`(간단한 데이터 치환정도만 제공하는 경량화 된 템플릿 엔진), `Pug`(들여쓰기 표현식을 사용한 간략한 표기와 레이아웃 등 강력한 기능을 제공)

### ❏ Pug

1. 들여쓰기 표현식을 이용해 가독성이 좋고 개발 생산성을 높인다.
2. `HTML`을 잘 몰라도 문법적인 실수를 줄일 수 있다.
3. `layout`, `include`, `mixin` 등 강력한 기능을 제공한다.
4. `HTML` 닫기 태그 없이 들여쓰기로 블럭을 구분한다.
5. `=` 을 이용해 전달받은 변수를 사용할 수 있다.
6. `id` 나 `class` 는 태그 뒤에 이어서 바로 사용하고, `()` 를 이용해서 `attribute` 를 사용한다.
7. `each-in`: `for` 과 비슷한 태그
8. `if, else if, else` : 조건문

```pug
// index.pug
html
	head
		title= title   // title 변수 사용
	body
		h1#greeting 안녕하세요
		a.link(href="/") 홈으로

// each, if
each item in arr
	if item.name == 'new'
		h1 New Document
	else
		h1= `${item.name}`

// layout.pug
html
	head
		title= title
	body
		block content

// main.pug, 반복되는 웹사이트의 틀을 작성하고 extends하며 개발하면 매우 편리하다.
extends layout  // layout을 extends하면 block 부분에 작성한 HTML 태그가 포함됨
block content  // block을 포함한 템플릿은 layout으로 사용가능
	h1 Main Page

// include, layout은 바깥에 선언하고 가져다 쓰고, include는 조각을 만들어서 가져다 쓴다.
// 자주 반복되는 구문을 미리 작성하고 include하여 사용한다.
// 일반적인 텍스트파일도 include하여 템플릿에 포함 가능하다.

// title.pug
h1= title

// main.pug
extend layout
block content
	include titie
	div.content
		안녕하세요
	pre
		include article.txt

// mixin, 템플릿을 함수처럼 사용할 수 있다.
// include는 값을 지정할 수 없지만, mixin은 파라미터를 지정하여 값을 넘겨받아 템플릿에 사용할 수 있다.

// listItem.pug
mixin listItem(title, name)
	tr
		td title
		td name

// main.pug
include listItem
table
	body
		listItem('제목', '이름')
```

### ❏ Express.js와 pug의 연동

1. `app.set` 을 이용해 템플릿이 저장되는 디렉토리를 지정하고, 어떤 템플릿 엔진을 사용할지 지정할 수 있다.
2. `res.render` 함수는 `app.set` 에 지정된 값을 이용해 화면에 그리는 기능을 수행한다. `render` 함수의 첫 번재 인자는 템플릿의 이름, 두번째인자는 템플릿에 전달되는 값

```javascript
// app.js
app.set("views", path.join(__dirname, "views"));
app.set("view engine", "pug");

// request handler
res.render("main", {
    title: "Hello Express",
});
```

3. `app.locals` : `render` 함수에 전달되지 않은 값이나 함수를 사용할 수 있다. 템플릿에 전역으로 사용될 값을 지정하는 역할

```javascript
// app.js
app.locals.appName = "Express"

// main.pug
h1= appName
<h1>Express</h1>
```

### ❏ Express-generator 사용 시 템플릿 엔진 지정하기

1. `express-generator` 는 기본적으로 `jade` 라는 템플릿 엔진을 사용한다.
2. `jade` 는 `pug` 의 이전 이름으로, 최신 지원을 받으려면 템플릿 엔진을 `pug` 로 지정해야 한다.
3. `--view`: 템플릿 엔진을 지정할 수 있다.

```javascript
$ express --view=pug myapp
```

### ❏ 게시판 CRUD 만들기

1. 데이터를 다루는 네 가지 기본적인 기능
2. Create: 게시글 작성기능, 제목, 내용, 작성자, 작성 시간 등의 정보를 기록함, 게시글의 제목과 내용은 최소 n글자 이상이어야 함
3. Read: 게시글의 목록과 게시글의 상세를 볼 수 있어야 함. 목록은 간략화된 정보를 보여줌, 게시글 상세는 제목, 작성자, 내용, 작성 시간, 수정 시간 등의 상세한 정보를 보여줘야 한다.
4. Update: 게시글은 수정이 가능해야한다. 제목, 내용을 수정하고, 수정 시간을 기록한다. (게시글 수정은 작성자만 가능하다. + 회원기능)
5. Delete: 게시글 삭제하기, (게시글 삭제는 작성자만 가능하다. + 회원기능)
6. 모델선언하기: `ID` 는 url에 사용하기 좋은 값이 아니기 때문에 `shortId` 로 생성한다. 제목, 내용, 작성자를 `string` 타입으로 스키마에 선언한다.(작성자는 회원가입 후 실시) `timestamps`옵션으로 작성 시간, 수정 시간을 자동으로 기록해준다.

```javascript
// shortId 타입을 mongoose custom type으로 선언
// nanoid: 중복 없는 문자열 생성
// default를 이용해 모델 생성시 자동으로 아이디 생성
const { nanoid } = require("nanoid");

const shortId = {
    type: String,
    default: () => {
        return nanoid();
    },
    require: true,
    index: true,
};

module.exports = shortId;
```

### ❏ 게시글 작성 흐름

1. `/posts?write=true` 로 작성페이지 접근
2. `<form action="/posts" method="post">` 를 이용해 `post` 요청 전송
3. `[router.post](http://router.post)` 를 이용하여 `post` 요청 처리
4. `res.redirect` 를 이용하여 `post` 완료 처리

```javascript
// ./routes/posts.js
const { Router } = require('express');

const router = Router();

router.get('/', (req, res, next) => {
	if (req.query.write){
		res.render('posts/edit');  // write 값이 있으면 edit파일로 연결한다.
		return;
	}
	...
});

module.exports = router;

// ./views/posts/edit.pug
...
form(action='/posts', method="post")
	table
		tbody
			tr
				th 제목
				td: input(type='text' name='title')
			tr
				th 내용
				td: textarea(name='content')
			td
				td(colspan="2")
					input(type="submit" value="등록")

// ./routes/posts.js
const { Post } = require('./models);

router.post('/', async (req, res, next) => {
	const { title, content } = req.body;
	try{
		await Post.create({
			title,
			content,
	});
	res.redirect('/');  // 게시글 작성 후 홈 화면으로 이동하기
	} catch(err){
		next(err);
	}
}
```

### ❏ 게시글 목록 및 상세 흐름

1. `/posts` 로 목록 페이지 접근
2. `<a href='/posts/:shortId'>` 를 이용하여 상세 URL link
3. `router.get('/:shortId')` path parameter를 이용하여 요청을 처리함

```javascript
// ./routes/posts.js
// 처음 접속시 모든 리스트를 불러온다.
router.get('/', async(req, res, next) => {
	const posts = await Post.find({});
	res.render('/posts/list', { posts });  // posts/list에 { posts } 값이 넘어간다.
});

router.get('/:shortId', async(req, rse, next) => {
	const { shortId } = req.params;
	const post = await Post.findOne({ shortId });
	if(!post){
		next(new Error('Post notfound!');
		return;
	}
	res.render('posts/view', { post });  // posts/view로 값 보내기
});

// ./views/posts/list.pug
...
	table
		tbody
			each post in posts  // each로 반복문 돌기
				tr
					td
						a(href='/posts/${post.shortId}') = post.title
					td= post.author
					td= formatDate(post.createdAt)  // formatDate: custom function
		tfoot
			tr
				td(colsapn='3')
					a(href="/posts?write=true") 등록하기

// app.js
// dayjs 패키지 사용
const dayjs = require('dayjs');
app.locals.formatDate = (date) => {
	return dayjs(date).format('YYYY-MM-DD HH:mm:ss');
}

// ./views/posts/view.pug
...
	table
		tbody
			tr
				td(colspan="2")= post.title
			tr
				td= post.author
				td= formatDate(post.createdAt)
			tr
				td(colspan="2"): pre= post.content
			tr
				td: a(href='/posts/${post.shortId}?edit=true') 수정
				td button(onclick=`deletePost("${post.shortId}")`) 삭제
```

### ❏ 게시글 수정 흐름

1. `/posts/{shortId}?edit=true` 로 수정페이지 접근
2. 작성페이지를 수정페이지로도 동작하도록 작성
3. `<form action="/posts/:shortId" method="post">` 를 이용해 `post` 요청 전송
4. html form 은 `PUT method`를 지원하지 않기 때문에 `post` 사용
5. `res.redirect` 는 항상 GET요청으로 넘어간다.

```javascript
// ./routes/posts.js
router.get('/:shortId', async (req, res, next) => {
	if (req.query.edit){
		res.render('posts/edit', { post });
	}
	...
});

// 수정 요청 처리하기
router.get('/:shortId', async (req, res, next) => {
	const { shortId } = req.params;
	const { title, content } = req.body;
	const post = await Post.findOneAndUpdate({ shortId }, { title, content })  // shortId를 찾아 새로운 title, content로 바꾸겠다.
	if(!post){  // 상세 post가 없으면
		next(new Error('Post notfound');
		return;
	}
	res.redirect(`/posts/${shortId}`);  // redirect는 항상 GET요청으로 넘어간다.
});

// ./views/posts/edit.pug
...
	- var action = post ? `/posts/${post.shortId}` : "/posts"  // post가 있는 경우에는 상세 페이지로 이동, 그렇지 않은 경우는 작성하기 위한 URL로 보낸다.
	form(action=action, method="post")
		table
			tr
				th 제목
				td: input(type="text" name="title" value=post&post.title) // post가 있으면 제목을 post.title로 채우기
			tr
				th 내용
				td: textarea(name="content")= post&&post.content  // post가 있으면 내용을 post.content로 채우기
			td
				td(colspan="2")
					- var value = post ? "수정" : "등록"
					input(type="submit" value=value)
```

### ❏ 게시글 삭제 흐름

1. 게시글 상세 페이지에 삭제 버튼 추가
2. `html form` 은 DELETE 메서드를 지원하지 않음
3. `JS` 를 이용해 `fetch` 함수로 `HTTP Delete` 요청 전송
4. `router.delete` 의 응답을 `fetch` 에서 처리

```javascript
// posts/view.pug
td
	button.delete(onclick='deletePost("${post.shortId}")') 삭제

// delete.pug, promise로 실행된다.
script(type="text/javascript").
	function deletePost(shortId){
		fetch('/posts/' + shortId, { method: 'delete' })
			.then((res) => {
				if (res.ok) {
					alert('삭제가 완료되었습니다.');
					window.location.href='/posts';  // 삭제 완료 후 게시글 목록으로 이동
				}else{
					alert('오류가 발생했습니다.');
					console.log(res.statusText);
				}
			})
		.catch((err) => {
			console.log(err);
			alert('오류가 발생했습니다.');
		});
}

// 삭제 요청 처리하기
// ./routes/posts.js
router.delete('/:shortId', async (req, res, next) => {
	const { shortId } = req.params;
	try{
		await Post.delete({ shortId });  // mongoDB 내 해당 데이터 삭제
		res.send('OK');
	}catch(e){
		next(e);
	}
});
```

### ❏ Async Request Handler

1. 공식적으로 사용되는 `express` 기술은 아니고 패턴 중 하나임.
2. `async` 함수를 조금 더 쉽게 사용할 수 있고, 비동기 실행 중 오류 처리를 더 간단하게 할 수 있는 장점이 있다.
3. `request handler` 에서 오류를 처리하기 위한 방법 (`promise().catch(next)`, `async function, try - catch, next`)
4. `async` 의 비동기 처리는 매우 편리하지만, 매번 `try-catch` 구문을 작성하는 것은 귀찮고 실수하기 쉬움 따라서 `request handler` 를 `async function` 으로 작성하면서 `try-catch next` 를 자동으로 할 수 있도록 구성한 아이디어
5. `asyncHandler` 는 `requestHandler` 를 매개변수로 갖는 함수형 미들웨어, 전달된 `requestHandler` 는 `try-catch` 로 감싸져 `asyncHandler` 내에서 실행되고, `throw` 되는 에러는 자동으로 오류처리 미들웨어로 전달되도록 구성됨.
6. 오류처리를 올바르게 사용하지 않으면 `express` 앱이 종료될 수 있다.
7. `next` 인자는 제거하고 `try-catch` 구문을 제거해도 동일하게 오류 처리가 가능하다.

```javascript
const asyncHandler = (requestHandler) => {
	return async (req, res, next) => {
		try{
			await requestHandler(req, res);
		}catch(err){
			next(err);
		}
	}
}

router.get('/', asyncHandler(async (req, res) => {
	const posts = await Post.find({});
	if (posts.length < 1){
		throw new Error('Not found');
	}
	res.render('posts/lists', { posts });
});

// 실제 적용 코드(next 인자는 빼줘야한다.)
// posts.js
const { Router } = require('express');
const { Post } = require('../models');
const asyncHandler = require('../utils/async-handler');

const router = Router();

router.get('/', asyncHandler(async (req, res) => {
  if (req.query.write) {
    res.render('post/edit');
    return;
  }

  const posts = await Post.find({});

  res.render('post/list', { posts });
}));

router.get('/:shortId', asyncHandler(async (req, res) => {
  const { shortId } = req.params;
  const post = await Post.findOne({ shortId });

  if (req.query.edit) {
    res.render('post/edit', { post });
    return;
  }

  res.render('post/view', { post });
}));

router.post('/', asyncHandler(async (req, res) => {
  const { title, content } = req.body;

  if (!title || !content) {
      throw new Error('제목과 내용을 입력해 주세요');
  }

  const post = await Post.create({ title, content });
  res.redirect(`/posts/${post.shortId}`);
}));

router.post('/:shortId', asyncHandler(async (req, res) => {
  const { shortId } = req.params;
  const { title, content } = req.body;
  if (!title || !content) {
      throw new Error('제목과 내용을 입력해 주세요');
  }

  await Post.updateOne({ shortId }, { title, content });
  res.redirect(`/posts/${shortId}`);
}));

router.delete('/:shortId', asyncHandler(async (req, res) => {
  const { shortId } = req.params;
  await Post.deleteOne({ shortId });
  res.send('OK');
}));

module.exports = router;
```

### ❏ Pagination

1. 데이터가 많아지면 한 페이지의 목록에 모든 데이터를 표현하기 어려움. 따라서 데이터를 균일한 수로 나누어 페이지로 분리하는 것(ex, 10개씩 나누어 1페이지는 10~20, 2페이지는 11~20번까지 보여주기)
2. `page`: 현재 페이지, `perPage`: 페이지 당 게시글 수
3. `/posts?page=1&perPage=10` 처럼 `url query` 를 사용해 전달, `url query` 는 문자열로 넘어가기 때문에 사용시 `number` 로 형 변환을 해줘야 한다.

```javascript
router.get( => {
	const page =
			Number(req.query.page || 1)  // `page`가 없으면 default 1
	const perPage =
			Number(req.query.perPage || 10)  // `perPage`가 없으면 default 10
})
```

4. `mongoDB` 의 `limit`, `skip` 을 사용하여 구현도 가능하다. (`limit`: 검색 결과 수 제한, skip: 검색 시 포함하지 않을 데이터 수)

```javascript
// 데이터의 순서가 유지 될 수 있도록 sort를 사용한다.
// 최신순으로 정렬하고 처음부터 몇개의 게시물을 제외시키고 나머지 게시물은 몇개씩 가져오는지
router.get(... => {
	const total = await Post.countDocument({});
	const posts = await Post.find({})
		.sort({ createdAt: -1 })  // 최신순정렬
		.skip(perPage * (page - 1))
		.limit(perPage);
	const totalPage = Math.ceil(total / perPage);  // 게시글 수 / 페이지 당 게시글 수 = 총 페이지 수
})

// pug
// patination이 필요한 페이지에서 해당 템플릿을 include한 후, + pagination으로 mixin을 사용 함.
// 현재 페이지는 b 태그로 굵게 표시
mixin pagination(path)
p
  - for(let i=1; i<=totalPage; i++)
		a(href=`${path}?page=${i}&perPage=${perPage}`)
			if i == page
				b= i
			else
				= i
      = " "

include pagination
tr
	td
		+pagination("/posts")
```

### ❏ PM2 (Process Manager)

1. `Node.js` 의 작업을 관리해주는 `Process Manager`
2. `node` 명령어로 실행 시 오류 발생이나 실행 상태 관리를 할 수 없음
3. `pm2` 는 작업 관리를 위한 다양한 유용한 기능을 제공해 줌
4. 안정적인 프로세스 실행: 오류발생 시 자동 재실행
5. 빠른 개발환경: 소스 코드 변경 시 자동 재실행
6. 배포 시 편리한 관리: pm2에 모든 프로세스를 한 번에 관리
7. `pm2 init simple`, `pm2 init` 이후 `pm2 start` 명령어 실행 개발 시 `watch` 옵션 사용하여 파일 변경 시 서버 자동 재실행 구성

```javascript
// ecosystem.config.js
module.exports = {
	apps: [{
		name: 'simple-board',
		script: './bin/www',
		watch: '.',  // 모든 경로를 바라본다.
		ignore_watch: 'views',
	}],
}

$ pm2 start
```

---

## 📍 33일차 12.9.목. 실시간 강의

오늘은 `graphQL`, `인증`에 대해서 배웠다. 실습시간 마지막에는 `HTTP / HTTPS(SSL)`의 차이, `cookie-session, JWT` 방식의 차이에 대해서 알려주셨는데 너무 유익했다. `restAPI`와 `graphQL`의 차이는 내겐 스승과도 같으신 <a href='https://blog.toycrane.xyz/rest-api%EA%B0%80-%EA%B0%80%EA%B3%A0-graphql%EC%9D%B4-%EC%99%94%EB%8B%A4-a9e400b77902'>튜터님</a> 미디움을 참고하면 도움이 많이 된다.

### ❏ REST API vs gql API

1. `gql` 은 하나의 `Endpoint` 만 존재
2. `REST API` 는 `End point` 마다 데이터베이스 `SQL` 쿼리가 달라짐
3. `gql API` 는 `gql` 스키마의 타입마다 데이터베이스 `SQL` 쿼리가 달라짐

### ❏ GraphQL

1. FACEBOOK에서 2015년에 발표한 새로운 api 규격
2. `type system` 을 기본적으로 갖추고 있어서 `REST` 보다 훨씬 안정적
3. `Apollo`, `Prisma` 등 방대하고 강력한 오픈 소스 툴들로 양질의 개발자 경험 개선을 기대한다.
4. `SDL(Schema Definition Language)` : 서버에 무엇을 질의하여 값을 돌려받기를 원할 때 `SDL`로 기술(명확한 타입을 정의하여 기술)
5. `CLI` 로 `post` 요청시 쌍 따옴표를 빼도 보내진다.

### ❏ OAuth

1. 접근권한 위임을 위한 공개 표준
2. 유저 진입장벽이 매우 낮아짐(원클릭으로 로그인 가능)
3. 유저가 비밀번호를 기억할 필요가 없어짐
4. 유저 허용 여부에 따라 이메일, 프로필 사진, 닉네임 등의 기본 정보를 얻을 수 있다.

### ❏ 기타 내용들

1. 프로젝트를 할 때 `F/E` 를 나누기보다는 기능별로 담당하자(ex, `login + front + back` / `pay + front + back`)과 같이 수평적으로 제작)
2. 프론트와 백을 나눠서 개발하면 속도에서 차이가 난다. (처음은 백엔드가 느리다. DB, 보안, 인프라 등등... 나중엔 반응형때문에 프론트 개발 속도가 늦어진다. 서로 의견충돌이 난다. 즉, 전체적인 프로젝트가 늦어지기 때문에 친한친구나 숙련된 분들과 하면 기능별로 쪼개서 개발하는것을 권장한다.)
3. 템플릿 엔진: `html` 코드인데, 그 안에서 반복, 조건절로 `view` 를 만들어줄 때 사용한다.(일일이 따로 만들면 중복되는 코드가 많기 때문에 로직을 붙여서 자동으로 `html` 코드를 만들어줄 때) `EJS`, `JADE -> PUG` , `nunjunks` 사용빈도: `nunjunks` → `EJS`

```javascript
1. nunjunks: EJS의 상위호환(html을 닮음), junja2의 영향을 받음(flask에서 나온?)
2. EJS: html을 닮음
3. pug: 문법이 특이해서 따로 공부해야함
```

4. `passport` : 로그인 구현시 편리하게 도와주는 친구, 이게 없으면 `header`, `session` 관리를 직접 해줘야 한다. 써드파티 로그인도 지원한다.
5. 로그인 혹은 마이페이지를 보여주는 기능 등의 서버로부터 인증을 받아야하는 상황일 때 선택지는 크게 3가지 `cookie`, `cookie - session` , `JWT` 방식이 있다. 서버는 절대 한개로 운영하지 않고, 2개 이상으로 운영되는데 요청은 한 곳에서 들어온다. 이때 요청을 여러개의 서버 중 한곳으로 분배해주는 장치가 필요한데, 이것이 `LB(load balancer` 다. `AWS` 에서는 `ELB(elastic load balancer)` 라고 부른다.( `elastic: 탄력적인, 고무의`), `cookie-session` 는 `DB` 가 필요하고, `JWT` 는 `DB` 가 필요하지 않다.
6. `cookie` 방식은 클라이언트에 저장되는 `key - value` 로 이루어진 데이터다. 인증 유효시간을 설정할 수 있고, 유효시간이 정해진다면 클라이언트가 종료되어도 쿠키가 유지된다. 그러나, 중요정보를 쿠키에 담고있으므로 해커에게 탈취당하면 사용자의 정보를 모두 빼앗길 수 있다. 그래서 쿠키자체로는 보안과는 상관없는 개인 장바구니, 자동로그인 설정 등에 사용한다.
7. `cookie-session` 방식은 `client` 에서 요청을 보내면 `server` 에서 `cookie` 의 값을 가지고 있다가 `cookie` 와 일치하는 `session` 을 해당 서버에서 찾고 `cookie` 를 사용자에게 보내준다. 그런데, 여러개의 서버가 연결되어있다고 가정해보자. `server 1`에 현재 `cookie`를 가지고 있다가 연결이 끊겨 다시 `LB` 를 거쳐가서 2번째 `server` 로 연결이 되면, `cookie` 가 없기 때문에 지금 요청한 사용자가 인가된 사용자인지 모른다. 이럴 때는 서버에 `session` 데이터를 저장하지않고, `DB`(redis) 를 이용해 해당 `session` 데이터를 `DB` 에 저장한다. `DB` 에서 쿠키에 맞는 세션데이터를 찾고 해당하는 데이터가 있으면 리퀘스트를 돌려준다. `DB` 단이 붙었기 때문에 요청량이 많아지면 시간이 오래 걸릴 수 있다.
8. `JWT` 방식은 `cookie-session` 방식과 다르게 `DB` 단이 필요없다. `JWT` 는 일종의 신분증이라고 생각하면 편하다. `JWT` 는 `JSON web Token` 를 뜻하는데, 토큰의 특성상 위조가 상당히 어렵다. 그러나 한번 탈취되면 보안에 굉장히 취약해진다. 이를 방지하고자 만료시간이 생겼다. 이때 만료시간은 보통 5-30분 길면 1주일정도로 세팅한다. 요청이 오면 `JWT` 를 발급해준다. `mypage` 로 요청이 날라오면 요청과 함께 온 `JWT` 가 위조되었는지 확인한다. 서버에 저장되어있는 `JWT` 와 일치하면 `mypage` 요청을 같이 보내준다. `cookie-session` 방식처럼 `DB` 단에서 세션 데이터를 확인할 일이 사라진다.
9. `http` (80), `https` (443): 보안 유무, `get` 은 `URL` 에 `post` 는 `http.body` 에 요청이 넘어간다. 그래서 `http.body` 도 `postman` 같은 프로그램으로 열어볼 수 있다. 따라서 `http` 에서 `get`, `post` 의 보안은 안전하지 않다.(`id`, `pw`, `cookie` 가 평문으로 날아간다.) 특히, `cookie` 를 도청하게 되면 다른 사이트에서 재사용할 수 있따. (`cookie` 는 로그인을 성공한 사람에게 넘겨주기때문에 노출되면 위험하다.) `https` 는 이런 `id`, `pw`, `cookie` 가 암호화가 되어 서버로 날아간다. 그래서 중간에 해커가 탈취하기 힘들다. `curl` 명령어
10. `http -> https`: `DNS` 가 담당한다. `http` 로 요청이 날라오면 `DNS` 에서 다시 클라이언트로 반송처리 시키고 클라이언트에서 `DNS` 한테 `https` 로 요청하게 된다. `server` 에서 `client` 로 갈 때 `https` 로 변환한다.(항상 그런것은 아니고 대부분 캐싱이 되어있어서 중간에 다시 옴)
11. `SSL` 인증서: 이 사이트가 안전한지 확인하는 인증서(대표적으로 `AWS` certificate manager에서 발급해준다. 인증기관에 비용을 지불하면 `DNS` 에 붙여준다. 만약, `SSL` 인증서가 없으면 다시 브라우저로 리턴하거나 에러를 발생시킨다.)
12. `node template engine` 은 서버에서 파일을 보내줘서 브라우저단에서 띄우기만 한다. 이런 방식은 `SSR`, 반대로 `CSR` 은 리액트에서 파일을 만들고 데이터만 서버에 요청해서 둘다 합치면 `CSR` 이 된다.
13. `SSR` 은 검색엔진이 데이터를 모두 읽을 수 있다. `CSR` 은 파일을 한번 거쳐서 탐색해야하기 때문에 바로 노출이 되진 않는다(feat. CORS)
14. 리액트는 노드서버에 직접 요청해서 받아오는것은 아니다. 그냥 브라우저로 데이터를 보내주고 데이터는 브라우저에서 서버로 요청하여 브라우저에서 취합한다.
15. 로그인처럼 `DB` 사용하는건 `node.js` 사용하고, 보여주기만 할거면 `CSR`
16. 실 서비스할때는 내부 웹서버보다 `nginx`를 직접 붙이는 편이 더 좋다. `node.js` 는 내부 웹서버도 배포하기 충분하다.
17. `AWS - route 53` 에서 `DNS` 에 `SSL` 을 직접 붙인다. `ELB` 에도 `SSL` 을 붙여야한다. 이후 뒷단에 있는 `EC2` 서버로 넘어간다.
18. `ELB` 를 쓰는 이유는 `autoScaling` 을 쓰기 위함이다.
19. 인스턴스를 늘릴 때는 사용률이 51%를 넘어섰을 때 이때 서버가 터져버리면 다음서버는 `@ + 51%` 가 되는데 다음 서버가 50이면 서버가 터져버린다.

---

## 📍 34일차 12.10.금. 온라인 강의

오늘은 `회원가입`, `passport.js`, `session-store`, `댓글 기능`을 배웠다.

### ❏ 회원가입

1. 이메일, 이름, 패스워드의 간단한 정보만 사용(이메일 형식이 올바른지 확인, 비밀번호 최소 길이 설정, 패스워드와 패스워드 확인 문자가 일치하는지 확인)
2. 회원의 비밀번호를 `DB`에 그대로 저장하면, 관리자가 모든 회원의 비밀번호를 알 수 있고, `DB`가 해킹되면 보안 취약점이 발견하게 되므로 `hash`값으로 비밀번호를 저장한다.(`hash`는 문자열을 되돌릴 수 없는 방식), 비밀번호의 `hash`값을 `DB`에 저장하고, 로그인 시 전달된 비밀번호를 `hash`하여 저장된 값과 비교해 로그인을 처리한다.
3. `node.js`의 기본제공 모듈인 `crypto` 모듈을 사용하여 `hash` 값을 얻을 수 있다. 간단하게 `sha1` 알고리즘을 사용하거나, 보다 강력한 `sha224`, `sha256` 등의 알고리즘도 사용할 수 있다.

```javascript
const hash = crypto.createHash("sha1");
hash.update(password);
hash.digest("hex");
```

4. 회원가입 페이지 구현 -> `script`를 이용해 이메일 형식, 비밀번호 확인 문자 -> `form`을 이용해 `post` 요청 전송 -> 회원가입 처리 및 `redirect`

```javascript
// 비밀번호 hash 값 저장
// 이미 존재하는 회원인지 체크
// 가입 후 메인화면으로 redirect

router.post(... => {
	const { email, name, password } = req.body;
	const pwHash = getHash(password);
	const exists = await User.findOne({ email })

	if (exists){
		throw new Error("이미 가입된 메일입니다.");  // try - catch 문이 아니므로 async request handler를 사용한다.
	}

	await User.create({
		email,
		name,
		password: pwHash,
	})

	res.redirect('/');  // 메인화면으로 보내기
})
```

### ❏ passport란?

1. `express.js` 어플리에키션에 간단하게 사용자 인증 기능을 구현하게 도와주는 패키지, 유지 세션 관리 및 다양한 로그인 방식 추가 기능 제공
2. `passport-local`: 다양한 로그인 방식을 구현하기 위해 `strategy`라는 인터페이스를 제공한다. `strategy`는 인터페이스에 맞게 설계된 다양한 구현체(facebook, google, ...)들이 있다. `passport-local` 은 `username`, `password`를 사용하는 로그인 구현체를 의미한다.

```javascript
1. 로그인 화면 구성
2. passport-local strategy로 로그인 구현하기
3. passport.js 설정하기
4. passport로 요청 처리하기

// passport-local stratgy
// config 정보 전달 -> authenticate 실행(config를 인자로 전달받음 이메일, 패스워드, 완료처리 콜백함수(done)) -> 데이터 찾기

const config = {
	usernameField: 'email',
	passwordField: 'password',
}

const local = new LocalStrategy(config, )

..., async(email, password, done) => {
	try{
		const user = await User.findOne({ email });
		if(!user){
			throw new Error("회원을 찾을 수 없읍니다.");
		}

		if(user.password !== getHash(password)){
			throw new Error("비밀번호가 일치하지 않읍니다.");
		}

	// 세션에 저장되는 유저 정보의 최소화
    // 첫 번째 인자: error, 두번째인자: data
		done (null, {
			shortId: user.shortId,
			email: user.email,
			name: user.name
		});
	}catch(e){
		done(e, null)
	}
}

// passport.js
// 작성한 strategy를 passport.user를 이용해 사용하도록 선언해야 함
// passport.use를 이용해 strategy를 사용하도록 선언한 후 passport.authenticate를 사용해 해당 strategy를 이용해 요청을 처리할 수 있음
const local = require('./strategies/local');
passport.use(local);

// routes/auth.js
router.post('/',
	passport.authenticate('local');
...

// app.js
// passport.authenticate 함수를 http 라우팅에 연결하면 passport가 자동으로 해당하는 strategy를 사용하는 request handler를 자동 생성
// express-session과 passport.session()을 사용하면 passport가 로그인 시 유저 정보를 세션에 저장하고 가져오는 동작을 자동으로 수행해 줌
const session = require('express-session');
app.use(session({
	secret: 'secret',
	resave: false,
	saveUninitialized: true,
}));

app.use(passport.initialize());
app.use(passport.session());
app.use('/auth', authRouter);

// session 유저 활용하기
// session을 이용해 user를 사용할 때는 serializeUser와 deserializeUser를 설정한다.
// 이는 세션에 user정보를 변환하여 저장하고 가져오는 기능을 제공한다.(회원 id만 세션에 저장하고 사용 시 회원정보를 디비에서 찾아서 사용)
// 세션 사용 시 위 두 함수를 작성하지 않으면 passport 로그인이 동작하지 않음
passport.serializeUser((user, callback) => {
	callback(null, user)
})

passport.deserializeUser((obj, callback) => {
	callback(null, obj)
})

// logout
// passport는 req.logout 함수를 통해 세션의 로그인 정보를 삭제하여, 로그아웃 기능을 구현할 수 있다.
router.get('/logout', ... {
	req.logout();
	res.redirect('/');
})

// login 확인 미들웨어
// 로그인을 필수로 설정하고 싶은 경우, 미들웨어를 사용하여 체크할 수 있음
function loginRequired(req, res, next){
	if(!req.user){
		res.redirect('/');
		return;
	}
	next();
}

app.use('/posts', loginRequired, postsRouter)  // 로그인이 확인되면 postsRouter로 넘어간다.
```

### ❏ Session

1. 웹 서버가 클라이언트의 정보를 클라이언트별로 구분하여 서버에 저장하고, 클라이언트 요청시 `session ID`를 사용하여 클라이언트의 정보를 다시 확인하는 기술(클라이언트가 정보를 저장하고 요청시 정보를 보낸 `Cookie`와 대조 됨)
2. 서버는 세션을 생성하여 세션의 구분자인 `session ID`를 클라이언트에 전달함. 클라이언트 요청시 `session ID`를 함께 담아서 전송, 서버는 전달받은 `session ID`로 해당하는 세션을 찾아 클라이언트 정보를 확인함
3. `express-session` 패키지를 사용하여 간단하게 `session` 동작을 구현할 수 있다. 특별한 설정 없이 자동으로 `session`동작을 구현해줌, ㅈ동으로 `session ID`를 클라이언트에게 전달, `session ID`로 클라이언트 정보 확인

### ❏ Session Store를 사용하는 이유

1. `express-session` 패키지는 `session` 을 기본적으로 메모리에 저장함. 따라서 현재 구현된 어플리케이션을 종료 후 다시 실행하면 모든 유저의 로그인 해제됨, 혹은 서버가 여러 대 있을 경우, 서버 간 세션정보를 공유할 수 없음

### ❏ MongoDB - Session Store

1. `connect-mongo` 패키지를 이용해 `MongoDB` 를 `session store` 로 사용할 수 있다.
2. `connect-mongo` 패키지는 `express-session` 패키지의 옵션으로 전달 가능하다. 자동으로 `session` 값이 변경될 때 `update` 되고 `session` 이 호출될 때 `find` 함
3. 재부팅되어도 `data` 가 삭제되지 않기 때문에 `session-data` 를 유지 할 수 있다.
4. 세션데이터를 몽고디비에 저장하고 관리하는 기능을 자동으로 수행해 줌

```javascript
// connect-mongo 패키지를 이용해 express-session 설정시 store 옵션에 전달 및 mongoUrl 설정
const mongoStore = require('connect-mongo');

app.use(session({
	secret: 'secret',
	resave: false,
	saveUninitialized: true,
	store: mongoStore.create({
		mongoUrl: 'mongoUrl',
	}),
});
```

### ❏ 회원과 게시글의 연동

1. 게시글 작성시 로그인된 회원 정보를 작성자로 추가

```javascript
// PostSchema에 author 추가
// populate를 사용하기 위해 ObjectID 사용
// ref를 유저 모델의 이름은 'User'로 선언
author: {
	type: Schema.Types.ObjectId,
	ref: 'User',
	required: true,
}

// 게시글에 작성자 추가
// req.user에는 straegy에는 최소한의 정보인 shortId, email, username만 가지고 있다.
// Post 생성 시 user의 ObjectID를 전달해야하는데, User에서 shortId로 회원을 검색하여 한 번 더 검증
// 객체가 주어지면 자동으로 ObjectID 사용
const author = await User.find({
	shortId: req.user.shortId,
})

if(!author){
	throw new Error('No User')
}

await Post.create({
	title,
	content,
	author,  // author만 들어가있는게 아니고 user객체 data전체가 들어가는데, mongoDB가 여기서 _id만 꺼내서 저장해준다.
})
```

2. 게시글 - 작성자는 populate 하여 사용하도록 구현

```javascript
// populate
// 자동으로 user collection에서 author를 찾아서 넣어준다.
const posts = await Post.find({}).populate("author");

res.render("posts/list", { posts }); // posts를 반복문으로 꺼내 쓸 수 있다.
```

3. 게시글 수정, 삭제 시 로그인된 유저와 작성자가 일치하는지 확인

```javascript
// 수정, 삭제 시 유저 확인
const post = await Post.find({ shortId }).populate("author");

if (post.author.shortId !== req.user.shortId) {
    throw new Error("Not Authorized");
}
```

4. 작성자의 게시글 모아 보기 기능 구현: 기본적으로 `MongoDB` 는 `Document` 검색 시 전체 문서를 하나씩 확인하기 때문에 매우 비효율적인 검색을 수행한다. 데이터가 많아질 경우 속도 저하의 큰 원인이 된다. 검색을 위해 `Document` 를 정렬하는 기능을 제공함. index 를 설정하면 주어진 쿼리를 효율적으로 수행하여 성능을 향상시킬 수 있다.

```javascript
// index: true 옵션을 사용하면 mongoose가 자동으로 MongoDB에 인덱스를 생성해줌
// 이미 데이터가 많을 때 index 추가시 작업시간이 길어져 MongoDB가 응답하지 않을 수 있다. 예상되는 인덱스를 미리 추가하는 것이 좋음(처음부터 설정))
author: {
	type: Schema.Types.ObjectId,
	ref: 'User',
	required: true,
	index: true,
}
```

5. 회원 게시글 라우팅 추가하기: RESTful 한 구성을 위해 /users/{userId}/posts 로 구성, 게시글 목록 view 는 기존에 작성한 posts/list.pug 를 재활용

```javascript
// /routes/users.js
router.get('/:shortId/posts', ... => {
	const { shortId } = req.params;
	const user = await User.find({ shortId });
	const posts = await Post
			.find({ author: user })
			.populate('author');
	res.render('posts/list', { posts, user });
})

h2= user ? `${user.name}의 게시글` : `전체 게시글`
td: a(href=`/users/${post.author.shortId}/posts`)
	= post.author.name
```

### ❏ CSR로 댓글 기능 구현하기

1. 페이지 로드 시 필요한 리소스를 클라이언트에 선언(HTML Template, 브라우저에 표시되지 않는 HTML element를 작성해두고 JS로 이를 화면에 반복적으로 그릴 수 있게 하는 기술)
2. 클라이언트에서 필요한 데이터를 비동기 호출
3. 클라이언트가 전달받은 데이터를 가공, 리소스를 사용하여 화면에 표시
4. `HTML template` 사용하여 한 개의 댓글이 표시될 모양을 선언(JS로 조작하기 위해 `id`, `class` 를 선언하는 것이 유용하다)
5. `CSR` 을 구현하기 위해서는 `HTML` 이 아닌 데이터만 주고받을 수 있는 `API` 를 구성해야한다.(JSON 사용), 댓글 작성 시 댓글목록을 다시 불러와 그리는 형식으로 구현
6. `sub-schema` 를 이용하여 `Post` 스키마에 `Comment` 를 배열로 추가

```javascript
const CommentSchema = new Schema({
	content: String,
	author: {
		type: Schema.Types.ObjectId,
		ref: "User",
	},
}, {
	timestamps: true
});

const PostShema = new Schma({
	...
	comments: [CommentSchema],
  ...
})
```

7. 댓글 작성: `api/posts/{postId}/comments` 경로로 댓글 작성 기능 구현, 게시글 업데이트시 `${push}` 를 사용하여 `comments` 배열에 새로 작성된 댓글 추가(동시에 들어오는 요청을 정확하게 처리), `api` 는 `render` 대신 `json` 으로 응답

```javascript
// 댓글 업데이트
await Post.updateOne(
    { shortId },
    {
        $push: {
            comments: {
                content,
                author,
            },
        },
    }
);

res.json({ result: "success" });

// 댓글 목록
// find에 populate하지 않고, User (model)의 populate를 사용하는 방법도 가능
await User.populate(posts.comments, {
    path: "author",
});
```

8. 비동기 HTTP 요청은 `fetch` 함수를 이용함.

```js
// 댓글 작성하기
// 호출 결과의 성공 여부를 확인하여, 댓글 다시 불러오기 실행
fetch('url', {
	method: "post",
	headers: { ~ },
	body: JSON.stringify({ content }),
})
```

### ❏ MongoDB Aggregation

1. MongoDB에서 Document들을 가공, 연산하는 기능
2. RDMBS에서 SQL로 수행할 수 있는 기능들을 유사하게 구현할 수 있음 (SQL의 GROUP BY, DISTINCT, COUNT, JOIN 등)
3. mongoDB의 find는 검색 필터링과 정렬 이외의 기능을 제공하지 않음, 다른 collection에서 데이터를 가져오거나, 그룹화할때는 Aggregation을 통해 이를 수행할 수 있음

---

## 📍 35일차 12.11.토. 온라인 강의

오늘은 `JWT` 그리고 회원 비밀번호 찾기, `SMTP`를 이용하여 메일 발송기능, 비밀번호 초기화, `OAuth`, 웹 서버 소프트웨어인 `Nginx`에 대해서 배웠다. 나중에 로그인 관련 기능을 구현할 때 써먹으면 도움이 되는 내용이라서 까먹지 않고 기억해야겠다.

### ❏ JWT(Json Web Token)

1. 인증을 위한 정보를 특별한 저장소를 이용하지 않고, 전자 서명을 이용하여 확인하는 방법
2. `header`(토큰의 타입(jwt), 데이터 서명방식), `payload`(전달되는 데이터), `signature` (헤더와 페이로드의 전자서명)로 구성되어 있다.
3. `JWT` 는 `Web Token`, 데이터를 웹에서 사용하기 위한 스펙이므로 웹에서 문제없이 사용할 수 있는 문자열로만 구성된 `base64` 인코딩을 사용한다.
4. `JWT` 의 `payload` 는 단순히 정보를 `base64 encode` → `decode` 시 정보가 노출된다 → 민감한 정보는 제외하고 토큰을 생성한다.
5. 서버는 `JWT` 를 생성할 때, 비공개키를 이용하여 서명을 함. `payload` 를 조작할 경우 서명(signature)이 일치하지 않기 때문에 인증 실패
6. 사용자 로그인 → 서버는 로그인된 유저 정보를 JWT 로 생성하여 클라이언트에 전달 → 클라이언트는 전달받는 JWT 를 이용하여 인증이 필요한 요청에 사용

![](https://images.velog.io/images/abcd8637/post/080642e9-3012-4b15-8761-b2bc72473699/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-11%2009.31.32.png)

### ❏ JWT 사용 이유

1. `session` 은 기본적으로 웹 브라우저를 위한 통신 스펙
2. 모바일 앱 등, 웹 브라우저가 아닌 어플리케이션의 경우 `session` 을 활용하기 부적합함, `JWT` 를 사용하면 어느 클라이언트에서나 동일한 방식의 사용자 인증을 구현 가능

### ❏ JWT + Cookie

1. `cookie`: 웹 서비스에서 사용하는 정보를 클라이언트(브라우저)에 저장하고, `HTTP` 요청시 이를 함께 전송하여 클라이언트 정보를 서버에 전달하는 기술
2. `session`: 클라이언트 정보를 서버 측 저장소에 저장하고 사용(`session id` 로 `session store` 에서 확인해서 클라이언트 정보를 확인함),
3. `session` 을 사용한 유저 로그인: `cookie에 session ID` 저장 → `session store` 에서 유저 정보 가져오기
4. `JWT` 를 쿠키처럼 사용하는 경우: `JWT` 로 요청 → 서명 확인 후 유저 정보 사용(DB 접근이 한단계 줄어서 효율적인 인증 구현 가능)
5. 로그인 로직에서 `JWT` 생성 후 쿠키로 전달 → `passport-jwt` 패키지로 `JWT 로그인 미들웨어` 작성 및 사용

```js
// token 생성 및 미들웨어 선언하기
setUserToken = (res, user) => {
	const token = jwt.sign(user, secret);
	res.cookie('token', token);  // res.cookie 함수를 사용하여 token을 클라이언트 쿠키로 전달
}

---
router.post('/', passport.authenticate('local'),
	(req, res, next) => {
		setUserToken(res, req.user);  // 쿠키를 브라우저에 저장함

	res.redirect('/');
});

// passport-jwt 사용하기
// 요청된 JWT토큰의 서명을 확인하고 인증하는 기능을 구현
const JwtStrategy = require('passport-jwt').Strategy;

const cookieExtractor = (req) => {
	const { token } = req.cookies;

	return token;
};

const opts = {
	secretOrKey: secret,  // import
	jwtFromRequest: cookieExtractor,
}

module.exports = new JwtStrategy(opts, (user, done) => {
	done(null, user)
})

---
passport.use(jwt);
```

6. `JWT` 토큰은 기본적으로 모든 요청에 포함한다. 요청에 토큰이 있는 경우 로그인된 상태로 처리하기 위해 모든 요청에 공통적으로 적용할 수 있는 미들웨어로 `JWT` 로그인을 추가
7. 로그아웃은 간단하게 클라이언트 쿼리를 삭제하여 처리 가능, `token` 값을 `null` 로 전달하고 `cookie` 의 만료시간을 0으로 설정하여 클라이언트가 쿠키를 바로 만료시키도록 전달

```js
// jwt middleware
app.use((req, res, next) => {
    if (!req.cookies.token) {
        next();
        return;
    }

    return passport.authenticate("jwt")(req, res, next); // req.user에 저장
});

// jwt logout
res.cookie("token", null, {
    maxAge: 0, // 쿠키 만료 시키기
});
```

### ❏ 회원 비밀번호 찾기 구현

1. 임의의 문자열로 비밀번호 초기화
2. 초기화된 문자열을 메일로 전달 → 메일 발송기능 개발 필요
3. 초기화 후 첫 로그인 시 비밀번호 변경 요청

### ❏ 메일 발송기능 구현 방법

1. `SMTP` 서버 이용: 네이버 구글 등의 메일서버를 이용하여 무료로 발송 가능, 메일 발송 및 관리 기능 직접 개발 필요
2. 메일 발송 서비스 이용(Mailgun, Sendgrid): 메일 발송 api 제공 및 관리용 웹페이지 제공, 사용량에 따라 유료 과금

### 💡 SMTP란?

1. `Simple Mail Transfer Protocol`: 메일 전송을 위한 표준 규약, `SMTP` 서버란 표준 규약을 통해 메일 전송하는 기능을 구현한 서버
2. `Node.js` 에서 메일 발송하기: `Nodemailer` 패키지를 사용하여 `SMTP` 서버(gmail, naver...)를 통해 메일 발송하기, 직접 만드는 것은 비효율적이다.
3. `Nodemailer` 에서 `gmail` 을 사용하기 위해서는 앱 비밀번호 설정 필요, 한번 설정하면 재 확인 불가

```js
const nodemailer = require("nodemailer");

const transport = nodemailer.createTransport({
    service: "Gmail",
    auth: {
        user: "google account",
        pass: "app password",
    },
});

const message = {
    from: "login account",
    to: "mail address",
    subject: "title",
    text: "message",
};

transport.sendMail(message, (err, info) => {
    if (err) {
        console.error("err", err);
        return;
    }
    cosnole.log("ok", info);
});
```

### ❏ 비밀번호 초기화 기능

```js
// 임의의 문자열을 만들어주는 함수
function generateRandomPassword(){
	return Math.floor(
		Math.random() * (10 ** 8)
		).toString().padStart('0', 8);
}
---

// email을 받아서 generateRandomPassword로 사용자의 비밀번호 초기화 후 메일로 발송
router.post('/reset-password', asyncHandler(... => {
	const { email } = req.body;
	const randomPassword = generateRandomPassword();
	await User.findOneAndUpdate({ email }, {
		password: getHash(password),
	});

	await sendEmail(email, '...', password);
	res.redirect('/');
}));
```

### ❏ 비밀번호 초기화 후 로그인 시 비밀번호 변경 요청

```js
// 비밀번호 변경
const UserSchema = ...
	passwordReset:{
		type: Boolean,
		default: false,
	}
...

---

router.poast('/reset-password', ...
	await User.findOneAndUpdate({
	...
	passwordReset: true
})

// 비밀번호 변경 요청
function checkPasswordReset(req, res, next){
	if(req.user && req.user.passwordReset){
		res.redirect('/update-password');
		return;
	}

	next();
}

router.poast('/update-password', ...
	await User.findOneAndUpdate({
	...
	passwordReset: false
})
```

### ❏ OAuth의 이해

1. `open authorization`: 서비스 제공자가 다른 서비스에게 데이터를 제공하기 위해 서비스 사용자에게 제공하는 사용자 인증방식의 표준
2. 서비스 제공자에게 인증 요청 → 인증 완료 후 사용자 정보를 요청한 서비스로 전달 → 인증 정보를 이용해 서비스 제공자의 데이터 사용
3. 구글 `OAuth` 인증 요청 → 인증된 `OAuth Token` 을 기록 → `OAuth Token` 을 사용하여 구글 캘린더 `API` 사용
4. 웹 서비스 제공자는 ID, PW 로그인을 구현할 필요가 없음
5. 웹 서비스 사용자는 ID, PW 를 입력할 필요가 없음

### ❏ 구글 로그인 구현하기

1. 구글 클라우드 플랫폼 프로젝트 생성
2. API 및 서비스 → OAuth 동의화면 설정
3. 사용자 인증정보 → OAuth 클라이언트 ID 만들기
4. passport-google-oauth20 연동
5. `passport-google-oauth20` : passport-strategy 인터페이스의 구글 로그인 집합체(OAuth 인증을 구현하기 위해서는 인증 요청, 데이터 수신 등의 복잡한 작업 필요), `passport-google-oauth2.0` 은 손쉽게 구글 `OAuth 2.0` 을 구현해주는 패키지

### ❏ Nginx

1. 최근 신규 프로젝트에서 가장 많이 채택되고 있는 웹 서버 소프트웨어(웹 서버 소프트웨어: `HTTP` 요청을 받아 파일이나 프로그램 실행 결과를 `HTTP` 응답으로 보내주는 소프트웨어)
2. `Java - Tomcat`, `PHP - fastcgi` 등 다른 언어가 `HTTP` 요청을 처리를 위한 의존성이 있는 것에 반해, `Node.js` 는 기본적으로 `HTTP` 요청을 수신하고, 응답하는 기능이 이미 있다. 따라서 웹 서버 소프트웨어 없이도 스스로 동작할 수 있다. 하지만, `node.js` 단독으로 사용하게 되면 `HTTPS`, `도메인 연결`, `static file caching` 등의 기능을 `production-level` 서비스를 구축할 수는 없다. 따라서 `node.js` 앞 단에 웹 서버 소프트웨어를 붙여서 사용한다. `HTTP` 요청과 응답은 node.js에서 자체적으로 사용이 가능하다.
3. `Nginx` 의 `reverse-proxy` 기능을 사용해, `Node.js` 와 `Nginix` 를 연결할 수 있다. `reverse-proxy` 는 `HTTP` 요청을 다른 서버에 전달하는 기능인데, `Nginx` 가 요청을 받아, 설정된 내용에 해당하는 요청만 `node.js` 에 전달한다.

![](https://images.velog.io/images/abcd8637/post/9d61eb15-28cf-47e0-9c8e-5b6cdb9ea673/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-11%2016.38.13.png)

```js
// 외부에서 온 모든 요청을 localhost:3000으로 전달하는 설정 파일
// HTTPS, file caching들의 작업은 Nginx의 설정방법을 참고하기
server {
	listen 80;
	server_name www.example.com;

	location / {
		proxy_pass http://localhost:3000;
		proxy_http_version 1.1;
	}
}
```

---

## 📍 36일차 12.14.화. 실시간 강의

오늘부터 25일 크리스마스까지는 1차 팀 프로젝트 기간이다. 팀원은 총 6명이고 역할은 `FE` 4명, `BE` 2명이다. 이때까지 혼자서 프로젝트를 진행했다면 이번엔 팀으로 진행하는거라 팀에 누가되지 않도록 열심히 해야겠다는 생각이 가득찼다. 약간의 걸림돌(?) 있다면 지금까지는 `React`, `React + Typescript`로 진행했다면 이번엔 `바닐라 자바스크립트 + node.js`로 진행하는 것이다. `react`를 사용하면서 `DOM` 관리를 편하게 사용했었는데,, 이번엔 `DOM`을 하나씩 관리하는 일이 얼마나 까다로운지 몸소(?)느껴보는 시간을 가져보자.. 내가 맡은 파트는 `image drag & drop + form`, `login` 화면이다. 이번에 맡은 파트를 어떻게 코드로 구현했는지 프로젝트가 끝나갈 무렵에 올려야겠다.

## ❏ 애자일 방법론

1. 프로젝트를 처음부터 다시 만든다면 비효율적일 것이다. 따라서 처음부터 설계를 꼼꼼하게 진행한다. 데모버전을 빠르게 만들어서 지속적으로 피드백을 시도한다.
2. 폭포수 방법론: 요구 사항 분석 → 기획 → 개발 → 테스트 → 통합 → 유지보수
3. 애자일 방법론: 고객이 수용하고 납득할만한 최소한의 설계와 개발을 반복하는 고객 중심의 개발 방법론이다. 익스트림 프로그래밍(XP, TDD: Test Driven Development), 스크럼(Scrum, Sprint) 등의 여러 방법이 있다. (고객의 니즈를 즉시 반영) 이번 프로젝트는 스크럼방식 사용
4. `TDD`: 테스트 코드를 통해 프로덕트가 원활하게 돌아가는지 확인하는 방법
5. 애자일 방법론은 순서가 없다. 2주내에 결과물을 내기위해 어떻게 해야할지 생각한다.
6. 한 가지 방법만 따라야 하지도 않고 전체적인 큰 틀인 스크럼과 스프린트 수행을 유지한 상태에서 우리 팀의 상황에 맞게 조금씩 변형하며 적용해야 한다.

### ❏ 스크럼

1. 작은 목표를 짧은 주기로 체크하며 프로젝트를 지속적으로 개발하는 관리 기법
2. 매일 짧게 진행되는 미팅을 수행하며 어제 한일, 오늘 할일, 장애 현상 등을 공유한다.

### Git flow

1. 이번 프로젝트에서는 `branch` 를 간소화해서 생성
2. `Master branch` : 배포 가능한 상태의 코드, 서비스로 출시될 수 있는 브랜치
3. `Sprint branch` : 기능 개발을 위한 브랜치 병합을 위해 사용, 모든 기능이 추가되고 버그가 수정되어 배포 가능한 상태라면 `master` 로 `MR`
4. `Feature branch` : 새로운 기능 개발 및 수정하는 브랜치로 사용, 작업이 끝난 기능은 `sprint` 로 `MR`
5. `feature branch` → `sprint branch` → `master branch`
6. 매주 코드리뷰를 위해 `master branch` 로 `MR` 을 올린다.
7. `MR`(merge request)

### ❏ 스프린트

1. 짧은 기간 내에 빠르게 결과를 만들어내는 기법, 스프린트 종료 후 구성원들은 스프린트 리뷰와 회고를 진행
2. 프로덕트 계획 → 아이디어 스케치 → 프로토 타입 개발 → 테스트
3. 비전에서 최종목표를 세우고 로드맵을 통해 구체적인 단계를 세운다.
4. 깃랩 이슈는 3-4시간만에 할 수 있는 단위로 쪼개라.
5. 스크럼 마스터: 코치
6. 사소한 기능 하나라도 `product owner` 처럼 만들자.

### ❏ Issue

1. 프로젝트 진행 시, 어떠한 상황, 문제 또는 계획을 개발 할 예정이라는 것을 알려주는 이정표(문제가 생겨서 `issue` 가 아니라 해야 할 일? `todo` 정도)
2. `milestone`: 프로젝트에서 주요한 이벤트를 표시하는 기준점,

### ❏ Wiki

1. 문서화 시켜줄 수 있는 기능, 프로젝트의 정보를 넣어두면 된다.(스크럼 내용 등)

---

## 📍 37일차 12.15.수. 프로젝트 2일차 TLDR

1. `Cannot delete branch 'image-upload'`: branch checkout으로 다른 branch로 옮기고 삭제하기
2. `onload()`메소드보다는 `addEventListener('load')` 사용하기
3. `github`는 `pull-request`, `gitlab`은 `merge-request`
4. merge 완료했으면 기존 branch 삭제하고 새로운 branch 생성하기
5. `git branch -D 브랜치명`: 브랜치 삭제
6. input태그에서 `debounce` 적용하기
7. input태그에서 `datalist`는 추천하는 선택지를 나타냄
8. `CSS 방법론`: BEM

---

## 📍 38일차 12.16.목. 프로젝트 3일차 TLDR

1. `JPG`와 `JPEG`는 같은 압축파일형식이다. 원래는 `jpeg`로 사용되었으나, DOS 사용시절 확장자의 길이는 3자로 제한됨으로 인해 jpg로 줄여 사용했다.
2. `exif`는 디지털 카메라에서 이용되는 이미지 파일 포맷이다. jpg, tiff6.0, RIFF, WAV 파일 확장자에만 사용가능하다.(JPEG 2000, PNG, GIF에서는 지원하지 않는다.)
3. `JPEG2000`은 `JPEG`보다 높은 압축률과 이미지 품질을 얻기 위해 개발되었다. 대부분의 웹 브라우저에서 지원되지 않는다.(현재 `safari`에서만 사용가능)
4. `js` import시 오류가 뜨면 다음과 같이 설정하자

```
"settings": {
    "import/ignore": [".js$", "node_modules/*"]
},
```

5. `eslint` 설정 `npm ci `
6. `form` 데이터 전송은 `/post/tmp`로 넘겨주고 서버에서 처리 후 `/post/:id`로 `redirect`시킨다.
7. 서버는 `router/index.js/updatePath(path)`
8. 위치 입력받는 `input`은 1개로 만들어 놓고 `debounce`, `EXIF`라이브러리로 위치 적용하기

---

## 📍 39일차 12.17.금. 프로젝트 4일차 TLDR

1. `addEventListener`의 `event` 타입 전달 시 `on` 접두사를 제외하고 사용한다.(예. onchange -> change, onclick -> click, oninput -> input)
2. `event` 중 `change` 이벤트는 요소가 포커스를 잃을 때까지 이벤트가 실행되지 않고 다른 곳을 클릭하면 이벤트가 트리거 되는 반면, `input` 이벤트는 요소가 변경될 때마다 이벤트가 트리거 된다.
3. 자동완성기능에 `addEventListener`를 적용할 때 `change`와 `datalist+option`을 사용하면 `debounce`를 적용하지 않아도 된다. (change 이벤트는 요소의 포커스가 잃을 때 적용되기 때문에 글씨가 입력하는 중간에 이벤트가 발생하지 않는다.) 하지만, `UI`수정이 자유롭지 못하다. 반면, `input` 이벤트에 자동완성기능을 직접 구현한다면, `debounce`로 최적화를 시켜주자(input 이벤트는 입력할 때마다 이벤트가 일어나기 때문) `UI`수정은 `datalist+option`방법보다 비교적 자유롭다.
4. `debounce`: 일정 시간안에 연속적인 이벤트가 발생하면 일정시간 이후에 한번만 실행된다. 예를 들어 `input` 값을 `api` 통신할 때
5. `trigger`: 일정 시간안에 연속적인 이벤트가 발생하면 일정시간 내 딱 한번만 이벤트가 실행되는 기법
6. 배열의 값을 변경해서 적용할 때는 `map`을, 배열을 순회하면서 변수를 뽑아내려고 하면 `forEach`를 사용하자

---

## 📍 40일차 12.18.토. 프로젝트 5일차 TLDR

1. 비동기 함수가 중첩되어있을 때 `return` 하려면 `return new Promise`에 `resolve`를 넣어주어 꺼내주자.
2. 함수에 단순히 `return`을 넣고 `console.log` 찍으면 `undefined`가 나온다.
3. JS에서 라이브러리 사용시 npm install 이후 import from으로 불러오기

```javascript
// getGPSData
function getGPSData(img) {
    return new Promise((resolve, reject) => {
        img.addEventListener("load", function () {
            EXIF.getData(this, async function () {
                const GPSLatitude = EXIF.getTag(this, "GPSLatitude");
                const GPSLatitudeRef = EXIF.getTag(this, "GPSLatitudeRef");
                const GPSLongitude = EXIF.getTag(this, "GPSLongitude");
                const GPSLongitudeRef = EXIF.getTag(this, "GPSLongitudeRef");

                if (GPSLatitude === undefined || GPSLongitude === undefined)
                    reject("GPS 정보가 없습니다.");

                const latitudeDecimal = changeToDecimal(
                    GPSLatitude,
                    GPSLatitudeRef
                );
                const longitudeDecimal = changeToDecimal(
                    GPSLongitude,
                    GPSLongitudeRef
                );

                const response = await fetchAddressAPI(
                    longitudeDecimal,
                    latitudeDecimal
                );

                const [wide_addr, local_addr] = response;
                resolve(`${wide_addr} ${local_addr}`);
            });
        });
    });
}
```

---
## 📍 41일차 12.21.화. 프로젝트 6일차 TLDR

1. 컴포넌트의 리턴값이 1개 이상일 때는 객체로 리턴하자.

```javascript
const getGPSTag = () => ({
    GPSLatitude: "GPSLatitude",
    GPSLatitudeRef: "GPSLatitudeRef",
    GPSLongitude: "GPSLongitude",
    GPSLongitudeRef: "GPSLongitudeRef",
});

const { GPSLatitude, GPSLatitudeRef, GPSLongitude, GPSLongitudeRef } =
    getGPSTag();
```

2. 라이브러리를 페이지에서 호출하면 함수 `parameter`로 넘기지 않아도 된다. (전역적으로 호출 가능)
3. JavaScript로 HTML코드를 다루는 방법 3가지를 배움: `innerHTML`은 보안에 취약한 요소가 있다. DOM조작이 불편하다. 만들기는 쉽다. 가독성도 나쁘지 않다. `node manipulate`는 유지보수가 불편하다. 그러나 DOM을 정확하게 조작할 수 있다. `hyperscript`는 가독성과 컴포넌트의 재사용성이 증가한다. 엘리먼트에 접근할 상황이 생길 때는 한계가 있다. 
4. `innerHTML`의 장점과 단점

```
* 장점
  - HTML 마크업 문자열로 간단히 DOM조작이 가능하다.
  - 구현이 간단하고 직관적이다.
* 단점
  - HTML 코드에 JS 악성코드가 심어져 있다면 파싱과정에서 그대로 실행되기 때문에 위험하다. (XSS)
  - 기존노드가 존재하고 자식노드를 추가할 때 원래 있던 기존노드까지 새로 만들어 렌더링 한다. 즉, 바뀌지 않아도 되는 노드까지 모두 제거하고 처음부터 새롭게 자식 노드를 생성하여 DOM에 반영하는데 이는 효율적이지 않다.
  - 새로운 요소를 삽일 할 때 삽입될 위치를 지정할 수 없다.(insertAdjacentHTML 메서드 활용하기, insertAdjacentHTML도 innerHTML과 마찬가지로 HTML 마크업 문자열을 파싱하므로 XSS에 취약하다.)
```

5. `develop branch`는 `d/upload-page`, `feature branch`는 `f/upload-page`와 같이 설정할 수 있다.
6. `hyperscript`(HTML 마크업의 Javascript 기반 표현이며, 순수 DOM을 생성한다.)

```
  * 장점
    - 순수 DOM을 생성한다.
    - 코드의 가독성과 재사용성이 크게 향상된다.
  * 단점
    - element에 자유롭게 접근이 쉽지 않다.
```

7. n만큼 자식 node를 추가할 때 직접 DOM에 n번만큼 추가하지 말고(n번만큼 reflow가 발생한다.), `createDocumentFragment`를 사용해서 DOM접근을 한번만 하자.
8. hyperscript에서 HTML코드에서 class를 추가할 때 class를 쓰지 않고 className을 사용하는 이유: class가 예약어이기 때문
9. git reset: `git add .`로 track하는 파일 제거하기
10. css 속성 중 width: clamp(0, 100%, 860px)는 다음을 나타낸다.

```
  - min-width: 0px;
  - width: 100%;
  - max-width: 860px;
```

11. 중앙정렬은 flex를 사용하기보다는 margin: 0 auto를 사용하자(내용이 1column 일 때)
12. 저장할 때 원하는 언어 prettire, elint 적용 제외시키기

```
"[markdown]": {
    "editor.formatOnSave": false
}
```

---
## 📍 42일차 12.22.수. 프로젝트 7일차 TLDR
1. `git commit`에서 다음에 구현해야 할 사항이 있다면 다음과 같이 작성하기 `TODO: fetch가 정상적으로 수행되지 않았을 때 예외 처리하는 함수 만들기`
2. 함수 인자로 객체로 둘러싸여 있을 경우

```javascript
function createInstance({baseUrl}){}

// 인자에 URL 바로 넣기
createInstance({baseUrl: "www.naver.com"});

// URL 변수로 따로 저장하기
const URL = "www.naver.com";
createInstance({baseUrl: URL});
```

3. `try - catch` 문에서 `error`의 메세지만 출력할 때는 `error.message`를 사용하자
4. MIME type: 클라이언트에게 전송된 문서의 다양성을 알려주기 위한 매커니즘, 각 문서와 함께 올바른 `MIME` 타입을 전송하도록, 서버가 정확히 설정하는 것이 중요하다.

```
  * text/plain
  * text/html
  * image/jpeg
  * image/png
  * audio/mpeg
  * audio/ogg
  * audio/(별표)
  * video/mp4
  * application/octet-stream
```

5. 모르는 개념은 공식문서를 참고하자. 관련 예제를 참조하면 좋다.
6. 클라이언트 사이드 `WEB API`(브라우저 API)가 포함된 자바스크립트 코드를 실행하면 `node.js` 환경이 아닌 브라우저에서 실행해야 한다.
7. `input accept` 유형은 선택한 파일 유형을 검증하지는 않으며, 단순히 브라우저가 사용자를 올바른 파일 유형을 사용하도록 힌트를 제공할 뿐이다. 사용자가 옵션을 바꾸면 다른 형태의 파일도 게시할 수 있으므로 서버사이드에서 유효성 검증을 통해 `accept` 특성을 보조해야 한다.
8. 시각적으로 `input`을 숨긴 후 레이블에 버튼처럼 스타일을 적용해서 파일을 업로드하고 싶은 경우 레이블을 누르라고 알려주는 편이 낫다. 이때, `visibility: none`, `display: none`으로 숨길경우 접근성 보조 기술이 파일 입력 칸을 상호작용 할 수 없기 때문에 `opacity`를 대신 사용한다.
9. 파일 업로드 취약점: 파일을 업로드 할 때 1차적으로 `input accept`를 이용해 사용자에게 원하는 `MIME` 타입으로만 입력할 수 있게 유도할 수 있지만 악성 코드를 업로드 할 수 있기 때문에 서버사이드에서 유효성검사를 동시에 진행해야 한다. 브라우저에서 `proxy` 툴을 이용해 파일타입 변조를 통해 확장자 검사를 피할 수 있다. (정확하게는 파일 업로드 시 `Content-type`(응답 내에 있는 헤더) 속성을 프록시로 이용해 우회한다.) 기초적인 방어는 다음과 같다.

```
* 확장자 검사
* 대소문자 구분하지 않고 확장자 비교
* 특수문자 금지
* 업로드 된 파일명, 확장자 난수화
* 업로드된 파일을 url 요청으로 직접 접근이 불가능한 위치에 저장
```

10. `innerHTML`의 `script` 공격예시

```js
// script
document.body.innerHTML = `<script>alert(\"hi\")</script>`

// onerror
document.body.innerHTML = `<img src='' onerror="alert(\'hi\')">"
```

11. `blob` 파일을 데이터를 메모리에 저장하는 방식인데, 이를 사용하려면 메모리 누수와 메모리 해제도 같이 진행해야 한다.
12. `latency test`: 지연성 검사, scroll이 frame 단위로 어떻게 흘러가는지?, user가 갑자기 늘어났을 때 어떻게 대응할 것인가?, image의 개수를 무제한으로 넣고 실험, image의 용량 무작위, 어떤 컴포넌트가 로딩이 제일 오래 되는지?
13. 프로젝트 설계에 대한 고민을 충분히 하자. 2~3일씩 걸려도 된다. 나중에 발표할 때 설계에 대한 고민을 다른 팀과의 차별성으로 사용하면 경쟁력있는 프로젝트가 된다.

> reference
1. MDN: https://developer.mozilla.org/ko/docs/Web/HTML/Element/Input/file
2. 티스토리: https://owin2828.github.io/devlog/2020/01/09/etc-2.html

---
## 📍 43일차 12.23.목. 프로젝트 8일차 TLDR
1. `eslint`가 적용되지 않을 때 `VScode`의 버전을 살펴보자. `VScode`의 버전이 낮으면 `eslint`를 아무리 설정해도 적용되지 않는다. 현재 버전 `1.63.2`, 이전 버전 `1.52.2`
2. `component`와 `util` 폴더의 차이는 쉽게 생각해서 `HTML` 코드를 리턴하는지 하지 않는지의 여부를 보면 된다. `HTML`코드를 리턴하면 컴포넌트, 리턴하지 않으면 해당 기능을 모든 폴더에서 사용할 수 있는 `util`폴더에 저장하자.
3. 사이트 배포형태: `SSG`(정적페이지를 빌드한 후 산출물을 CDN에 배포하고 필요할 때마다 CDN으로부터 전달받은 정적 페이지를 유저에게 빠르게 제공한다. JAM stack(Javascript, API, Markup stack), `netlify`, `vercel` 등에 배포만 하고 `API Fetch`만 주로 실시), `SSR`(서버측 코드가 연계되는지의 여부, 주로 `EC2`를 기반으로 한다.)
4. 렌더링 테스트는 `google - light house`, `snapshot` 테스트
5. `hyperscript`로 상태관리 하는 방법? `react-fiber` 참고(난이도가 상당히 높다.)
6. 뷰(VIEW): `proxy api`, `immer`
7. `redux` + `observer` + 아키텍쳐 패턴
8. 학습의 주도권을 나에게 갖고 있자. 책에서 나오는 목차를 그대로 옮겨 작성하는 것보다 `input`과 `output`을 고려해서 공부하는 것이 훨씬 기억에 잘 남는다. 
9. `redux`: 바닐라 자바스크립트에 리덕스를 붙여보자.(`npm install react-redux`는 `react`와 `redux`를 binding해주는 라이브러리고 `npm install redux`를 사용하자.)
10. 회사에 취업한다는 것이 곧 성장을 뜻하는 것은 아니다. 독학을 할 수 있다면 마음먹고 독학해서 취업해도 좋다. 그게 아니면 스터디를 가입하는 것

---
## 📍 44일차 12.24.금. 프로젝트 9일차 TL;DR
오늘은 크리스마스 이브다. 어제와 동일하게 열심히 프로젝트를 진행중인데, `python`이 만들어진 배경이 갑자기 생각났다. (궁금한 분들은 <a href='https://namu.wiki/w/Python#s-2'>나무위키</a> 참조) 나중에 심심해서 토이프로젝트를 만들다가 걸작을 만들 날이 올까? 거두절미하고 오늘의 `TL;RD`을 살펴보자.

1. `keyup`: 키가 놓을 때 이벤트가 발생한다.
2. `keydown`: 키가 눌렸을 때 이벤트가 발생한다.
3. `formData`자체로는 `console.log`를 사용하지 못하게 브라우저 정책으로 막혀있고, 대신 `for-of formData.entries()`, `for-of formData.keys()`, `for-of formData.values()`로 하나씩 볼 수 있다.
4. `formData.addEventListener('formdata')`, `btn.addEventListener('submit')`
5. `await`으로 결과 확인할 때 `then, catch` 대신 `if`문으로 확인하자.
6. `form enctype`: `method`가 `post`인 경우 데이터의 `MIME`유형을 나타내는 속성이다.

```
* application/x-www-form-urlencoded: 기본값(default)
* multipart/form-data: <input type="file">이 존재하는 경우 사용
* text/plain: HTML 5에서 디버깅 용으로 추가된 값
```

7. `formmethod`: `button type="submit"`일 때, `HTTP` 메서드를 지정한다. `formmethod`를 지정한 경우 버튼의 소유자가 가진 `method` 특성보다 우선한다. (post: 양식의 데이터를 HTTP body에 넣는다. get: action URL 뒤에 ?를 추가한 후 양식 데이터를 덧붙인다.)
8. `dependency cycle detected`: 서로 `export`된 파일을 `import` 할 때 발생하는 오류

```javascript
// dep-b.js
import './dep-a.js';
export function b() {/* ... */}

// dep-a.js
import { b } from "./dep-b.js" // reported: Dependency cycle deteced.
```

9. `header` 내부의 `formdata`를 서버로 보낼 때 `JSON.stringify`하지말고 `form` 형태로 보내자
10. `input`을 가릴 때는 `opacity:0`도 있지만 `hidden` 태그를 사용하자. (`label`의 `for`과 `input`의 `id`를 맞추면 된다.)
11. `name`: `form` 양식 데이터가 제출될 때 컨트롤의 값과 함께 제출 된다.
12. `form` 데이터 넘길 때 `img`태그 말고 `file` 형태로 읽은 값을 넘겨야 서버에서 인식한다.
13. `box-shadow`: 그림자 효과

```css
/* 수평방향(x), 수직방향(y), 흐림의 반경(숫자가 클 수록 그림자의 끝이 흐려지고 0이 될수록 선명하다), 그림자가 확산되는 거리, 그림자의 색상 */
.box_shadow {
	width: 300px;
	height: 300px;
	box-shadow: 3px 3px 8px black;  
}
```

reference
1. MDN: https://developer.mozilla.org/ko/docs/Web/HTML/Element/form
2. eslint-plugin-import git: https://github.com/import-js/eslint-plugin-import/blob/main/docs/rules/no-cycle.md

---
## 📍 45일차 12.25.토. 프로젝트 10일차 TL;DR
1. `input`태그의 file값을 동적으로 조작하고 싶으면 `dataTransfer` 객체에 임시로 옮겨 담자

```javascript
const tempTransfer = new DataTransfer();
tempTransfer.items.add(validFileData);
const targetInput = document.querySelector(`#empty-input__${id}`);
targetInput.files = tempTransfer.files;
```

2. `JWT` 토큰 사용시 `OAuth` 로그인 후 배포 사이트로 `redirect` 하지 않고 `local`에서 테스트해보려면 `userProfile`, `userId`, `token` 값을 `local browser`에 `localStorage`에 `setItem`으로 넣어두자.

---
## 📍 46일차 12.28.화. 실시간 강의 React
저번주까지는 프로젝트를 진행했고 오늘부터 다시 수업에 들어간다. 챕터를 넘어가 이제는 바닐라 자바스크립트 대신 `React`를 배운다. 일일이 `document.createElement` 코드를 작성하며 `DOM` 관리를 했는데 이제는 신경을 덜 써도 되는 `React`를 배운다니 뭔가 홀가분(?)하면서도 `document`코드가 그리워지는 느낌이 든다. 어제 프로젝트를 진행하면서 앞으로 배우고 싶은 내용은 `ESlint`, `prettier`, `webpack`과 `babel`을 정확하게 공부해야겠다는 생각이 들었다. 4주 뒤에 있을 두번째 팀 프로젝트 때 나의 목표는 `CRA`을 사용하지 않고 직접 `ESlint`, `prettier`, `webpack`, `babel` 설정을 나의 코드로 작성하는 것이다.

1. 프로젝트를 너무 거대하게만 생각하지말고 작은 부분에서 수동으로 해야할 일들을 자동으로 돌리면 그것 또한 포트폴리오가 된다. 일상에서 코딩으로 좋아지는 모습을 잘 기록하면 좋은 결과가 있을 것이다. ex) 페이스북 거절 버튼 누르기, 위도와 경도 자동계산??
2. `npm install --global create-react-app` : 리액트 개발환경 설치
3. `npx create-react-app react-app` : `CRA` 설치, 파일명 앞에 `.` 를 붙이면 현재 디렉토리에 그대로 생성한다
4. `CRA`는 코드 변경 후 저장하면 코드의 바뀐 부분을 알아서 적용해주는데, 이는 `webpack`의 `HotModuleReplacement`가 해준다. 웹팩 설정할 때 `devServer`를 설정하면 `CRA`를 사용하지 않고도 이를 구현할 수 있다.
5. 리액트의 본질은 사용자 정의 태그를 만드는 것이라 해도 과언이 아니다.
6. `npm run start`: src/index.js 엔트리 파일, `public/index.html`: html 템플릿 파일, `npm run build`: 배포 버전 생성, `build`: 배포 버전의 내용 파일, `import filename.css`를 이용해서 css 를 사용할 수 있다.
7. `index.css` : 리액트를 실행하면 실행되는 `css` 파일
8. 사용자 정의 태그를 만들 때 하나의 태그 안에 들어가야한다.
9. 태그의 제일 앞글자가 대문자면 사용자 정의 태그이고 소문자면 네이티브 태그다. 
10. `<></>` 와  `<React.Fragment>` 의 차이점:  `<></>` 는 바벨 7버전 이상에서 사용할 수 있다.  `<></>` 는 key를 부여할 수 없다. `<React.Fragment key="key"></React.Fragment>` 와 같이 `key`를 부여한다. `ESlint` 에서 관련된 설정을 할 수 있으며, 자세한 설정은 <a href='https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-fragments.md'>다음</a>을 참고하자

```javascript
// incorrect code
<React.Fragment><Foo /></React.Fragment>

// correct code
1. <><Foo /></>
2. <React.Fragment key="key"><Foo /></React.Fragment> 
```

11. `HtmlWebpackPlugin`: HTML 파일 생성을 단순화한다. 매번 컴파일에 변경되는 해시로 된 파일 이름을 가진 webpack 번들에 특히 유용하다. 플러그인이 HTML 파일을 생성하게 하거나 나만의 로더를 사용할 수 있다. script 태그에 사용하여 body 에 있는 모든 webpack 번들을 포함하는 HTML5 파일을 생성한다. 만약, entry 포인트가 여러개인 경우 생성된 HTML 에 모두 `<script>`태그로 포함 된다. 만약, webpack 출력에 CSS asset 이 있다면 이들은 생성된 HTML 파일의 `<head>` 요소 안에 `<link>` 태그로 포함된다.
12. `HotModuleReplacement`: 전체 재로드 없이 어플리케이션이 실행되는 동안 모듈을 교환, 추가 또는 제거한다. 소스 코드에서 CSS / JS 가 수정되면 브라우저를 즉시 업데이트 한다. 이는 브라우저의 개발 도구에서 직접 스타일을 변경하는 것과 거의 비슷하다.
13. `Vanilla JS`에 대한 지식이 있어야 한다. 왜냐하면 차세대 프레임워크도 기본은 `JS`기 때문이다.
14. `CRA` 를 사용하는 이유: Babel (JS Compiler, JS의 최신문법을 ES5 전 문법으로 변경해준다. 그리고 JSX 문법을 JS 문법으로 바꿔준다. JSX 는 문법은 자바스크립트 공식 문법은 아니다.  IE 는 최신문법을 모르기 때문에 예전 문법으로 알려줘야 한다.), webpack 은 여러 파일을 번들링해준다. 다른 파일들을 한 파일로 모아서 제공해준다. npm start 를 치면 Babel, webpack 이 동작한다.
15. `vite`, `snowpack` 은 프로젝트의 규모가 클 때 사용하고, `CRA` 는 가벼울 때 사용한다. 
16. `React.strictMode`로 감싸져있으면 `Develop`단계에서 렌더가 2번 되는게 정상이다. 프로덕션은 아님
17. `serviceWorker.unregister();` :  앱 배포 시 캐시가 남지 않도록 하는 코드
18. `ReactDOM.render(element, document.getElementById('root'));`: id 가 root 인 태그를 찾은 후, 정의한 엘리먼트를 ReactDOM 에 렌더링 하는 과정
19. `element`: 실제 화면에 표시 할 수 있는 정보가 들어있는 JS 객체 JSX 형태로 구성되어있다. `component`: document 내부 요소를 설정한다.(props, state 등등..)

---
## 📍 47일차 12.29.수. 온라인 강의
오늘은 `SPA`, `React`, `Component`, `ES6`, `module`,  `JSX` 등에 대해서 배웠다. 바닐라 자바스크립트와 `CRA`를 통해 프로젝트를 생성할 때 다른점이 있는데 `CRA`는 웹팩과 바벨을 자동으로 설정해준다는 것이다. 강의에서 배우는 내용과 별개로 웹팩과 바벨을 설정하는 방법을 공부하고 있는데 세팅이 끝나면 따로 포스팅으로 올려야겠다.

1. 첫 접속시 `HTML`을 내려받는것은 전통적인 페이지와 동일하나, `data` 변경시 전체를 새로고침하지 않고 변경된 `data`만 업데이트하는 것은 `SPA` 특징 중 하나이다.

![](https://images.velog.io/images/abcd8637/post/f8f37713-7557-4751-99d9-258d82c900d8/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-29%2010.04.06.png)

2. `React`를 사용하면 `SPA`를 편하게 사용할 수 있다.
3. `React`: 사용자 인터페이스를 만들기 위한 `Javascript` 라이브러리
4. `component`: react 에서 서비스를 개발하는데 있어 독립적인 단위로 쪼개어 구현 바닐라 자바스크립트를 사용할 때 페이지마다 HTML, CSS, JS 넣는방식과는 달리 한 페이지 내 각 요소를 쪼개 하나의 구성요소를 만들고 컴포넌트를 조립하여 한 페이지를 만든다.
5. `Virtual DOM`: 가상적인 표현을 메모리에 저장하고 `ReactDOM` 과 같은 라이브러리에 의해 실제 `DOM` 과 동기화하는 프로그래밍 개념
6. `JSX`: `JavaScript` 내에서 `UI` 를 작성하기 위해 개발자에게 익숙한 환경을 제공, `HTML` 과 유사
### ❏ 왜 React인가?
1. 생산성 / 재사용성: `Component` 와 `Hook` 을 활용하여 작은 단위의, 독립적인 요소로 개발하여 개발자의 생산성과 코드의 재사용성을 높인다.
2. 풍부한 자료 / 라이브러리: 방대한 자료 및 편리한 오픈소스 라이브러리
3. 다양한 사용처: 웹 애플리케이션뿐만아닌 React-native 에 적용하여 app 으로도 개발 할 수 있기 때문

### ❏ React 특징 분석하기
1. `JSX`
2. `component`: 하나의 블록을 만들어서 필요한 곳에 조립하여 개발한다.
3. `state`: 데이터를 유동적으로 관리한다. `state` 변경시 컴포넌트가 다시 렌더링 된다.(나중에 배우겠지만 `react`가 리렌더링 되는 시기는 `props`가 바뀌었을 때, `state`가 바뀌었을 때 부모 `component`가 렌더링 될 때, `forceUpdate()`를 실행했을 때가 있다.)

### ❏ React 프로젝트 생성
1. `React` 개발 시 `CRA` 를 사용해야하는것은 아니다 직접 `script` 를 추가해서 사용해도 된다.

```
<script crossorigin src="https://unpkg.com/react@17/umd/react.production.min.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@17/umd/react-dom.production.min.js"></script>
```

2. `CRA` 는 `React` 프로젝트를 손쉽게 생성할 수 있도록 도와주는 보일러플레이트(Boilerplate) , CRA 는 페이스북에서 직접 만들어서 관리한다. 상대적으로 덜 중요한 코드는 노출되지 않고, 강력한 Command 를 지원한다. 모든 브라우저가 해석될 수 있도록 `transcompile` 을 지원한다.(Babel, 코드 번들링(코드를 알아보기 어렵게 함), Webpack)

3. `npx` : `npm` 패키지를 1회성으로 내려 받아 실행할 때 사용하는 명령어 

```js
node_modules: npm을 이용해 설치한 패키지들 모음
public: 정적인 파일들을 모아 놓는 곳
src: 리액트 개발을 위한 파일들을 모아 놓는 곳
gitignore: git에 올리지 않는 파일
package.json: 프로젝트에 관한 정보와 사용하는 패키지들을 명세하는 파일 npm install ~로 설치하면 기록에 남는다. npm install을 치면 정의된 모듈을 한꺼번에 설치할 수 있다.
README.md: 내 프로젝트에 관한 설명을 작성하는 파일
```

4. 패키지 불러오기

```js
import "패키지명"  // CSS import하는 것만으로 역할을 하는 경우 패키지명만 import 한다. (확장자까지 명시해야한다.)

import something from "패키지명"  // 기본적으로 패키지를 불러올 때

import { a, b } from "패키지명"  // 일부 메소드나 변수만 가져올 때는 구조분해를 하여 가져온다.

import * as something from "패키지명"  // 패키지에 default로 export되는 객체가 존재하지 않을 경우 * as 이름으로 불러올 수 있다.

import defaultExport from "module-name";
import * as name from "module-name";
import { export1 } from "module-name";
import { export1 as alias1 } from "module-name";
import { export1 , export2 } from "module-name";
import { foo , bar } from "module-name/path/to/specific/un-exported/file";
import { export1 , export2 as alias2 , [...] } from "module-name";
import defaultExport, { export1 [ , [...] ] } from "module-name";
import defaultExport, * as name from "module-name";
import "module-name";
```

### ❏ JSX와 컴포넌트
1. `JSX` 는 함수 호출과 객체 생성을 위한 문법적 편의를 제공하는 `JS` 확장
2. `HTML` 과 비슷하게 생겼으나 `JS` 이고 `HTML` 과 다른 부분이 있음
3. `JSX` 는 `Babel` 에 의해서 `Transcompile` 이 된다.
4. 장점: 개발자 편의성 향상, 협업에 용이 / 생산성 향상, 문법 오류와 코드량 감소
5. `HTML` 과 차이점

```js
1. `HTML` 태그 내에 `JS` 연산, `HTML` 태그 안에 중괄호를 넣으면 `JS`코드를 사용할 수 있다.
2. `class` 대신 `className`
3. 스타일은 큰 따옴표 대신 `object`로만 입력한다. 인라인 스타일은 중괄호 2개 사용 `style={{ padding: 10, color: 'red' }}`(첫번째 중괄호는 자바스크립트를 사용하겠다는 뜻, 두번째 중괄호는 객체 형태로 넣는다. inlineStyle의 propertyName은 camelCase로 사용, 첫단어 소문자 다음은 대문자)
4. 닫는 태그 필수 `img`, `input`, `<br>` 등...
5. 최상단 `element`는 반드시 하나(실제 렌더링 시에는 `Fragment` 안에 있는 내용만 출력된다.) <>는 최근에 생긴 문법임
```

6. 컴포넌트: React 에서 페이지를 구성하는 최소 단위, 이름은 대문자로 시작, Class Component / Function Component로 나뉨, Controlled Component / Uncontrolled Component (form 태그에서 사용자의 입력을 받아 데이터를 state 를 이용해 직접 관리하는지의 여부)

```js
// MyComponent
const MyComponent = ({ children }) => {
	return <div style = {{ }}> { children } </div>
}

// App
const App = () => {
	return (
		<div>
			<p>안녕</p>
			<MyComponent>반가워</MyComponent>
			<div>반가워</div>
		</div>
	)
}
```

7. `class Component`, `Function Component`: 초기 `React` 는 모두 클래스 컴포넌트였으나, 이후 v16부터 새로운 Function Component와 Hooks개념이 발표되었으며 현재는 주로 Function Component를 사용한다. 클래스형은 `state` 선언이 가능하지만, 함수형은 `Hooks` 를 통해 `state` 선언이 가능하다.

```js
// class component
class Hello extends Component {
	render(){
		const { name } = this.props
		return <div>{ name }님 안녕하세요</div> 
	}
}

// function component
const Hello = (props) => {
		const { name } = this.props
		return <div>{ name }님 안녕하세요</div> 	
}
```

8. `class Component` 특징: `Java` 개발자에게 친숙한 형태이다. `React` 의 생명주기를 파악하기 쉽다. (렌더링, 값이 바뀌는 시기 등 명확한 구별 가능)
9. `props(properties)`: 컴포넌트 `Attribute` 에 해당하는 부분, 컴포넌트 안에 작성된 하위 `Element` 를 `children` 이라고 한다. 결국엔 `children` 도 `props` 중 하나이다.

```javascript
const MyComponent = (props) => {
	const { user, color, children } = props

	return (
		<div style={{color}}> 
			<p>{user.name}님의 하위 element는!</p>
			{children}
		</div>
	) 
}
```

10. 컴포넌트끼리 데이터를 주고받을 땐 props, 컴포넌트 내에서 데이터를 관리할 땐 state, 데이터는 부모에서 자식으로만 전달한다.

---
## 📍 48일차 12.30.목. 온라인 강의
오늘은 `react`의 `useState`, `props`, `Hooks`, `function component`, `class component`등에 대해서 배웠다. 

1. 나의 문제, 주변에 쉽게 해결 할 수 있는 작은 기능들을 만들어보자 나중에 도움이 된다.(영우 봇 - 지하철 실시간 도착, 영화 순위)
2. `useState` 를 `consol.log` 하면 첫번째 값은 내가 설정한 값이고 두번째 값은 `state` 의 값을 바꾸는 함수다.

![](https://images.velog.io/images/abcd8637/post/76f94348-99e3-47e8-bc93-0bdd2afaf9ff/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-30%2011.21.35.png)

3. `state` 가 바뀌면 해당 컴포넌트는 재 랜더링된다., `props` 의 값이 바뀌어도 새로 렌더링된다. 이때 자식들의 `component` 까지 재 렌더링된다.
4. `HEAD`: 워킹 디렉토리가 누구와 같은지 알려준다.
5. `data-attribute` : data를 임시로 저장하고 싶을 때

```javascript
// data attribute HTML syntax
<article
  id="electriccars"
  data-columns="3"
  data-index-number="12314"
  data-parent="cars">
...
</article>

// JS access
const article = document.querySelector('#electric-cars');
// The following would also work:
// const article = document.getElementById("electric-cars")

article.dataset.columns // "3"
article.dataset.indexNumber // "12314"
article.dataset.parent // "cars"

// CSS access
article::before {
  content: attr(data-parent);
}

article[data-columns='3'] {
  width: 400px;
}
article[data-columns='4'] {
  width: 600px;
}

// react
// event.target 객체 내에서 dataset객체를 가져올 수 있다.
function clickHandler(event) {
	event.preventDefault();
	const id = evt.target.dataset.id;
	props.onChangeMode("READ", id);
}
```

[데이터 속성 사용하기 - Web 개발 학습하기 | MDN](https://developer.mozilla.org/ko/docs/Learn/HTML/Howto/Use_data_attributes)

7. `teachable Machine` : 조명 세기를 기준으로 홈페이지 주간 / 다크 모드, 사진을 보고 누가 접속했는지 확인하고 UI 변경해주기?? 등등

### ❏ 실습
1. `component`: `props` 를 `input` 으로 하고 `UI` 가 어떻게 보여야 하는지 정의하는 `React Element` 를 `output` 으로 하는 함수
2. `class` vs `Functional` : `v16.8` 이전까지는 `class` 를 사용했다. `class` 컴포넌트의 문제점: 복잡하다.(ex. 생명주기 함수), 재사용이 안된다.(동작과정이 비슷한 컴포넌트는 재활용하는것이 효율적임), `this` (4개의 this가 잇음.) Hook이 등장하면서 함수 컴포넌트도 클래스 컴포넌트만 가능했던 작업이 가능해졌습니다. 기존의 클래스 컴포넌트가 가지고 있던 복잡성과 재사용성이 해결되었습니다.

```javascript
// functional
function Component1(props){
	return <div></div>
}

// class
class component1 extends React.component{
	render(){
		return ()
	}
}
```

3. `props`: 상위 컴포넌트에서 하위 컴포넌트로 데이터를 넘길 때
4. `state`: 컴포넌트 자체가 갖는 속성 → 보통은 자식에게 넘겨주지 않고 본인만 상태를 갖도록 작성한다.
5. `Hook:` : 함수형 컴포넌트에서 생명주기 기능을 연동할 수 있게 해줍니다.
6. `State Hook`: `const [<상태 값 저장 변수>, <상태 값 갱신 함수>] = userState(<상태 초깃값>);`
7. 클래스 컴포넌트에서는 `state` 변경 시에는 `state` 객체를 통째로 넣어줘야 한다.

```javascript
import React, { useState } from "react";
import "./App.css";
import { LIST } from "./components/mock/LIST";

// Q1. map을 사용해서 컴포넌트 만들기
// key는 unique한 값으로 넣어두기

// Q2. 데이터를 입력받는 <input> 만들기: state에 저장
// const [input, setInput] = useState("");

// Q3. 데이터를 추가하려면? data state에 새로운 값을 넣는다.
// 1. 버튼을 하나 만들자
// 2. 버튼을 눌렀을 때 title은 사용자가 입력한 값으로 date는 날짜로

// Q4. 플래그
// 1. 버튼을 하나 만들자
// 2. 버튼을 눌렀을 때, 위쪽 데이터가 전부 안 보임
// 3. 버튼을 다시 누르면 데이터가 다시 보임

function App() {
    const [flag, setFlag] = useState(false);

    function toggleFlag(flag) {
        setFlag(!flag);
    }

    const [data, setData] = useState(LIST);

    function onSubmit(event, title, date) {
        event.preventDefault();
        const newData = {
            id: data.length + 1,
            title: title,
            date: date,
        };
        setData([...data, newData]); // 기존의 data를 바꾸려면 원래 있던 Data를 복사해야함.
    }

    return (
        <div className="App">
            {flag === false &&
                data.map((item) => (
                    <Info key={item.id} title={item.title} date={item.date} />
                ))}
            <Form onSubmit={onSubmit} />
            <hr />
            <button onClick={() => toggleFlag(flag)}>
                화면 보이기 / 숨기기
            </button>
        </div>
    );
}

function Form(props) {
    const [title, setTitle] = useState("");
    const [date, setDate] = useState("");

    function handleTitle(event) {
        event.preventDefault();
        setTitle(event.target.value);
    }

    function handleDate(event) {
        event.preventDefault();
        setDate(event.target.value);
    }

    return (
        <form onSubmit={(event) => props.onSubmit(event, title, date)}>
            <input
                type="text"
                value={title}
                name={title}
                onChange={handleTitle}
                placeholder="이름을 입력하세요"
            />
            <input type="date" onChange={handleDate} value={date} name={date} />
            <button type="submit">제출</button>
        </form>
    );
}

// 원래는 `form`태그 양식으로 써도 되지만 button으로
/* <button onClick={(e) => {
    const today = new Date();
    const year = today.getFullYear();
    const month = today.getMonth();
    const day = today.getDay();
}}></button> */

function Info(props) {
    return (
        <div>
            <h3>{props.title}</h3>
            <p>{props.date}</p>
            <hr />
        </div>
    );
}

export default App;
```

---
## 📍 49일차 12.31.금. 온라인 강의
오늘은 `class component`와 `function component`에서 `props`와 `state`, `event`를 다루는 법을 배웠다. `function component`는 많이 사용해서 익숙했는데, `class` 문법은 많이 사용하지 않아서 손에 잘 잡히지 않았다. 다루는 법을 배워둬야 나중에 많이 써먹겠지?!
### ❏ props

1. `component` 에 원하는 값을 넘겨주고 재사용 할 때 사용하며, 넘겨줄 수 있는 값은 변수, 함수, 객체, 배열 등 `JS` 의 요소라면 제한이 없다.
2. 반환되는 `JSX` 요소가 많으면 `props` 를 활용하는것이 중요하다.

```javascript
const Welcome = (props) => {
	return <h1>Hello, {props.name}</h1>
}

const App = () => {
	return <Welcome name="영우" />
}
```

3. `props` 의 값을 임의로 변경해서 사용하는 것을 지양하자. `props`를 가공하려면 복제한다음 사용하자.

```javascript
// Don't
const Welcome = (props) => {
	props.name = props.name + "님";
	return <h1>Hello, {props.name}</h1>
}

// Do
const Welcome = (props) => {
	const username = props.name + "님";
	return <h1>Hello, {username}</h1>
}
```

4. 기본적인 `DOM Element(div, span 등)` 들의 `Attribute` 는 `camel case` 로 작성한다. 
5. `data-`, `aria-` 의 `Attribute` 예외다. (ex, data-type, aria-label 등)
6. `HTML` 의 `Attribute` 와 `JSX` 의 `Attribute` 는 다른 이름이 있다. `class -> className`, `for -> htmlFor`
7. `HTML` 의 `Attribute` 와 `JSX` 의 `Attribute` 는 다른 동작 방식을 가지는것이 있다. (`checked → defaultChecked`, `value -> defaultValue`,  `style은 object 형식`), `html` 에서는 기본값을 설정하는 역할을 했으나 jsx에서는 현재값을 의미한다. 자유롭게 변경하고 싶다면 `default` 값을 설정하자.

```javascript
// checked 값이 false면 checkbox를 클릭해도 변화가 일어나지 않는다.
// 초기값의 의미로 checked, value를 사용하고 싶다면 defaultChecked, defaultValue Attribute를 사용하자.
<input type="checkbox" checked={false} />
```

8. `React` 에서만 쓰이는 새로운 `Attribute` 가 있다.(`key`, `dangerouslySetInnerHTML` 등)

```javascript
1. key는 React가 어떤 항목을 변경, 추가 또는 삭제할지 식별하는 것을 돕는다.
2. key는 엘리먼트에 안정적인 고유성을 부여하기 위해 배열 내부의 element에 지정해야한다.
3. key는 배열 안에서 형제 사이에 고유해야 하고 전체 범위에서 고유할 필요는 없다.
4. 두 개의 다른 배열을 만들 때 동일한 key를 사용할 수 있다.
5. Key를 선택하는 가장 좋은 방법은 리스트의 다른 항목들 사이에서 해당 항목을 고유하게 식별할 수 있는 문자열을 사용하는 것입니다. 대부분의 경우 데이터의 ID를 key로 사용합니다.
6. 렌더링 한 항목에 대한 안정적인 ID가 없다면 최후의 수단으로 항목의 인덱스를 key로 사용할 수 있습니다.
```

### ❏ State
1. `state` 는 `component` 내에서 유동적으로 변할 수 있는 값을 저장한다.
2. `state` 값이 변경되고 재렌더링이 필요한 경우에 `react` 가 자동으로 계산하여 변경된 부분을 렌더링한다.
3. `state` 값을 직접 변경하지말자. 직접 변경하게 되면 `react` 가 값이 변경됐는지 알아차리지 못한다. 반드시 `setState` 함수를 이용해 값을 변경하자.
4. `state` 를 변경하는 두 가지 방법

```javascript
const [count, setcount] = useState(0);

// setState내에 변경할 값을 넣기
setCount(count + 1);

// setState에 함수를 넣기, 함수를 넣는 경우 함수가 반환하는 값으로 state가 변경된다.
// 현재 값을 기반으로 state를 변경하고자 하는 경우 함수를 넣는 방법을 권장한다.
setCount((current) => { return current + 1 });

// object state를 만들 때 주의사항
// user.grade 값이 변경되었지만 user 객체는 변경되지 않았으므로 재렌더링 하지 않는다.
const [user, setUser] = useState({name: "민수", grade: 1});
setUser((current) => {
	current.grade = 2;
	return current;
})

// 재렌더링이 되려면 객체 자체를 바꿔야 한다. 
// object를 복사해서 새로만들고 원하는 값으로 변경한다.
setUser((current) => {
	const newUser = { ...current }
	newUser.grade = 2;
	return newUser;
})
```

### ❏ event
1. 웹 브라우저가 알려주는 `HTML` 요소에 대한 사건의 발생을 의미한다. `Element` 로딩, `Element` 클릭, 마우스를 올렸을 때, 더블 클릭했을 때 등 다양한 이벤트가 존재한다.
2. 이벤트 처리 방법: 핸들링 함수선언, 익명 함수로 처리
3. 이벤트 객체: `DOM Element`의 경우 핸들링 함수에 이벤트 `object` 를 매개변수로 전달한다.

```javascript
const App = () => {
	const handleChange = (event) => {
		console.log(event.target.value
	}

	return (
		<input onChange={handleChange} />
	)
}
```

4. 여러개의 input을 한 개의 `handler` 로 관리하기

```javascript
import React, { useState } from 'react';

function App() {
  const [person, setPerson] = useState({
    name: "김민수",
    school: "엘리스대학교"
  })
  
  const handleChange = (event) => {
    const { name, value } = event.target;
    setPerson((current) => {
        const newPerson = { ...person };
        newPerson[name] = value;
        return newPerson;
    })
  }
  
  return (
    <div className="App">
        <input name = "name" value={person.name} onChange={handleChange}/>
        <input name = "school" value={person.school} onChange={handleChange}/>
        <button onClick={()=>alert(`${person.name}님은 ${person.school}에 재학중입니다.`)}>버튼클릭!</button>
    </div>
  );
}

export default App;
```

### ❏ 컴포넌트 내 이벤트 처리
1. 컴포넌트에 이벤트 넘기기

```javascript
// app.js
import React, { useState } from 'react';
import { MyForm } from "./components/MyForm";

function App() {
    const [username, setUsername] = useState("");
    
  return (
    <div className="App">
        <h1>{username}님 환영합니다.</h1>
				<MyForm onChange={(event) => {
            setUsername(event.target.value)
        } }/>
    </div>
  );
}

export default App;

// MyForm.js
import React from "react";

export const MyForm = ({ onChange }) => <input onChange={onChange}/>;
```

2. 커스텀 이벤트

```javascript
const SOS = ({onSOS}) => {
	const [count, setCount] = useState(0);
	const handleClick = () => {
		if(count >=2){
			onSOS();
		}
	setCount(count+1);
	}

	return <button onClick={handleClick}> 세 번 누르면 긴급호출({count})</button>
}

const App = () => {
	return (
		<div>
			<SOS
				onSOS={() => {alert("긴급사태!"}} />
		</div>
	)
}
```

3. 이벤트 명명법: 자유롭게 설정할 수 있으나, 보통 `on + 명사`, `on + 명사 + 동사` 형태로 작성한다. (`onClick`, `onButtonClick`, `onInputChange`) 혹은 `handle + 동사`, `handle + 명사 + 동사` 형태로 작성한다. 
4. 컴포넌트를 활용하여 기능을 모듈화 하면 다음과 같은 이점이 있다.

```javascript
1. 코드 유지보수성이 향상됩니다.
2. 코드 재사용이 용이합니다.
3. 가독성 향상됩니다.
```

5. `setState`: 시간이 변하는 것처럼 주기적으로 변하는 것이 아니라 버튼 클릭과 같은 특정 이벤트로 상태가 변하는 것을 `State` 가 비동기적으로 변경된다고 한다.
6. 생명주기: 앱이 실행되고 종료되는 과정을 특정 시점별로 나눠둔 것, 컴포넌트가 이벤트를 다룰 수 있는 특정 시점

```javascript
// react
1. constructor(): State 데이터를 초기화 하는 메소드
2. render(): 클래스 컴포넌트에서 반드시 구현되어야 하는 메소드
3. componentDidMount(): 컴포넌트가 마운트 된 직후 호출되는 메소드
4. componentDidUpdate(): 업데이트가 진행된 직후에 호출되는 메소드
5. componentWillUnmount(): 컴포넌트가 마운트 해제되어 제거되기 직전에 호출되는 메소드

// componentDidMount
class Header extends React.Component {
  constructor(props) {
    super(props);
    this.state = {favoritecolor: "red"};
  }
  componentDidMount() {
    setTimeout(() => {
      this.setState({favoritecolor: "yellow"})
    }, 1000)
  }
  render() {
    return (
      <h1>My Favorite Color is {this.state.favoritecolor}</h1>
    );
  }
}

ReactDOM.render(<Header />, document.getElementById('root'));
```

7. 재사용 캡슐화(현재 시간 출력 컴포넌트)

```javascript
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
import App from './App';
import * as serviceWorker from './serviceWorker';

//현재시간을 출력하는 컴포넌트
//현재시간의 props를 받아 출력합니다.
function Clock(props) {
  return (
    <div>
      <h1>Hello, world!</h1>
      <h2>현재 시간: {props.time.toLocaleTimeString()}</h2>
    </div>
  );
}

//매초 마다 호출되는 함수
function tick() {
  //Clock 컴포넌트를 호출합니다.
  const element = <Clock time={new Date()}/>;
  
  //ReactDOM에 element을 렌더링합니다.
  ReactDOM.render(element, document.getElementById('root'));
}

setInterval(tick, 1000);

serviceWorker.unregister();
```

8. 클래스 컴포넌트로 현재 시간 출력 하기

```javascript
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
import App from './App';
import * as serviceWorker from './serviceWorker';

//클래스 컴포넌트를 사용하여 Clock컴포넌트를 작성합니다.
class Clock extends React.Component {
    render(){
        return(
             <div className="App">
                <h1>Hello, world!</h1>
                <h2>It is {this.props.time.toLocaleTimeString()}</h2>
            </div>
        )
    }
}

//매초 마다 호출되는 함수
function tick() {
  const element = <Clock time={new Date()}/>;
  ReactDOM.render(
    element,
    document.getElementById('root')
  );
}

setInterval(tick, 1000);

serviceWorker.unregister();
```

9. 클래스 컴포넌트로 `state` 관리하기 (클래스 내부에서 `state` 를 사용하려면 `constructor` 메소드를 생성해야한다.)

```javascript
1. 클래스 컴포넌트 내에 `constructor()` 메소드 선언
2. `constructor()` 메소드 내에 `super(props)` 호출
3. `this.props`를 `this.state`로 변경 `props`를 제공하는 대신 `state`에 필요한 데이터 저장
```

10. 이벤트 핸들러에 인수 전달하기: 보통 반복문 안에서 id 값을 추가 인수로 전달 할 때 bind를 사용하는 경우, event 를 따로 전달하지 않아도 된다.

```javascript
<button onClick={(e) => this.deleteRow(id, e)}>Delete Row</button>
<button onClick={this.deleteRow.bind(this, id)}>Delete Row</button>
```

---
## 📍 50일차 22.1.1.토. 온라인 강의
22년 임인년이 밝았다. 새해를 맞으며 온라인 강의를 들으니까 별 감흥이 없었다. 내게 중요한 목표는 작년부터 준비하고 있는 프론트엔드를 잘 살려서 상반기에는 꼭 취업을 했으면 하는 바램이 있다. 그럼 `FE` 교육을 들으면서 배웠던 내용을 복습해보자..

### ❏ State Hook
1. `useState` 는 컴포넌트 내 동적인 데이터를 관리할 수 있는 `hook` 입니다.
2. 최초에 `useState` 가 호출될 때 초기값으로 설정되며 재 렌더링이 될 경우 무시됩니다.
3. `state` 는 읽기 전용이므로 직접 수정하지 마세요.
4. `state` 가 변경되기 위해서는 `setState` 를 이용합니다.
5. `state` 가 변경되면 자동으로 컴포넌트가 재 렌더링 됩니다.

```javascript
const App = () => {
	const [state, setState] = useState();

	// 1
	setState("Hello");

	// 2
	setState((current) => {
		return current+"world"
	})
```

### ❏ Effect Hook
1. 함수 컴포넌트에서 `side effect` 를 수행한다.
2. 컴포넌트가 최초로 렌더링될 때, 지정한 `state` 나 `props` 가 변경될 때마다 콜백 함수가 호출 됩니다.(`dependency array`)
```javascript
const App = () => {
	useEffect(EffectCallback, Deps?)
}
```

3. 다른 함수를 `return` 할 경우 `state` 가 변경되어 컴포넌트가 다시 렌더링되기 전과 컴포넌트가 없어질 때 호출할 함수를 지정한다.

```javascript
useEffect(() => {
	// state가 변경될 때, 컴포넌트를 렌더링할 때
	const intervalId = setInerval(() => {
		console.log("hi");
	}, 1000)

	// 컴포넌트를 재 렌더링 하기 전에, 컴포넌트가 없어질 때
	return () => {
		clearInterval(intervalId);
	}
}, [])

// 컴포넌트 생성 / 소멸 관리
import React, { useEffect } from "react";

export const Greeting = () => {
		// 컴포넌트 생성
    useEffect(() => {
        console.log("컴포넌트가 생성되었습니다.")
    
		// 컴포넌트 소멸
    return () => {
        console.log("컴포넌트가 소멸되었습니다.")
    }
  }, [])
    
    return <h1>안녕하세요.</h1>
}
```

### ❏ 이외의 Hooks
1. `useMemo`: `const memoizedValue = useMemo(() => computeExpensiveValue(a, b), [a, b])`, 지정한 `state` 나 `props` 가 변경될 경우 해당 값을 활용해 계산된 값을 메모이제이션하여 재렌더링 시 불필요한 연산을 줄인다. 메모리에 올려놓기 때문에 컴포넌트가 너무 무거우면 사용을 지양한다.

```javascript
const App = () => {
	const [firstName, setFirstName] = useState("영우");
	const [lastName, setLastName] = useState("안");

  // 이름과 성이 바뀔 때마다 풀네임을 메모이제이션
	const fullName = useMemo(() => {
		return `${firstName} ${lastName}`
	}, [firstName, lastName])
}
```

2. `useCallback`: 함수를 메모이제이션하기 위해 사용한다. 불필요하게 함수가 다시 생성되는 것을 방지한다. `useMemo` 와 원리는 동일하다. `useMemo` 에서 함수를 리턴해주는 것과 `useCallback` 에 함수 자체를 넣어주는 것은 같은 의미를 갖는다.

```javascript
const App = () => {
	const [firstName, setFirstName] = useState("영우");
	const [lastName, setLastName] = useState("안");

  // 이름과 성이 바뀔 때마다 풀네임을 메모이제이션
	const getFullName = useCallback(() => {
		return `${firstName} ${lastName}`
	}, [firstName, lastName])

	return <>{getFullName()}</>
}
```

3. useRef: .current 프로퍼티를 가지며 값을 자유롭게 변경할 수 있다. React 에서 DOM element 에 접근할 때 사용한다. useRef에 의해 ref 객체가 변경되어도 컴포넌트가 재렌더링되지 않는다. let 을 이용하면 컴포넌트를 렌더링 할 때 선언문을 통과하면서 초기화 시킨다. 그럴때 useRef 를 사용하면 편하다. 변수를 함수밖에다 선언해도되지만 잠재적인 버그를 일으킬 수 있다.

```javascript
const App = () => {
	const inputRef = useRef(null);
	const onButtonClick = () => {
		inputRef.current.focus()

		// inputRef.current.value: element의 value값 가져오기
		// inputRef.current.name: element의 name값 가져오기
	}

	return (
		<div>
			<input ref={inputRef} type="text" />
			<button onClick={onButtonClick}> input으로 포커스</button>
		</div>
	)
}
```

4. `customHook` : 자신만의 Hook 을 만들면 컴포넌트 로직을 함수로 뽑아내어 재사용할 수 있습니다. state 나 effect hook 을 사용할 때 별도로 분리하는 것, hook 의 이름은 use 로 시작한다. 한 Hook 내의 state 는 공유되지 않는다.

```javascript
// useToggle.js
import React, { useState } from "react";

// initialValue에 default 값 설정
export const useToggle = (initialValue = false) => {
    const [isOn, setIsOn] = useState(initialValue);
    const toggle = () => setIsOn((isOn) => !isOn);
    
    return {
        isOn,
        toggle
    }
}

// App.js
import React from 'react';
import { useToggle } from "./hooks/useToggle";

function App() {
  const { isOn, toggle } = useToggle(false);
  
  return (
    <div className="App">
        <button onClick={()=>toggle()}>{isOn ? "켜짐" : "꺼짐"}</button>
    </div>
  );
}

export default App;
```

### ❏ 종합 실습 / 유용한 팁들
1. `Form` 개발하기

```javascript
// InsertForm.js
import React, { useState } from "react";

export const InsertForm = ({ onInsert }) => {
    const [inputValue, setInputValue] = useState("")
    
    const handleSubmit = (event) => {
        event.preventDefault();

				// onInsert가 있을 때만 실행
        if(typeof onInsert === "function"){
            onInsert(inputValue);
        }
        setInputValue("");
    }
    
    return (
        <form onSubmit={(event) => handleSubmit(event)}>
            <input value={inputValue} onChange={(event) => setInputValue(event.target.value)}/>
            <button type="submit">등록</button>
        </form>
    )
}

// App.js
import React from 'react';
import { InsertForm } from "./components/InsertForm";

function App() {
  const onInsert = (value) => {
    console.log(value)
  }

  return (
    <div className="App">
        <InsertForm onInsert={onInsert}/>
    </div>
  );
}

export default App;
```

2. 리스트 표현하기: Form 으로부터 전달 받은 값들을 리스트에 저장하고, 리스트의 값을 순차적으로 화면에 출력해봅시다.

```javascript
// InsertForm.js
import React, { useState, useCallback } from "react";

const InsertForm = ({ onInsert }) => {
    const [inputValue, setInputValue] = useState("");
    const handleSubmit = useCallback((event) => {
        event.preventDefault(); // 기본적인 HTML 동작으로 인해 페이지가 새로고침 되는 것을 방지
        if(typeof onInsert === "function" && inputValue) { // onInsert가 정상적인 함수인 지 확인하여 에러 방지
            onInsert(inputValue);
        }
        setInputValue("");
    },[onInsert, inputValue])

    return (
        <form onSubmit={handleSubmit}>
            <input value={inputValue} onChange={(event) => {
                setInputValue(event.target.value);
            }} />
            <button type="submit">등록</button>
        </form>
    )

}

export default InsertForm;

// ListView.js
import React from "react";

export const ListView = ({ todoList }) => (
         <div>
            <ol>
                {
                    todoList.map((item) => 
                        <li key={item.key}>
                            <span>{item.value}</span>
                            <button type="button">완료</button>
                            <button type="button">삭제</button>
                        </li>
                )}
            </ol>
        </div>
 )

// App.js
import React, { useState } from 'react';
import InsertForm from "./components/InsertForm";
import { ListView } from "./components/ListView";

function App() {
  const [todoList, setTodoList] = useState([]);
  
  
  const onInsert = (value) => {
    const newTodo = {
        key: new Date().getTime(),
        value: value,
        isCompleted: false,
    }
    setTodoList([...todoList, newTodo])
    console.log(todoList)
  }
  
  return (
    <div className="App">
        <InsertForm onInsert={onInsert} />
        <ListView todoList={todoList}/>
    </div>
  );
}

export default App;
```

3. 리스트의 값을 변경 및 삭제하는 기능 구현하기

```javascript
// App.js
import React, { useState } from 'react';
import InsertForm from "./components/InsertForm";
import ListView from "./components/ListView";

function App() {
  const [todoList, setTodoList] = useState([]);
  
const handleInsert = (value) => {
    setTodoList((current) => {
      const newList = [...current];
      newList.push({
        key: new Date().getTime(),
        value,
        isCompleted: false,
      });
      return newList;
    })
  }
  
const handleComplete = (index) => {
    const newList = todoList.map((item, idx) => 
        idx === index ? {...item, isCompleted: true} : item
    )
    console.log(newList)
  }
  
  const handleRemove = (index) => {
    const newList = todoList.filter((item, idx) => idx !== index);
    setTodoList(newList);
  }
  
  return (
    <div className="App">
        <ListView todoList={todoList} onComplete={handleComplete} onRemove={handleRemove} />
        <InsertForm onInsert={handleInsert} />
    </div>
  );
}

export default App;

// ListView.js
import React from "react";

const ListView = ({todoList, onComplete, onRemove}) => {
  return (
    <div>
      <ol>
        {todoList.map((item, index) => {
          return (
            <li key={item.key}>
              <span>{item.value}</span>
              <button type="button" onClick={() => {
                if(typeof onComplete === "function") {
                  onComplete(index);
                }
              }}>완료</button>
              <button type="button" onClick={() => {
                if(typeof onRemove === "function") {
                  onRemove(index);
                }
              }}>삭제</button>
            </li>
          );
        })}
      </ol>
    </div>
  )

}

export default ListView;
```

1. 메모리 누수: `정리가 필요하지 않은 side effects`, 클래스형 컴포넌트의 생명주기 메소드를 작성하다 보면 동일한 코드가 들어가는 경우가 많습니다. Effect Hook을 이용하면 생명주기 메소드 내 중복되는 코드를 함수형 컴포넌트에서 간단하게 관리할 수 있습니다.

React가 DOM을 업데이트한 뒤 추가로 코드를 실행해야 하는 경우 side effects 정리가 필요 없습니다. 즉, 컴포넌트 실행 이후 신경 쓸 것이 없는 경우 별다른 정리를 하지 않아도 됩니다. 아래 예시는 버튼 클릭 시 1씩 카운트를 추가하는 컴포넌트입니다. 해당 컴포넌트는 렌더링 이후 계속 사용되기 때문에 따로 정리가 필요하지 않습니다.

```javascript
class Example extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }

  componentDidMount() {
    document.title = `You clicked ${this.state.count} times`;
  }
  componentDidUpdate() {
    document.title = `You clicked ${this.state.count} times`;
  }

  render() {
    return (
      <div>
        <p>You clicked {this.state.count} times</p>
        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
          Click me
        </button>
      </div>
    );
  }
}
```

2. `정리를 이용하는 side effects`: 한편 정리(clean-up)가 필요한 side effects도 있습니다. React가 DOM을 업데이트한 뒤 추가로 코드를 실행할 필요가 없으면 정리를 해줘야 합니다. 그렇지 않으면 경우에 따라 메모리 누수가 발생해 시스템에 치명적인 영향을 미칠 수 있기 때문입니다. 아래는 채팅 앱에서 친구의 상태를 보여주는 컴포넌트입니다.

```javascript
class FriendStatus extends React.Component {
  constructor(props) {
    super(props);
    this.state = { isOnline: null };
    this.handleStatusChange = this.handleStatusChange.bind(this);
  }

  componentDidMount() {
    ChatAPI.subscribeToFriendStatus(
      this.props.friend.id,
      this.handleStatusChange
    );
  }
  componentWillUnmount() {
    ChatAPI.unsubscribeFromFriendStatus(
      this.props.friend.id,
      this.handleStatusChange
    );
  }
  handleStatusChange(status) {
    this.setState({
      isOnline: status.isOnline
    });
  }

  render() {
    if (this.state.isOnline === null) {
      return 'Loading...';
    }
    return this.state.isOnline ? 'Online' : 'Offline';
  }
}
```

3. 정리가 필요 없는 컴포넌트: DOM을 업데이트 한 뒤 추가로 코드를 실행해야 하는 경우는 clean up을 하지 않아도 된다.

```javascript
// 클래스 컴포넌트
import ReactDOM from 'react-dom';
import './index.css';
import * as serviceWorker from './serviceWorker';


import React from 'react';

class Counter extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }
  
  // componentDidMount() 메소드를 완성하세요.
  componentDidMount(){
   alert(`${this.state.count}번 클릭했습니다.`)
  }
  
  // componentDidUpdate() 메소드를 완성하세요.
  componentDidUpdate(){
    alert(`${this.state.count}번 클릭했습니다.`)
  }
  
  render() {
    return (
      <div>
        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
          버튼 클릭
        </button>
      </div>
    );
  }
}

ReactDOM.render(<Counter />,document.getElementById('root'));

serviceWorker.unregister();

// 함수형 컴포넌트
import ReactDOM from 'react-dom';
import './index.css';
import * as serviceWorker from './serviceWorker';

// useEffect를 import 하세요.
import React, { useState, useEffect } from 'react';

function Counter() {
  const [count, setCount] = useState(0);
  
  // useEffect()와 화살표 함수를 이용해 버튼이 클릭된 횟수를 경고창으로 띄우세요.
  // componentDidMount(), componentDidUpdate()와 동일한 기능을 한다.
  useEffect(() => {
    alert(`${count}번 클릭했습니다.`)
  }, [count])

  return (
    <div>
      <button onClick={() => setCount(count + 1)}>
          버튼 클릭
        </button>
      </div>
  );
}

ReactDOM.render(<Counter />,document.getElementById('root'));

serviceWorker.unregister();
```

4. 정리가 필요한 컴포넌트

```javascript
// class형
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
import * as serviceWorker from './serviceWorker';

class Container extends React.Component {
  constructor(props) {
    super(props);
    this.state = {show: true};
  }
  delHeader = () => {
    this.setState({show: false});
  }
  render() {
    let myheader;
    if (this.state.show) {
      myheader = <Child />;
    };
    return (
      <div>
        {myheader}
        <button type="버튼" onClick={this.delHeader}> Delete Header </button>
      </div>
    );
  }
}

class Child extends React.Component {
  // componentWillUnmount() 메소드를 생성하고 경고창을 띄우세요.
  componentWillUnmount(){
    alert("텍스트가 제거 되었습니다!")
  }
  
  render() {
    return (
      <p>버튼을 클릭해 해당 텍스트를 제거하세요.</p>
    );
  }
}

ReactDOM.render(<Container />,document.getElementById('root'));

serviceWorker.unregister();

// 함수형 컴포넌트: useEffect 안에 작성함으로써 생명주기 메소드를 한 곳에서 관리할 수 있다.
import ReactDOM from 'react-dom';
import './index.css';
import * as serviceWorker from './serviceWorker';
import React, { useState, useEffect } from 'react';

function Container() {
  const [show, setShow] = useState(true);
  
  let myheader;
  if (show) {
    myheader = <Child />;
  }
  
  return (
    <div>
    {myheader}
    <button onClick={() => setShow(false)}>버튼</button>
    </div>
  );
}

function Child() {
  // useEffect() 내 경고 문구를 출력하는 cleanup() 메소드를 반환하세요.
  useEffect(() => {
    return () => {
        alert("텍스트가 제거 되었습니다!")
    }
  })
  
  return (
    <p>버튼을 클릭해 해당 텍스트를 제거하세요.</p>
  );
  
}

ReactDOM.render(<Container />,document.getElementById('root'));

serviceWorker.unregister();
```

5. Effect Hook 요약: 10초뒤에 clean up 함수 작동

```javascript
import ReactDOM from 'react-dom';
import './index.css';
import * as serviceWorker from './serviceWorker';


import React, { useState, useEffect } from 'react';

const Example = () => {
  const [username, setUsername] = useState("");

  // 언제 호출되는지 확인하기 위해 useEffect에서 콘솔 출력을 해보세요.
  useEffect(() => {
    console.log("componentMount, compnentDidUpdate", username);
    },
    [username]
  );

  useEffect(() => {
    return () => {
        console.log("unMount", username);
    };
  }, []);

  const handleUsername = e => {
    const { value } = e.target;

    setUsername(value);
  };

  return (
    <div>
      <div>
        <input value={username} onChange={handleUsername} />
      </div>
      <div>
        <span>{username}</span>
      </div>
    </div>
  );
};

function App() {
  const [shouldRender, setShouldRender] = useState(true);

  useEffect(() => {
    setTimeout(() => {
      setShouldRender(false);
    }, 10000);
  }, []);

  return shouldRender ? <Example /> : null;
}

ReactDOM.render(<App />, document.getElementById("root"));
serviceWorker.unregister();
```

5. `useReducer`: 컴포넌트의 상태 업데이트 로직을 컴포넌트에서 분리할 수 있습니다.
6. `useMemo` : 메모이제이션이란 함수의 인자로 넘겨진 함수로 기존 함수의 실행이 끝나고 난 뒤 실행되는 함수 또는 특정 시점이나 이벤트가 발생했을 때 시스템이 자동으로 실행시키는 함수를 말합니다.
7. `useCallback`: 함수를 `props` 로 넘겨줄 때 사용 (실습 코드 생략)

---
## 📍 51일차 1.4.화. 실시간 강의
오늘은 `React`의 `form`태그, `props`, `컴포넌트 계층으로 분리`, `역방향 state`처리에 대해서 배웠다. `50일`차 내용에 크게 벗어나지 않아서 난이도가 있지는 않았다. 

### ❏ 이론
1. 부모에서 자식으로 오는 변경된 값은 `props` 를 사용하고, 자식에서 부모로 가는 값의 변경은 부모에서 내려오는 함수로 값을 전달한다.
2. `form` 에서 `onSubmit` 으로 제출 된 값 가져올때는 `event.target.name.value` 사용하기

```javascript
<form onSubmit={submitHandler}>
  <input type="text" name="title" placeholder="title" />
  <textarea name="body" placeholder="body" />
  <input type="submit" value="제출" />
</form>;

function submitHandler(event) {
    event.preventDefault();
		const { title, body } = event.target;
    console.log(title.value, body.value);
}
```

3. `update` 시 `props` 로 받아온 내용은 수정이 정상적으로 되지 않기때문에 `props` 로 받아온 내용을 `state` 로 선언하고 `setState`로 바뀌는 값을 적용한다.
4. 서버를 변경하는 명령으로 `a href` 태그를 사용하지 않고 `form` 태그를 사용한다.

### ❏ 실습
1. `UI`를 컴포넌트 계층으로 분리하기: 한 가지의 기능만 수행하는 컴포넌트로 만들기.

![](https://images.velog.io/images/abcd8637/post/8725fccd-2753-4d26-b281-4b356ff69f65/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-04%2015.32.09.png)

2. 역방향으로 `state`를 처리하려면 `state`를 한 단계 위로 올리는 방법이나 상위 컴포넌트에서 `state`를 적용하는 함수를 만들기
3. 스타트업에 지원할 때는 지원회사가 시리즈 투자를 받은 이력이 있는지 확인해보고 `job description`이 내가 지원하는 분야와 맞는지 확인하기

---
## 📍 52일차 1.5.수. 온라인 강의
오늘은 `react`에서 스타일링과 관련한 내용을 배웠다. `CSS-import`, `CSS-module`, `CSS-in-JS`인데, 나는 `CSS-in-JS` 방식 중 하나인 `styled-componentns`를 줄곧 사용해왔었고, `CSS-module`은 처음 듣는 용어였는데, 각 방식의 장/단점과 차이점들을 배우고나니까 이해가 잘됐다.

### ❏ React styling
1. 스타일링을 통해 사용성을 높이면 유저경험이 높아진다.
2. 좋은 앱을 만들기 위해서는...

```
1. 번들 사이즈: CSS코드가 차지하는 사이즈는 무척 중요한 요소, 번들 사이즈가 클수록 서버로부터 파일을 받아 파싱하고 유저에게 보이는 시간이 길어질 것이다.
2. 앱 성능: animation, transition 등 유저와의 상호작용에서 스타일 코드의 성능이 중요한 요소다.
3. UI/UX: 스타일링에 대한 지식으로, 고급 테크닉을 적용하여 더 나은 UI/UX를 반영
4. JS 를 이용한 다양한 스타일 기법: UI 토글링, 애니메이션, 다크모드, 복잡한 UI 컴포넌트 등은 JS에 대한 지식만으로 구현하기 힘듦
5. 유지보수가 용이하고 확장 가능한 코드: 스타일에 관련된 코드를 작성하고 어떻게 관리하는가에 대한 지식이 필요하다.
```

3. 자바스크립트로 스타일을 바꾸는 코드를 여러 줄 작성할 때, 브라우저는 각 줄을 수행하며 해당 DOM Element뿐만 아니라 주변의 모든 Element에 대한 스타일 재계산을 수행하게 됩니다. 반면에 CSS class를 바꾸면 한 번에 스타일을 변경하게 됩니다.
4. CSS에는 관련 스타일을 하나로 축약하는 코드가 많습니다. 또한 cascading을 이용해 inherit할 수 있는 속성, default 속성 등도 있습니다. 이처럼 CSS 지식을 이용해 간결하고 효율적인 코드를 작성할 수 있습니다.
5. `CSS-import`: `CSS(SCSS, Sass)` 파일을 `import` 해서 사용. 필요한 모든 `CSS` 스타일을 하나의 파일에 작성하여, 자바스크립트 파일과 코드 분리 가능, 단순하게 `import` 문만 작성하면 되니까 간단하다.

```javascript
1. 단순히 CSS 파일만을 import하여 사용할 수 있어 편리.
2. 컴포넌트가 많지 않을 경우, 하나의 CSS 파일에 코드를 관리하는 것도 가능함
3. CSS 파일은 분리할 수 있으나, namespace를 나눌 수 없음. 만일 스타일이 겹칠 경우, cascading rule에 따라, 마지막에 나온 룰이 덮어씌워짐
4. button 스타일을 따로 따로 적용하고 싶은데 마지막에 import한 css의 button으로 통일된다.
5. className을 구체적으로 명시함으로써 해결 가능하지만, 불필요하게 클래스명이 길어지고 비슷한 버튼 컴포넌트가 여러개 생길수록 코드 관리가 어려워진다. 

import 'button.css'

function Button({ children }){
	return <button className="button"> { children } </button>
}
```

![](https://images.velog.io/images/abcd8637/post/6c485b65-93dc-44b9-90c4-2c815eeaa213/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-05%2009.42.26.png)

6. `CSS-module`: 하나의 `CSS module` 파일 안에 작성한 스타일은 하나의 파일 `nameSpace` 로 관리한다. `className` 뒤에 겹치지 않는 `hash`를 붙인다. 스타일이 겹치는 문제 해결, 두 단어 이상의 경우 `camelCase` 로 이름을 지음

```javascript
// InputWithButton.jsx
import styles from "./input-with-button.module.css";

export function InputWithButton(){
	return(
		<div className={styles.container}>
			<input className={styles.input}/>
			<button className={styles.button}/>
		</div>
	)
}
```

![](https://images.velog.io/images/abcd8637/post/cf575f51-5693-4446-b184-f47dfd099e08/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-05%2023.24.06.png)

7. `CSS-in-JS`: 별도의 CSS 파일을 만들지 않고 하나의 컴포넌트 파일 안에서 스타일을 작성, JS 문법을 그대로 활용하여 코드를 작성, React 컴포넌트를 사용하는 것처럼 사용, Sass 문법 활용 가능

```javascript
// InputWithButton.js

import styled from "styled-components";

const Container = styled.div`
	background: black;
	margin: 10px;
	padding: 3px;
`

const Input = styled.input`
	border: none;
	height: 20px;
`

function InputWithButton(){
	return(
		<Container />
		<Input />
		<Button />
	)
}
```

### ❏ CSS, Sass
1. `CSS Box Model`: `CSS layout` 의 기본이 되는 모델

```
1. content-box, padding-box, border-box, margin-box 순으로 하나의 element 를 감싸고 있음
2. `box`의 타입은 `inline`, `block` 두 가지
3. `display`: `inline`, `inline-block`, `block` 으로 서로 다른 `box type`을 적용함
4. `element`의 기본 flow는 normalFlow
div - block
	span - inline
div - block
p - block

5. box-sizing
  - 보통 박스의 크기를 정할 때 `width`, `height` 속성을 정하는데 이때는 `default`로 content-box를 정하게 된다.
  - 기본적으로 `width`, `height` 는 기본적으로 content-box로 정하게 된다.
  - width와 padding의 값까지 모두 합하면 width보다 커지거나 작아진다. 이때 이해하기 쉬운 레이아웃을 정의하기 위해 `box-sizing: border-box`를 사용한다.
  - `border-box`의 경우 `padding`, `border`의 크기까지 하나의 영역으로 잡는 `box-sizing`이 된다. (width나 height에 영향을 주지 않는다.), `border-box`까지 `width`를 설정한다.              
```

![](https://images.velog.io/images/abcd8637/post/77cdc8a4-2417-4e76-a1bb-56c822ee3b4b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-05%2023.26.26.png)

2. `css-position`

```
1. static: position의 default값으로, element는 normal flow를 따라 위치함
2. relative: normal flow를 따라 위치하되, 자기 자신에 상대적으로 위치함 (기본위치에서 얼마나 움직여서 지정할지?)
3. absolute: normal flow에서 벗어나 가장 가까운 ancestor에 상대적으로 위치함
4. fixed: normal flow에서 벗어나 viewport에 상대적으로 위치함 (바닥에 딱 붙이려면 left:0, bottom: 0)
5. sticky: normal flow에 따라 위치하되, 가장 가까운 scrolling ancestor에 상대적으로 위치함

* anscestor: 어떤 엘리먼트를 감싸는 개념(부모), containing block(static 속성을 제외한 다른 position을 가진 속성)

div - relative
	div - static
		p - absolute(div - relative에 상대적으로 위치한다. 만약, relative가 없다면 가장 최상위의 ancestor containing block으로 위치하게 된다.)

- modal을 만들 때 감싸는 element를 relative로 설정하고 relative의 상대적인 위치를 따라 모달을 설정한다.(top: 100px, left: 100px), 보통은 fixed를 사용함. 
```

3. `css-units`

```
1. px, pt, cm, in: 절대적인 길이를 표현(pt, cm, in은 printable에 많이 사용한다.)
2. rem, em, %: 특정 값에 상대적인 길이를 표현
3. vw, vh, vmin, vmax: viewport에 상대적인 길이를 표현

div - 5em
	div - 3em
		span - 2em(부모의 크기에 따라 변경된다.)
		span - 2rem(5em(root)의 크기에 따라 변경)

모바일 가로: 100vw, 세로: 100vh 일 때
- 내가 바라보는 창의 전체사이즈를 차지하게 된다.
```

4. `Sass`

```javascript
1. Syntactic Awesome Style Sheets. CSS Preprocessor
2. SCSS, Sass 문법을 지원함
3. 모듈, 믹스인, nested style, 변수, 조건문, 반복문 등의 기능으로 `CSS`를 프로그래밍 언어적으로 활용하도록 확장
4. `styled-components`는 Sass를 기본적으로 지원함

// & 문법
.reset-button{
	&.active {}  // .reset-button.active
	&.disabled {}
	&:hover {}
  &:not(:first-of-type){}
	&+&{}  // .reset-button + .reset-button
	&~&{}
	& > button {}
}

// variable
// 색상, 사이즈 등 자주 등장하는 값을 주로 변수로 사용함
$color-red: red;
$color-white: #fff;

.reset-button{
	color: $color-red;
	&:hover {
		color: $color-white
	}
}

// nested style
// 별도의 class를 정의할 필요 없이, 하나의 block안에 여러 css를 적용할 수 있는 방법
// CSS sepcificity가 그대로 적용되므로, 너무 깊은 nested는 유지보수가 힘들다. 보통 1depth
.reset-button{
	color: $color-red;
	&:hover {
		color: $color-white;
	} 
	> button {}
}

/* 일반적인 css 적용시
resset-button{ 
	color: red
}

reset-button: hover{
	color: black
}
*/

// mixins, import, include
// font-styles.scss
@mixins font-style-1 {
	font-size: 36pt;
	font-weight: 700;
	line-height: 1.5;
	letter-spacing: -0.05;
}

@mixins flex-center{
	display: flex;
	justify-content: center;
	align-items: center;
}

// usage.scss
@import './font-styles.scss';
@import './flex-center.scss';

.button{
	@include font-style-1;
	background: red;
}

.layout{
	@include flex-center
}
```

### ❏ `CSS flexbox model`
1. `CSS flexbox model`

```js
1. HTML element를 하나의 상자로 간주하고, 그 안에서 내부의 item을 어떻게 배열할 것인지 스타일 하는 모델
2. 1차원의 레이아웃을 디자인하는데 사용
3. responsive design에 유리
4. 가운데 정렬, 비율로 정렬 등을 처리할 때 유리
```

2. `flex-box` 기본 개념

![](https://images.velog.io/images/abcd8637/post/b75d653a-33ab-4551-8f9a-b195922fb2b6/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-05%2023.28.48.png)

```
1. flex container: flexbox 아이템을 담는 컨테이너
2. flex item: 컨테이너 안에 담긴 아이템
3. flex axis: flex 아이템의 방향을 결정하는 축
```

3. `flex-container`

```js
1. flex-direction: row, column
2. justify-content: main axis 정렬
3. align-items: cross axis 정렬
4. flex-wrap: flex container가 내부 item의 width를 합친것보다 작아질 때 어떻게 정렬할것인지를 결정
```

4. `flex-item`

```js
1. flex-grow: flex container가 커질 때 item이 얼마나 늘어날 것인가(flex-grow: 0, container가 늘어나도 item의 모양은 그대로)
2. flex-shrink: flex container가 줄어들 때 item이 얼마나 줄어들 것인가 (flex-shrink: 0, container가 줄어들어도 item의 모양은 그대로)
3. flex-basis: 기준점이 되는 item의 크기(width, height 속성을 대신해서 사용, flex-basis:120px, item의 기본 길이가 120px이 된다.)
4. justify-self: 한 아이템을 main-axis에 따라 정렬할 것인지를 결정(container보다 우선순위가 높다.)
5. align-self: 한 아이템을 cross-axis에 따라 정렬할 것인지를 결정(container보다 우선순위가 높다.)
6. order: flex container내에서 item의 순서를 결정
```

5. `flex` : `flex-grow`, `flex-shrink`, `flex-basis` 를 축약한 속성이다. (default: `0 1 auto`)

```js
flex: 1 => 1 1 auto;(container의 영역이 여유가 있다면 그만큼 늘어나고, container의 영역이 줄어들면 같이 줄어든다. 기본 길이는 auto)
```

![](https://images.velog.io/images/abcd8637/post/f0ae209e-a2e0-4664-8c2e-8ad9b2cfe0dd/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-05%2023.30.13.png)

![](https://images.velog.io/images/abcd8637/post/45f57441-ae36-4cc3-ad9e-dcf822cf0cab/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-05%2023.30.31.png)

6. 첫번째 태그를 제외한 나머지 태그에 style 적용하기

```js
.problem span:not(:first-of-type){
	margin-left: 12px;
}
```

### ❏ styled-components
1. 자바스크립트 파일 안에 스타일을 정의하고 `React` 컴포넌트처럼 활용
2. `JS` 코드와 긴밀히 연계하여 다양한 코드작성 가능(변수, 반복문, 조건문, 함수, 모듈 등 활용가능)
3. 별도의 `CSS` 파일을 만들지 않고 하나의 파일 안에 스타일을 관리하고 싶을 때 유리
4. 스타일코드와 컴포넌트 코드간의 결합을 나누고 싶을 때 유리
5. `tagged template literal` 문법 활용
6. `CSS` 코드에 `post-css`, `minification`, `Sass` 적용
7. `CSS` 코드를 겹치지 않게 처리
8. 클래스 이름 자체가 `hash`