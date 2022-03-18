## 📍 61일차 1.18.화. 실시간 강의
이번주가 마지막 정규 수업이고 다음주부터 교육과정이 종료되는 주까지는 2차 프로젝트 기간으로 진행된다. 벌써 교육을 들은지도 4개월이 되어간다니... 시간이 참 빠른것 같다. 엘리스 교육을 들으며 프론트부터 백엔드까지 네트워크 통신에 대해 대략적인 큰 틀과 프론트엔드에서 사용하는 언어, 프레임워크 등 다양한 내용들을 배웠다. 참으로 도움이 많이 되었다. 교육이 끝날 때까지 열심히 공부해서 현업에서 함께 일하고 싶은 개발자가 되고 싶다. 그럼 `SSR`, `CSR`, `style-components`, 배포에 대해서 배워보자. 덧붙여 오늘은 `json-server`, `github-action`, `CI-CD`, `webhook`, `nginx`에 대해서도 배웠다.
 
### ❏ 이론 강의
`development` 단계에서 `API`를 `RESTful`하게 통신할 수 있는 간단한 라이브러리가 있는데 바로 `json-server`다. 사용법도 어렵지 않은데, `npx json-server --watch <실행 할 파일 명>` 을 터미널에 치면 곧바로 사용할 수 있다. 나는 `db.json` 파일을 생성하고 다음과 같이 작성했다. 이렇게 개발단계에서 임시적으로 `API`를 만들어 통신하는 서버를 `mock server`라 부르는데, 프로젝트 진행중에 백엔드에서 `API`가 만들어지지 않았을 때 사용하면 괜찮을 것 같다. `db.json`에서 여러개의 데이터를 `collection`이라 부르고, 단일 데이터를 `element`라고 부른다.

```javascript
{
    "topics":[
        {"id":1, "title":"html", "body":"html is ..."},
        {"id":2, "title":"css", "body":"css is ..."}
    ]
}

// POST
const URL = 'http://localhost:3000/topics';
const data = {id: 4, title: 'gimotti', body: '오마에와 모 신데이루..'};

response = await fetch(URL, {
        method: 'POST',
        headers: {
            'Content-Type': 'application/json',
        },
        body: JSON.stringify(data)
    });
result = await response.json
```

지금은 `POST`만 구현했지만 이처럼 `fetch` 혹은 `axios`를 이용해 데이터를 `CRUD` 할 수 있다.

### ❏ 실습 강의
1. `CI/CD`: `commit` 한번만으로 자동으로  `discord` 에 알림 설정하고 배포까지 한다. 
2. 해당 아이콘은 배포용으로 적합하지 않다는 뜻, 개발용으로만 사용하기

![](https://images.velog.io/images/abcd8637/post/8d63ca10-fb19-493c-ab7b-dae63589a436/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-18%2015.24.10.png)

3. `development`: 디버깅 및 개발 환경
4. `production`: 실제 배포 환경
5. `node.js`로 `development`로 배포한다면 오류가 어디에서 났는지 알 수 있기 때문에 보안에 취약하다
6. `front`에서 `development`로 배포하면 `production`보다 느리다. `development`에서는 `warning`이 잘 보인다. 반면에, `production` 에서는 `warning` 같은것이 뜨지 않는다. `production`은 가볍다. 개발모드와 배포모드의 속도차이는 약 4배(2017년 기준)
7. `npm run build`를 작성하면 `production`모드로 `build` 해주는데, `build` 폴더에서 파일을 클릭하면 코드가 한줄로 작성되어 코드를 읽기 힘들다. 
8. `scripts` 객체에서 명령어를 사용하려면 `npm run`을 작성하자
9. `serve -s build`: 배포용 버전 확인

```javascript
// 배포용에서만 확인 할 수 있는 코드
if(process.env.NODE_ENV === "production"){
	console.log("현재 Production 빌드로 돌아가고 있어요!")
}
```

10. `<script src=""></script>`로 `js` 파일을 불러오면 `window`인 전역객체에 생성되므로 나중에 생성한 파일이 이전에 생성한 함수의 값을 변경할 수도 있다. 이를 보완하기위해 `webpack`으로 번들링하여 보관한다.
11. `cloud`, `web hosting`: 개인적으로 서버를 빌려 운영하면 가격이 비쌈(`VM`), 반면에, `heroku`와 같이 `PasS`를 이용하여 서버의 일부자원을 이용하는 작업은 소스코드를 올려주어 페이지를 띄우는 작업이라 비용이 들지 않는다. 
12. `AWS`: 점유율이 높고, 매우 안정적이며 다양한 기능을 제공하지만 가격이 비싸다...
13. `oracle`, `google cloud`: 가입시 프리티어 무료 제공
14. `프론트만 쌩으로 돌린다.`: `Github Page`, `Netlify`, `Vercel`
15. `Node.js`도 돌린다: 시간제한이 괜찮다면 `Heroku`
16. `Nginx`같은 웹 서버도 돌리고, 다양한 작업을 한다: `2G`, `1 Core`로 충분
17. `Docker`도 돌리고 싶다: 최대 `8G`, `4 Core`..
18. 실물서버의 단점: 데이터 복구시 절차가 까다롭다. 
19. `NGINX`(web server): http를 통해 웹 브라우저에서 요청하는 HTML문서나 오브젝트을 전송해주는 서비스 프로그램을 말한다. `SSL`, `forward proxy`, `reverse froxy`, `cache`, `로드 밸런서`, `정적이고 가벼운 데이터 제공`시 사용하기에 적당하다.
20. `proxy-server`: 클라이언트와 서버 중간에서 무언가를 해주는 서버
21. `reverse-proxy`: 클라이언트가 요청하면 `Nginx`가 대신해서 응답해준다. 서버의 보안을 높일 수 있다
22. `Docker`: 한 서버에서 서로 같은 두 개의 서비스를 만들려면? 서버를 컨테이너로 나눈다면 개발환경을 구축하다가 충돌이 발생하거나, 의존성이 꼬일 필요가 없다.(가상화)
23. `CI(Continuous Integration) / CD(Continuous Deployment)`: 통합, 배포를 자동으로 해주는 과정, 단순하게 커밋만 하면 배포까지 한번에 된다. 원래는 `GitLab` 의 기능이었으나 `github` 에서  `github-action` 를 만들어 제공했다. 현업에은 `Jenkins` 를 주로 사용한다. `Jenkins` 는 별도의 서버를 요구한다. `Travis CI`: 상황에 따라 유료인점을 감안하기
24. `web-hook`: 특정 이벤트가 발생했을 때 타 서비스나 응용프로그램으로 알림을 보내는 기능(다른 팀원이 커밋하면 해당 코드를 바로 볼 수 있음)
25. `web-hook` 디스코드로 설정하기: 서버 생성 → 이 서버 설정 → 웹 후크 → URL 복사 → `github settings/webhook` → `payloadURL`에 붙여넣고 끝에 `/github` 붙여주기
26. `yml`: 들여쓰기를 신경쓰는 문법
27. `git action` 빌드 중 중간에 에러가 발생하면 그 이후의 작업은 수행하지 않는다.

---
## 📍 62일차 1.19.수. 온라인 강의
오늘은 `SSR`과 `CSR`, 간단하게 `Next.js`를 사용하는 법에 대해서 배웠다. 이전에 병과테스트 프로젝트를 react로 구현 하면서 SSR에 대해서 관심이 생겼는데 이번에 깊게는 아니어도 작동하는 원리, 간단한 예제등을 배울 수 있어서 좋았다.

### ❏ Server Rendering
1. React, Vue, Angular 등 자바스크립트 프레임워크가 나오기 이전 초기 웹 환경에서는 모든 페이지를 서버에서 빌드
2. 클라이언트는 별도의 처리 없이 웹페이지 노출 이를, `Server Rendering` 이라고 함

### ❏ Client Side Rendering
1. `Ajax` 등의 기술, 자바스크립트 프레임워크를 활용하여, 데이터를 받아 자바스크립트로 페이지를 동적으로 만들 수 있게 됨(`XMLHTTPRequest`)
2. 데이터는 `XML`, `JSON` 형태로 클라이언트에 전송하는데, 이를 `CSR`이라고 함

### ❏ CSR의 장점
1. CSR은 자바스크립트만으로 완전히 페이지를 만들 수 있다.
2. 자바스크립트를 최대한도로 활용하여 HTML, CSS를 동적으로 생성
3. 컴포넌트 단위로 코드를 나누고, 다양한 디자인 패턴을 적용하는 등 클라이언트 개발의 수준을 한 단계 끌어올림.
4. Full page load 없이 라우팅(페이지 이동시 매번 새로고침을 할 필요가 없음)

### ❏ CSR의 단점
1. `JS` 코드가 많으면 앱 로딩이 느려짐
2. `SEO` 가 좋지 않음(검색엔진이 아예)
3. `crawler` 는 서버에 페이지를 요청하고 서버는 HTML, CSS, JS를 내려줄 수 있지만 `crawler` 는 HTML만을 읽어서 페이지에 어떤 정보가 있는지 판별함 `crawler` 가 HTML을 읽어서 얻은 정보를 DB에 저장하고, 나중에 user가 search engine에 검색했을 때 DB에서 정보를 꺼내게 된다. CSR의 경우 JS에서 페이지를 만들기 때문에 초기 HTML을 내려줄때는 정보가 별로 없다.

### ❏ SSR
1. 서버에서 자바스크립트(`js engine`)를 이용해 페이지를 미리 빌드
2. 컴포넌트 생성에 필요한 `API 요청`, `routing`, `redux store` 생성 등을 처리.
3. 클라이언트는 빌드된 페이지와 자바스크립트를 받아 웹앱을 CSR처럼 동작하게 함(`hydration`)
4. 이런 특징으로, `Universal Rendering`이라고도 함
5. `server rendering` 은 `MPA` 라고도 부름.
6. CSR은 자바스크립트 프레임워크를 활용하여, 데이터를 받아 자바스크립트로 페이지를 동적으로 만들 수 있게 된다.

![](https://images.velog.io/images/abcd8637/post/4befebbc-69ae-42ca-9a6d-d7bd41722b38/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-19%2010.52.09.png)

### ❏ SSR의 장점
1. `Crawler`는 페이지를 `Indexing`하기 위해 페이지에 관한 많은 정보가 필요
2. `SSR`을 활용하여 미리 페이지를 빌드하면, `Crawler`에게 많은 정보를 줄 수 있음
3. `SEO`(Search Engine Optimization)에 유리

### ❏ SSR의 단점
1. `CSR`에 비해 `TTFB(Time To First Byte)`에 불리함(서버에서 미리 빌드를 하고 있어야 하기 때문, 시간이 오래걸리면 오히려 CSR보다 느려질 수 있다.)
2. 별도의 서버를 유지하는데 비용(유저가 많을 경우 서버를 여러 대 유지해야할 수 있음)이 듦
3. `CSR` 보다 `CDN Caching`에 불리함(같은 요청 시 `CDN`에 직접 요청할 수도 있음, 도메인 관리 서버에서 직접 서버로 요청할것인지 CDN으로 요청을 보낼 것인지 관리를 할 수 있다.)

### ❏ 웹 퍼포먼스
1. 웹 페이지가 로드되고 유저와 상호작용하는 모든 것들을 측정
2. 성능을 측정하여 웹앱의 사용성을 개선할 수 있음
3. 열악한 네트워크 환경에서도 사용 가능한 앱을 만드는 등 좋은 유저 경험으로 유저의 만족을 얻음
4. `Time To First Byte` , TTFB

```
1. 브라우저에서 서버로 페이지 요청 후 서버가 브라우저에게 처음 데이터를 전달할 때 도착하기까지 걸리는 시간
2. 요청을 받았을 때, 서버에서 처리하는 시간이 오래 걸리거나, 네트워크가 딜레이되는 등의 상황 발생 시 지표가 악화됨
3. 브라우저의 요청이 서버까지 가는 시간
4. 서버에서 요청을 처리하는 시간
5. 서버에서 브라우저까지 응답이 가는 시간
```

5. `First Contentful Paint`: FCP

```
1. 페이지에 진입하고부터, 브라우저가 어떤 DOM Content를 만들 때까지 걸리는 시간
2. 페이지 진입 후 FCP(뭐라도 paint되는 시간)까지 평균 3초 이상 걸리면 성능 개선이 필요
3. 브라우저에서 HTML, CSS, JS 등을 파싱하는 시간
4. 브라우저에서 페이지를 그리는 시간
```

6. `Time to Interactive`: TTI

```
1. 웹 페이지 진입 후, 유저가 클릭, 스크롤, 인풋 등의 행위를 하기까지 걸리는 시간
2. 자바스크립트가 로드되고 나서, 이벤트 핸들러 등이 부착되어 입력을 처리할 수 있기까지의 시간
3. JS가 처리되어 DOM에 이벤트를 부착하는 시간
```

### ❏ CSR, SSR의 페이지 로드방식
1. 먼저 CSR의 페이지 로드방식은 다음과 같다.

```
1. 브라우저에서 HTML을 요청한다.
2. 서버에서 HTML을 응답한다.(TTFB)
3. 브라우저에서 JS를 요청한다.(script태그를 만나면)
4. JS 응답
5. JS 엔진으로 페이지 빌드
6. data 요청(axios, API 등등)
7. data 응답
8. 페이지 로드 완료(FCP, TTI)
9. CSR은 브라우저에서 JS를 끄고 리로딩을 하면 내용물조차 보이지 않는다.
```

![](https://images.velog.io/images/abcd8637/post/62c5a210-dd2d-4dc3-8ebe-f3f6c83a1e0e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-19%2011.01.17.png)

2. SSR의 페이지 로드 방식

```
1. 브라우저가 HTML을 요청한다.
2. 서버에서 페이지를 빌드하는 시간이 소요된다(CSR과 다른 부분), 경우에 따라 API 데이터 요청, routing, redux store 처리, dom 생성 등
3. HTML 응답(TTFB, FCP)
4. JS 요청
5. JS 응답
6. Rehydration(TTI): input, navBar가 완벽하게 동작하지 않음(js가 모두 파싱되기 전까지)
7. data 요청
8. data 응답
9. 페이지 로드 완료
10. SSR은 브라우저에서 JS를 끄고 리로딩을 하면 내용물은 보여도 동작하지 않는다.
11. 유저가 빠르게 페이지의 내용을 볼 수 있도록 HTML을 미리 빌드하여 FCP등의 키 메트릭을 개선한다.
12. 서버 자원을 활용하여, 초기 큰 성능이 필요하거나 내용이 많은 페이지 등을 미리 빌드하는 데 활용한다. 
```

![](https://images.velog.io/images/abcd8637/post/171124ca-4102-4336-8676-340d17a6670e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-19%2011.05.05.png)

### ❏ React를 활용하여 SSR구축하기
1. `ReactDOMServer`를 활용하여, 특정 `React Component`를 가상의 DOM에서 HTML로 빌드
2. `Node.js` 서버에서 `JSX`를 사용하여 페이지 빌드

```
1. `renderToString`: `React component`를 `HTML`로 변환, 한꺼번에 모든 페이지를 만들어서 리턴하기 때문에 브라우저가 기다려야한다.(`ReactDOMServer.renderToString(<App />)`)
2. 클라이언트의 페이지 요청 시, 변환된 HTML string을 전달
3. `renderToNodeStream`은 DOM서버가 조금씩 페이지를 만들어서 `readable stream` 에 전달함.브라우저가 받아서 점진적으로 페이지를 부분적으로 보여줄 수 있음
4. ReactDOM.hydrate: CSR에서 동작하는 객체, renderToString으로 생성한 HTML의 root를 기준으로, 받아온 React code를 통해 markup에 이벤트 핸들러를 등록하는 등 컴포넌트화
5. Hydration 시 주의할 점
  - 서버에서 생성한 컴포넌트와 브라우저에서 Hydration을 거친 후의 마크업이 다르면, React runtime은 경고를 보냄 (ex, 현재 시간을 보여주는 컴포넌트)
  - 경고 발생 시, 어느 부분에서 차이점이 생기는지 반드시 파악해야 함
  - componentDidMount 역할을 하는 useEffect의 경우, SSR시 서버에서 동작하지 않음, 이때는 getInitialProps로 초기 데이터를 채운 다음에 페이지를 보내는 방법을 사용할 수 있다.
  - data loading 등의 처리를 별도로 해주어야 할 필요가 있음
```
6. 실습1: div root 내부에 html 컴포넌트 생성: <a href='https://github.com/YWTechIT/ssr-with-react-node-practice'>github</a>
7. 실습2: next.js router 해보기: <a href='https://github.com/YWTechIT/next-js-init-practice'>github</a>

### ❏ React 앱 배포 overview
1. 인터넷에서 내가 만든 앱에 접근할 수 있어야 함
2. 지속적으로 앱을 수정하고 배포해야 함(bug, feature 등...)
3. Public IP 주소 혹은 DNS로 직접 접근할 수 있도록 함

![](https://images.velog.io/images/abcd8637/post/690b688d-f9ac-4589-9689-915c58033ec9/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-19%2014.37.25.png)

4. 서버와 통신시, CORS가 허용되었는지 점검
5. 브라우저, 디바이스별로 앱이 정상적으로 동작하는지 점검
6. 앱의 로딩 속도, 각 동작 시 성능, 버그 등을 점검
7. IP를 부여받은 서버(VM)에 React앱을 배포 → 앱을 빌드하고, 웹서버를 세팅 → 앱을 서빙하는 웹서버를 통해 사용자에게 앱을 전달 → 사용자는 필요한 데이터를 받아 앱을 로딩

```
git clone ${url}
cd ${project_name} 
npm i 
sudo npm i -g serve  # build 후 간단한 웹서버를 띄워줌
npm run build
sudo -s(serve) -p(port) 80 build(directory)  # serve 웹 서버를 사용해 프로젝트를 80번 포트에서 서빙함
```

### ❏ React 앱 준비
1. `yarn.lock`, `package-lock.json` 이 동시에 존재하지 않는지 점검(npm과 Yarn dependency가 충돌에서 build가 실패할 수 있음)
2. 로컬에서 `npm run build` 를 실행하여, 빌드 시 에러가 발생하지 않는지 점검하자.(로컬에서 빌드시 에러가 발생하면 서버에 배포했을 때에도 에러가 발생할 여지가 있다.)
3. 로컬에서 배포하여, `production build` 가 제대로 실행되는지 점검하기.

### ❏ Gitlab 연동
```bash
> git remote add origin ${git repository url}
> git push --set-upstream origin master
```

---
## 📍 63일차 1.20.목. 실시간 강의
오늘은 화요일에 배웠던 `CI/CD`, `github-actions`, `Heroku`, 그리고 백엔드 서비스를 구축 할 때 서버 인프라 구축을 쉽게 할 수 있도록 도와주는 `firebase`에 대해서 배웠다. 이 강의를 듣기 전에 `CI/CD` 관련한 내용을 봤을 때 저게 대체 왜 필요하지? 라는 생각이 들었는데, 직접 해보니까 자동화 구축이 주는 효과는 굉장했다!! `CI/CD`를 배웠지만 여기서 그치지 않고 내가 직접 프로젝트를 만들 때 사용할 수 있을 정도까지 공부하고 싶다는 생각이 들었고 `firebase`가 무엇인지 배우면서 `Authentication`, `NoSQL`, `Storage`, `Hoisting`을 적용해보고 싶다는 생각이 들었다. 개념을 새로 배울 때마다 이론에서 그치지 않고 어떻게 실전에 써먹어 내것으로 만들까 생각하지만, 배운내용이 많아서 한꺼번에 적용하려니까 버거웠다. 천천히 한 개념씩 적용하다보면 언젠간 손에 익지 않을까? 

1. `react` 개발환경에서 `proxy` 를 쓰는 이유

```js
 1. 절대경로(ex `https://www.example.com/todos`) 대신 proxy를 사용하여 상대경로(`/todos`)로 요청해도 React에서는 에러가 나지 않는다.
  * 상대경로로 작성하면 나중에 URL이 바뀔 때 일일이 바꾸는 것보다 package.json에서 URL만 바꾸면 모두 적용되므로 간편하다.
 2. 예를 들어, 브라우저는 `localhost:8080`이고 서버에서 데이터를 받아오는 URL은 `localhost:8888/todos` 라면, 상대경로를 '/todos'로 작성했을 때 react는 브라우저 서버인 `localhost:8080/todos`로 요청하게 된다. 분명 해당 주소는 값이 없기때문에 에러를 내지만, `package.json`의 `proxy`를 보고 react가 `proxy(중계)`역할을 대신한다. 따라서 `localhost:8888/todos`로 요청하게 되고 해당 주소의 데이터를 가져올 수 있게 된다.
  * 이전까지는 `브라우저 <-> react`, `브라우저 <-> 백엔드`와 통신을 지속했지만, react가 `proxy(중계서버)`역할을 하면서 `브라우저 <-> react <-> 백엔드` 순으로 통신을 하게된다.
 3. 이렇게 통신할 때의 장점은 `CORS`에 적용되지 않는다는 점이다. (서버와 서버간에는 `SOP`가 적용 되지 않는다. 그렇기 때문에 백엔드에서 데이터를 `react`로 가져오고 `react`는 `browse`r로 걱정없이 데이터를 뿌려 줄 수 있게 된다.)
```

2. `mui.com(material UI)`: 디자인 시스템을 제공하는 React UI Framework
3. `npm install @mui/material @emotion/react @emotion/styled`
4. `git reset --hard hash`: 해당 커밋으로 이동

### ❏ 실습
1. <a href='https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions#overview'>Git Actions</a>
2. CI(Continous Intergration): 통합시키는데 초점
3. CD(Continous Deployment): 배포하는데 초점
4. `Github - actions`:  빌드, 테스트 및 배포 파이프라인을 자동화할 수 있는 `CI/CD`(지속적 통합 및 지속적 전달) 플랫폼. `PR` 혹은 `Merge` 와 같은 이벤트가 일어날 때 workFlow를 트리거 할 수 있다. 각 작업은 자체 가상 머신 실행기 내부 또는 컨테이너 내부에서 실행되며, 사용자가 정의한 스크립트를 실행하거나 작업을 실행하는 하나 이상의 단계가 있다.
5. `workFlow`: 하나 이상의 작업을 실행하는 자동 프로세스, `YAML` 으로 파일을 작성하며, PR, merge와 같은 이벤트, 수동 설정, 스케쥴에 의해 트리거하게 설정할 수 있다.

![](https://images.velog.io/images/abcd8637/post/060f2c32-0f94-49cf-8344-8d84facddffe/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-20%2015.12.36.png)

6. 단계별로 나눠서 `build` 할 때는 독립된 형태로 `build` 한다.

```yaml
name: first-CI-practice  # 이름: 이후에 CI가 동작하는 과정에서 이름으로 뜬다.

on:  # 어떤 경우에 아래 동작을 시행할 것인가?
  push:  # code push 할 때
    branches: [ master ]
  pull_request:  # code PR 할 때
    branches: [ master ]

jobs:  # 실제 동작

  build:  # 동작의 이름(바꿔도 됨), 첫번째 CI
    runs-on: ubuntu-latest  # 우분투 최신 버전 적용
    strategy:  # 매개변수 네이밍시 사용
      matrix:
        node-version: [12.x, 14.x, 16.x]
        # See supported Node.js release schedule at https://nodejs.org/en/about/releases/

    steps:  # 실제로 돌아가는 동작
    # '-'는 각각의 동작을 의미함.
    - uses: actions/checkout@v2  # 플러그인 사용, 워크플로가 실행될 때마다 체크아웃 작업을 사용한다.
    - name: Use Node.js ${{ matrix.node-version }}
      uses: actions/setup-node@v2
      with:
        node-version: ${{ matrix.node-version }}
        cache: 'npm'
    - run: npm ci
    - run: npm run build --if-present
    - run: npm test

	test:  # 두번째 CI
	  runs-on: ubuntu-latest
		needs: build  # build 단계 이후 실행
	  strategy:
	    matrix:
	      node-version: [12.x, 14.x, 16.x]
	
	  steps:
	    - uses: actions/checkout@v2  # 플러그인 사용
	    - name: Use Node.js ${{ matrix.node-version }}
      uses: actions/setup-node@v2
      with:
        node-version: ${{ matrix.node-version }}
        cache: 'npm'
	    - run: npm ci
	    - run: npm run build --if-present
	    - run: npm test
```

7. `actions/cache`: `actions`의 의존성을 매번 새로 작성하거나 빌드한 결과물을 다른데에 사용하고 싶다. 
8. `yml` 로 파일을 만들고 수정(연필)버튼을 누르면 `marketplace` 가 뜬다. 여기서 원하는 `CI/CD` template를 가져 올 수 있음
9. `Heroku`

```js
1. 유럽보다 미국이 태평양을 바로 지날 수 있어서 속도가 조금 더 빠르다.
2. Heroku가 cloud의 기능을 대신 해줌(Load balance, Auto scaling 등...)
3. Heroku CLI: git <-> heroku, git Action을 쓸 수 없음
4. Github Action + Heroku plugin
5. Github Actions에서 heroku_api_key는 그대로 commit하지 말고 secret에 넣어서 ${{secrets.api_key}}로 사용하자 대신 actions에 한번 secret을 업로드하면 작성자조차 무슨 값인지 다시 볼 수 없다.
6. 개발 -> commit -> Github -> Action -> Test -> Heroku
7. 개발 -> commit -> P/R -> Test(코드리뷰) -> build -> deployment
8. actions를 사용하는 큰 이유: 각종 테스트로 정상적으로 배포 할 수 있는 상태인지 확인할 수 있다. 특정상황에서 배포, 추가적인 명령어 설정 등 원하는조건에서 배포 할 수 있게끔 커스터마이징이 가능하다.

- name: Generate.env file
  run: |
      echo "DISCORD_TOKEN=$DISCORD_TOKEN" >> .env
      echo "WEATHER_API_KEY=$WEATHER_API_KEY" >> .env
    env:
      DISCORD_TOKEN: ${{ secrets.DISCORD_TOKEN }}
      WEATHER_API_KEY: ${{ secrets.WEATHER_API_KEY }}
```

9. `firebase`: 기본적인 서비스 구축하기 위한 서버 인프라 구축, 서버단 세팅 등을 고민하지 않고 클라이언트 단의 작업만 진행하여 서비스를 제작할 수 있는 플랫폼, 전통적인 서버 구성처럼 매번 서버 - DB를 나누어 데이터를 가져와서 관리해야하는 불편함을 덜수 있음. `Baas(Backend as a Service)`, `RealTimeDB`, `Cloud Firestore(NoSQL DB)`, `Storage`, `OAuth`, `Hosting`, `CDN`, `Cloud Functions` 등 지원하는 기능이 생각보다 많다. 백엔드를 관리할 필요없이 클릭 몇번으로 서버를 관리할 수 있다.
10. `npm i firebase`, `npm i -g firebase-tools`
11. `firebase login`
12. `firebase deploy`
13. `firebase 사용 예시 코드`

```javascript
// App.js
import React, { useState, useEffect } from 'react';
import './App.css';
import { FormControl, Button, Input, InputLabel } from '@material-ui/core';
import Todo from './Todo';
import db from './firebase_setting';
import firebase from 'firebase/compat/app';
import 'firebase/compat/firestore';

function App() {
  const [todos, setTodos] = useState([]);
  const [input, setInput] = useState('');

  useEffect(() => {
    db.collection('todos')
      .orderBy('timestamp', 'desc')
      .onSnapshot(data => {
        setTodos(data.docs.map(doc => ({ id : doc.id, todo: doc.data().todo })))
      })
  }, [input])

  const addTodo = (e) => {
    e.preventDefault();
    db.collection('todos').add({
      todo: input,
      timestamp: firebase.firestore.FieldValue.serverTimestamp()
    });
    setTodos([...todos, input]);
    setInput('');
  }

  return (
    <div className="App">
      <h1>Hello World</h1>
      <form>
        <FormControl>
          <InputLabel>Write a Todo</InputLabel>
          <Input value={input} onChange={e => setInput(e.target.value)} />
        </FormControl>
        <Button disabled={!input} type="submit" variant="contained" color="primary" onClick={addTodo}>Add Todo</Button>
      </form>
      <ul>
        {todos.map(todo => (
          <Todo todo={todo} />
        ))}
      </ul>
    </div>
  )
}

export default App;
```

---
## 📍 64일차 1.21.금. 온라인 강의
오늘은 `CSS Module`, `UI Framework`, `CSS framework`, `CSS-in-JS`, `Styled-components`에 대해서 배우고 전반적인 사용 역사(?)에 대해서 배웠다. 기존에 사용하던 방식의 단점, 불편함 때문에 새로운 방식이 나왔고, 새로운 방식에서 생겨난 단점, 불편함을 통해 새로운 방식을 사용하고.. 이렇게 일련의 과정들을 배우니까 이해가 잘 됐다. 그리고 평소에 관심있던 리팩토링에 대해서도 배웠는데 일련의 과정들을 보면서 리팩토링의 `before / after`를 보며 가독성이 어떻게 증가되었는지 한번 살펴보자. 마지막에는 `figma`의 조작법을 3가지정도만 작성했다. 한번 살펴보자.

### CSS Module
1. 기존 `CSS`의 단점: 하나의 스타일 `sheet`가 여러 컴포넌트에 영향을 미친다.
2. CSS module을 사용하면 `class`, `id` 등 선택자가 겹칠 우려가 없음 (`hash`값 사용)
3. 스타일 충돌을 방지하고 코드를 격리하여 체계적으로 CSS 설계가 가능
4. CSS module의 단점은 개발자가 스타일링을 직접 하나하나씩 해야한다는 점이다. 

```javascript
// App.jsx
import styles from "./app.module.css";

export default function App(){
	return(
		<div>
			<h1 className={ styles.title }>Pink Hello world</h1>  // hash가 붙어있음
			<h1 className={ "title" }>Hello world</h1>  // 그냥 title
		</div>
	)
}

// app.module.css
h1 {
	font-size: 1.5rem;
}

.title {
	font-size: 2.5rem;
	color: pink;
}
```

### UI Framework
1. 종류: `MUI(material UI)`, `Ant design`
2. 장점은 이미 만들어져 있는 스타일이기 때문에 간편하고 쉽게 사용하기 좋다.
3. 단점으로는 이미 다 만들어져 있기 때문에 styling의 학습 및 훈련이 필요한 초심자들에게는 비추천한다. 또한 해당 framework의 디자인철학을 벗어나기 쉽지 않고, 컴포넌트들을 커스터마이징하기 어려움

```javascript
// App.jsx use Ant design
import "antd/dist/antd.css";
import { Button } from "antd";

export default function App(){
	return(
		<div>
			<Button type="primary">Primary Button</Button>
			<Button type="secondary">Secondary Button</Button>
			<Button type="danger">Danger Button</Button>
		</div>
	)
}
```

### CSS Framework
1. 종류: `Tailwind CSS`, `w3.css`
2. 거대한 CSS 파일 하나를 가져오는 것
3. 장점: 개발자가 따로 CSS 파일을 작성하지 않아도 HTML에 클래스만 적어주면 정해진 규칙대로 스타일링이 적용됨.
4. 단점: CSS에 대한 이해력이 있어도 해당 framework를 사용하기 위한 학습을 또 다시 해야함, 이미 다 만들어져 있어서 styling의 학습 및 훈련이 필요한 초심자들에게는 비추천

```javascript
// W3CSS 예시
import { Helmet } from "react-helmet";

export default function App(){
	return(
		<div>
			<Helmet>  // <head></head>
				<link
					rel="stylesheet"
					href="https://www.w3schools.com/w3css/4/w3.css"
				</>
			</Helmet>

			<div className="w3-container w3-green">
				<h1>W3Schools Demo</h1>
				<p>Lorem</p>
			</div>
		</div>
	)
}
```

### CSS-in-JS
1. 종류: `Styled-components`, `emotion`
2. 따로 CSS 파일을 만들지 않고 JSX 파일 안에서 스타일링까지 해결 가능함
3. 컴포넌트 재사용성이 쉬워짐
5. JS 값을 props로 넘겨줘서 해당 JS 값에 의도된 styling을 바로 적용할 수 있다.
6. class 이름에 hash값을 생성하여 선택자 이름이 겹칠 우려가 없다.
7. 스타일링을 개발자가 직접 해야함

```javascript
import styled from "styled-components";

const Title = styled.hi`
	font-size: 1.5rem;
	text-align: center;
	color: pink;
`

export default function App(){
	return <Title>Hello world</Title>
}
```

### ❏ 기존 CSS 문법을 SCSS로 리팩토링하기
리팩토링하면서 느낀것이지만 `SCSS`로 작성했을 때의 장점은 코드를 계층적으로 작성할 수 있다는 것이었다. 따라서, 부모 - 자식간의 관계를 코드를 통해 유추 할 수 있었고, 동일한 선택자를 불필요하게 여러번 사용할 필요없이 `&`으로 대체해서 사용하거나, 현재 선택자 이외에 다른 선택자만 사용하는 등 간편하게 사용하는 점이 좋았다.

```scss
/* 기존 CSS 문법 */
.container {
  padding: 10px;
  background-color: lightgray;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.counter {
  width: 100px;
  height: 50px;
  line-height: 50px;
  font-size: 2rem;
  border: 1px solid black;
  border-radius: 8px;
  text-align: center;
}

.buttons-container {
  margin-top: 20px;
}

button {
  color: white;
  width: 80px;
  height: 50px;
  text-align: center;
  border-radius: 10px;
}

button + button {
  margin-left: 10px;
}

button.inc {
  background-color: blue;
}

button.dec {
  background-color: red;
}
button:hover {
  box-shadow: 10px 5px 5px gray;
}

/* SCSS 리팩토링 */
/* 어떤 클래스안에 종속되어있는지 계층적으로 확인이 가능하다. 
동일한 선택자는 제거하고 &로 대체 할 수 있다. 가독성이 증가하는 효과가 있음 */
.container {
  padding: 10px;
  background-color: lightgray;
  display: flex;
  flex-direction: column;
  align-items: center;
  
      .counter {
      width: 100px;
      height: 50px;
      line-height: 50px;
      font-size: 2rem;
      border: 1px solid black;
      border-radius: 8px;
      text-align: center;
    }
    
      .buttons-container {
          margin-top: 20px;
      
        button {
          color: white;
          width: 80px;
          height: 50px;
          text-align: center;
          border-radius: 10px;
          
          + button { 
            margin-left: 10px;
          }
          
          &.inc {
            background-color: blue;
          }
          
          &.dec {
            background-color: red;
          }
          
          &:hover{
            box-shadow: 10px 5px 5px gray;
          }
        }
    }
}
```

### ❏ JavaScript template literal
1. 문자열 안에서 JS 표현식을 사용할 수 있게 하는 문법이다. `string text ${expression} string text`

```javascript
const string = "elice"
const message = `hello ${string}`;
console.log(message)  // "hello elice"

const number = 12345
const message = `hello ${number}`;
console.log(message)  // "hello 12345"

const boolean = true;
const message = `hello ${boolean}`;
console.log(message)  // "hello true"

const object = { a: "apple" };
const message = `hello ${object}`;
console.log(message)  // "hello [object object]"

const name = "Ted";
const gender = "male";
const message = `hello ${gender === "male" ? "Mr. " : "Mrs."}`;
console.log(message)  // "hello Mr.Ted, nice to meet u";
```

### ❏ Styled-components
1. `props` 유무에 따른  `styled-components` 작성 방법

```javascript
// props가 없는 경우
const Button = styled.button`
  font-size: 32px;
	margin: 1em;
	padding: 0.25em 1em;
`

function App(){
	return <Button>Hello!</Button>
}

// props가 있는 경우
const Button = styled.button`
  font-size: 32px;
	margin: 1em;
	padding: 0.25em 1em;
	background: ${(props) => props.primary ? "pink" : "black"}
	color: ${(props) => props.primary ? "white" : "green"}
`

function App(){
	return <Button primary>Hello!</Button>  // primary = true와 같음
}
```

2. `css` vs `scss` vs `styled-components`

```scss
// CSS
.name .red {
	color: red;
}

.name .blue {
	color: blue;
}

.name .green {
	color: green;
}

.name .child .yellow {
	color: yellow;
}

.name + .name {
	color: purple;
}

// SCSS: 중복된 선택자 제거 가능
.name {
	&.red {
		color: red;
	}

	&.blue {
		color: blue;
	}

	&.green {
		color: green;
	}

	.child {
		.yellow {
			color: yellow;
		}
	}

	+ .name {  /* 인접요소 연산자 */
		color: purple;
	}
}

// SCSS in styled components
const SCSSStyledDiv = styled.div`
	background-color: orange;
	color: white;

	div{   // SCSSStyledDiv 내부의 div태그의 bg color
		background-color: red;
	}

	.purple{  // SCSSStyledDiv 내부의 purple 클래스의 bg color
		background-color: purple;
	}
`

// Componennt Use Case
function Test(){
	return (
		<SCSSStyledDiv>
			<div className={"purple"} />
	)
}
```

3. style-components 로 CSS 수정하기

```js
// CSS
.container {
  margin: 0 auto;
  width: clamp(0px, 100%, 860px);
  padding: 10px;
  background-color: lightgray;
  text-align: center;
}

.count {
    width: 128px;
    margin: 0 auto;
    margin-bottom: 16px;
    padding: 16px;
    border: 2px solid black;
    border-radius: 16px;
    font-size: 32px;
    font-weight: 700;
}

.button-wrapper {
    margin-bottom: 16px;
}

button {
    padding: 16px;
    background-color: blue;
    color: white;
    font-size: 32px;
    border-radius: 16px;
}

button:last-child {
    background-color: red;
}

button + button {
    margin-left: 16px;
}

button:hover {
    box-shadow: 8px 4px 4px gray;
}

// styled-components
const Container = styled.div`
  margin: 0 auto;
  width: clamp(0px, 100%, 860px);
  padding: 10px;
  background-color: lightgray;
  text-align: center;
`

const Count = styled.div`
    width: 128px;
    margin: 0 auto;
    margin-bottom: 16px;
    padding: 16px;
    border: 2px solid black;
    border-radius: 16px;
    font-size: 32px;
    font-weight: 700;
`

const ButtonWrapper = styled.div`
    margin-bottom: 16px;
`

const Button = styled.button`
    padding: 16px;
    background-color: ${(props) => props.bgColor };
    color: white;
    font-size: 32px;
    border-radius: 16px;
    
    & + & {  // 둘중에 하나 사용하면 됨
        margin-left: 16px;
    }
    
    + button {  // 둘중에 하나 사용하면 됨
        margin-left: 16px;
    }
    
    &:hover {
        box-shadow: 8px 4px 4px gray;
    }
`
```

### ❏ Figma
1. `shift + scroll` :횡으로 `scroll`
2. 좌측 Search: 컴포넌트 구조 확인 가능
3. 마우스 커서로 컴포넌트 사이의 거리 확인 가능(`px`)

---
## 📍 65일차 1.22.토. 온라인 강의
오늘은 직접 `React`와 `Styled-components`를 이용해서 트랙카드, 탭, 검색창을 초기 `UI`로 구현하고 이후에는 실제 `API`를 연동하면서 검색창에서 검색 데이터를 가져오는 방법까지 응용하는 법을 배웠다. 그리고 마지막에는 `JS`에서 `TS`로 마이그레이션 설정 방법에 대해서 배웠다. `CSS`를 배울 때 `position`과 같은 내용을 직접 적용하려고 할 때 어려움이 많았는데 이번 실습을 보면서 `position: absolute`의 사용시기를 잘 배울 수 있었고, 아무 조건에서 적용되는것이 아니라 부모가 `relative`일 때 적용된다는 점도 배웠다. 인상깊었던 부분은 `::before`연산자로 `background-color`를 만드는 방법인데, 평소에 잘 적용하지 않는 방법이어서 나중에 써먹을 수 있도록 따로 기록을 해놓았다. 그리고 검색창 구현시 `debounce`를 적용하여 매 입력마다 서버로 요청하지 않고 특정 시간 이후에 서버로 입력값을 요청하여, 서버입장에서 부하를 어느정도 줄여줄 수 있는 방법인데, 현업에서 많이 사용하는 방법이라서 까먹지 않아야겠다고 생각했다.

### Styled-components
1. `styled-components` 를 사용 할 때 다음과 같이 컴포넌트 하나마다 `import` 해야 할 상황이 많으면 `* as Card` 처럼 전체 페이지를 로드하고 `component` 앞에 `Card` 를 붙여  `after` 과 같이 사용하면 같은 결과를 반환해도 코드가 줄어들어 가독성이 올라간다.

```javascript
// before
import { 
		Container,
		Tags,
		Title,
		Description,
		TextsWrapper,
		TextWrapper,
		Chart,
		Text,
		Computer,
		Calendar,
		Image,
		LanguagesWrapper,
		Language,
		DividerLine,
		CostFree,
		CostWrapper,
		CurrentCost,
		OriginalCost,
		DiscountPercentile
} from "./js";

return (
    <Container>
        <Tags>{tags.join("﹒")}</Tags>
        <Title>{title}</Title>
        <Description>{description}</Description>
        <TextsWrapper>
            <TextWrapper>
                <Chart />
                <Text>난이도 : {level}</Text>
            </TextWrapper>
            <TextWrapper>
                <Computer />
                <Text>수업 : {classFormat}</Text>
            </TextWrapper>
            <TextWrapper>
                <Calendar />
                <Text>기간 : {duration}</Text>
            </TextWrapper>
        </TextsWrapper>
        <Image src={imgUrl} />
        <LanguagesWrapper>
            {languages.map((lang, idx) => {
                return (
                    <Language key={`${lang}-${idx}-${title}`} lang={lang}>
                        {lang}
                    </Language>
                );
            })}
        </LanguagesWrapper>
        <DividerLine />
        {isFree ? (
            <CostFree>무료</CostFree>
        ) : (
            <CostWrapper>
                <CurrentCost>
                    {currentCost.toLocaleString()}원
                </CurrentCost>
                <OriginalCost>
                    {originalCost.toLocaleString()}원
                </OriginalCost>
                <DiscountPercentile>
                    {discountPercentile}%
                </DiscountPercentile>
            </CostWrapper>
        )}
    </Container>
);

// after
import * as Card from "./Card.js";

return (
    <Card.Container>
      <Card.Tags>{tags.join("﹒")}</Card.Tags>
      <Card.Title>{title}</Card.Title>
      <Card.Description>{description}</Card.Description>
      <Card.TextsWrapper>
        <Card.TextWrapper>
          <Chart />
          <Card.Text>난이도 : {level}</Card.Text>
        </Card.TextWrapper>
        <Card.TextWrapper>
          <Computer />
          <Card.Text>수업 : {classFormat}</Card.Text>
        </Card.TextWrapper>
        <Card.TextWrapper>
          <Calendar />
          <Card.Text>기간 : {duration}</Card.Text>
        </Card.TextWrapper>
      </Card.TextsWrapper>
      <Card.Image src={imgUrl} />
      <Card.LanguagesWrapper>
        {languages.map((lang, idx) => {
          return (
            <Card.Language key={`${lang}-${idx}-${title}`} lang={lang}>
              {lang}
            </Card.Language>
          );
        })}
      </Card.LanguagesWrapper>
      <Card.DividerLine />
      {isFree ? (
        <Card.CostFree>무료</Card.CostFree>
      ) : (
        <Card.CostWrapper>
          <Card.CurrentCost>{currentCost.toLocaleString()}원</Card.CurrentCost>
          <Card.OriginalCost>{originalCost.toLocaleString()}원</Card.OriginalCost>
          <Card.DiscountPercentile>{discountPercentile}%</Card.DiscountPercentile>
        </Card.CostWrapper>
      )}
    </Card.Container>
  );
```

2. props 에 맞게 해당 컴포넌트의 css 를 추가하거나 변경하고 싶다면 다음처럼 사용하자

```javascript
// Card.js
import styled, { css } from "styled-components";

export const Container = styled.div`
  background-color: white;
  border: 1px solid #f0f1f3;
  border-radius: 8px;
  width: 296px;
  height: 407px;
  box-sizing: border-box;
  padding: 28px 24px 20px;
  position: relative;
  display: flex;
  flex-direction: column;
  
  ${(props) => props.large && css`
    width: 398px;
    height: 409px;
    padding-top: 32px;
  `}
`;

// TrackCard.jsx
export default function TrackCard() {
  return <Card.Container large />
}
```

3. `absolute` 상태에서 `left: 0, right: 0`으로 설정하면 `width: 100%` 와 마찬가지로 좌우로 쭉 펴진다. `left: 0, right: 0, top: 0, bottom: 0`으로 설정하면 상하좌우로 쭉 펴진 상태가 된다.
4. `navBar` 에서 원하는 메뉴를 클릭했을 때 `active` 시키는 방법은 `useState` 를 이용해서 해당 태그를 누르면 `active`되게 끔 설정하면 된다.

```javascript
// App.jsx
import { useState } from "react";
import Tab from "./Tab.jsx";

export default function App() {
  const [currTab, setCurrTab] = useState("트랙");
  const handleClickTab = (tab) => {
    setCurrTab(tab);
  }

  return (
    <Container>
      <Tab currTab={currTab} onClick={handleClickTab}/>
    </Container>
  );
}

// Tab.jsx
import styled, { css } from "styled-components";

const Container = styled.div`
    display: flex;
    border-bottom: 1px solid #E1E2E4;
    width: 100%;
`

const EachTab = styled.p`
    font-size: 14px;
    line-height: 22px;
    color: #151618;
    padding: 8px;
    
   & + & {
        margin-left: 16px;
    }
    
   ${props => props.active && css`
        color: $524FA1;
        font-weight: bold;
        background: rbga(230, 230, 230, 0.0001);
        box-shadow: inset 0px -4px 0px #524FA1;
   `}
`

const tabs = ["트랙", "과목"];

Tab.defaultProps = {
  currTab: "트랙",
  onClick: () => {},
};

export default function Tab({ currTab, onClick }) {
  return (
      <Container>
        {tabs.map((tab, i) => {
            return (
                <EachTab 
                    key={`${tab}-${i}`}
                    active={currTab === tab}
                    onClick={() => onClick(tab)}
                    >{tab}</EachTab>)
        })}
      </Container>)
}
```

5. 검색 창 만들기: `container` 안에 `input` 을 넣는다. 돋보기 모양은 `container` 안에서 `svg` 태그를 따로 설정해준다.

```javascript
// App.jsx
import { useState } from "react";
import SearchTextField from "./SearchTextField.jsx";

export default function App() {
  const [value, setValue] = useState("");
  const handleChangeValue = (value) => setValue(value);

  return (
    <Container>
      <SearchTextField value={value} onChange={handleChangeValue}/>
    </Container>
  );
}

// SearchTextField.jsx
import styled from "styled-components";
import MagnifyingGlass from "./icons/MagnifyingGlass.jsx";

const Container = styled.div`
    width: 100%;
    position: relative;
    
    svg {
        position: absolute;
        top: 15px;
        left: 12px;
    }
`;

const Input = styled.input`
    padding: 11px 11px 11px 39px;
    border: 1px solid #C9CACC;
    border-radius: 4px;
    height: 46px;
    box-sizing: border-box;
    width: 100%;
    font-size: 14px;
    line-height: 22px;
    color: #7D7E80;
`;

SearchTextField.defaultProps = {
  value: "",
  onChange: () => {},
};

export default function SearchTextField({ value, onChange }) {
  return (
    <Container>
      <MagnifyingGlass />
      <Input 
        placeholder="배우고 싶은 언어, 기술을 검색해 보세요."
        value={value}
        onChange={(e) => onChange(e.target.value)}
      />
    </Container>
  );
}
```

### React에서 TS로 마이그레이션 하기
1. 타입스크립트 라이브러리 설치

```javascript
* 새로 CRA를 생성하는 경우: npx create-react-app <project name> -template typescript만 작성
* 기존 JS 파일을 TS로 마이그레이션 하는 경우 하단 과정 시작

npm i -D typescript esbuild-loader @types/react @types/react-dom
yarn add -D typescript esbuild-loader @types/react @types/react-dom

- typescript: tsc 컴파일러, ts 문법 지원을 위해 필요한 라이브러리
- @types/react: react 라이브러리를 위한 타입 패키지
- @types/react-dom: react에서 dom element와 관련된 타입들을 모아놓는 패키지
  * @types/라이브러리 이름: 타입스크립트에서 라이브러리 설치할 때 사용하는 명령어(Definitely Typed 참고)
- esbuild/loader: 타입스크립트 트랜스파일링을 위한 패키지(속도가 매우 빠르다)
  * 본래는 babel-loader를 사용했으나, 최근 들어 webpack의 빌드를 빨리하기 위해 esbuild를 많이 사용하는 추세다
```

2. tsconfig.json 설정

```javascript
1. tsconfig.json 파일 생성 
  * tsc --init 혹은 npx tsc --init 입력 시 tsconfig.json의 기본적인 컴파일러 옵션을 설정해준다.

{
  "compilerOptions": {
    "target": "es5",  // 트랜스파일링을 할 경우 어떤 버전으로 변환 할 것인지(IE 지원은 es5로 설정)
		"outDir": "./dist/",  // 컴파일 후 어떤 경로로 저장할지?
		"sourceMap": true,  // 디버깅을 위한 소스맵이 필요한 경우에 설정
    "module": "esnext",  // 모듈 코드를 ESM(ECMAScript Module: import, export), CJS(Common JS: require, exports.module) 모드로 설정할것인가?
    "jsx": "react-jsx"  // jsx파일을 js파일로 변환하도록 하는 설정, react 설정시 jsx파일이 js로 변환된다.
  }
}

jsx 옵션은 preserve, react, react-native 3가지 옵션을 설정할 수 있습니다.
1. preserve: 바벨이나 swc 같은 다른 트랜스파일러가 변환할 수 있도록 jsx 문법을 트랜스파일링하지 않고 그대로 둡니다. 따라서 트랜스파일링 결과는 .tsx에서 .jsx 파일이 됩니다.

2. react: jsx 문법을 js로 변환시킵니다. 트랜스파일링 결과는 .js 확장자 파일입니다.

3. react-native: preserve 모드처럼 jsx 문법을 그대로 두지만 트랜스파일링 결과는 .js 확장자 파일이 됩니다.
```

3. 사용하는 라이브러리들 중 @types 패키지 추가(타입 전환)

```javascript
1. npm i -D @types/<library name>: DefinitelyTyped 오픈소스에 등록된 타입 선언 파일 설치
2. git repo에 index.d.ts에 있는 라이브러리면 설치 안해도 됨. 
3. npm에서 @types/패키지명 검색해보고 있으면 @types/패키지 설치하고 @types/패키지가 없다면 직접 모듈에 대한 타입을 선언해야 한다.
4. 모듈에 타입을 직접 선언했다면 다른 개발자도 사용할 수 있게 라이브러리에 DefinitelyTyped에 PR을 날려보자
```

4. `webpack` 설정 변경

```javascript
module.exports = {
  entry: {  // 앱을 시작할 파일
    main: "./src/index.js",
  },
  output: {  // 웹팩 번들링 결과에 대한 옵션, 기본 경로는 dist
    path: path.resolve(__dirname, "dist"),
    filename: "[name].js",
  },
  resolve: {  // 번들링할 확장자 설정
    extensions: [".js", ".jsx", ".ts", ".tsx"],
  },
  module: {  // 번들링 할 때 플러그인 설정 가능
    rules: [
      {
        test: /\.(t|j)sx?$/,
        loader: "esbuild-loader",  // 타입스크립트 변환을 위한 로더
        options: {
          loader: "tsx", // Or 'ts' if you don't need tsx
          target: "es2015",
        },
      },
      {
        test: /\.css$/,  
        use: ["style-loader", "css-loader"],  // style-loader: style 태그를 삽입해 dom에 css 추가, css-loader: css 확장자의 css파일을 읽기 위한 로더, css 확장자를 가져와서 style 태그를 삽입해 DOM에 css를 추가한다.
      },
    ],
  },
  externals: {  // 번들링 결과에서 제외할 라이브러리들
    react: "React",
    "react-dom": "ReactDOM",
  },
};
```

5. `jsx` → `.tsx` 로 확장자 변환

```javascript
- jsx 파일에서 tsx파일로 확장자 변경을 하고 이 과장에서 생기는 타입 오류들을 해결해야 마이그레이션이 끝난다.
```

---
## 📍 [선택강의] React에서의 타입스크립트
이번 글은 필수로 들어야하는 강의를 기록하기 위해 적는 글은 아니고 선택적으로 듣는 강의 중 `React에서의 타입스크립트` 강의를 기록으로 남겨 놓을까한다. 그 이유는 이전부터 사용해왔지만 앞으로도 사용할 언어인 타입스크립트와 프레임워크인 React기 때문이다. 그리고 지금까지 내가 작성한 코드를 어떻게 더 효율적이게 작성할 수 있을지에 대한 몇가지의 샘플을 배울 수 있기 때문이다. 한가지 예로 나는 <a href='https://ywtechit.tistory.com/404?category=950465'>이거 먹어봄?</a> 프로젝트의 후속조치로 `webpack`과 `babel`를 직접 설정하는 간단한 예시(<a href='https://github.com/YWTechIT/image-drag-and-drop'>image-drag-and-drop</a>)를 만들었으나, `babel`을 설정하기 위해 생각보다 많은 플러그인(`npm i -D @babel/core @babel/preset-env @babel/preset-react @babel/polyfill babel-loader`)이 필요했고, 이는 곧 빌드 시간을 늘어나게 하는 주범이었다. 하지만, `esbuild-loader`를 사용하면 빌드 시간을 대폭 단축시킬 수 있는데(<a href='https://github.com/privatenumber/esbuild-loader/discussions/138'>링크</a>) 이는 나에게 새로운 영감을 주었다. 내일부터 2차 팀 프로젝트를 하게 되는데 이때 `babel-loader` 대신 `esbuild-loader`을 사용하려고 한다. 마지막으로 상태관리 라이브러리 중 하나인 `Jotai`에 대해서도 배웠다. 2021년 11월 28일 기준으로 깃헙의 스타 수는 `redux`는 57.1k, `recoil`은 14.9k, `jotai`는 6.2k인데, 스타 수로만 봤을 때 `jotai`가 현저히 낮은데 왜 배우는지 처음에는 궁금했지만, 단순히 많은 사람들이 사용하기 때문에 사용해야 한다는 생각보다는 각 오픈소스 프로젝트가 어떻게 관리되고 있는지, 코어 개발자는 어떤 사람인지, 각 라이브러리의 장단점을 살펴서 선택해야한다는 강의 내용을 보고 꼭 스타수가 많은 라이브러리만 사용해야한다는 편견을 갖고있던 나의 오만함을 바로 잡을 수 있었다. 


### React에서 TS로 마이그레이션 하기
1. 타입스크립트 라이브러리 설치

```javascript
* 새로 CRA를 생성하는 경우: npx create-react-app <project name> -template typescript만 작성
* 기존 JS 파일을 TS로 마이그레이션 하는 경우 하단 과정 시작

npm i -D typescript esbuild-loader @types/react @types/react-dom
yarn add -D typescript esbuild-loader @types/react @types/react-dom

- typescript: tsc 컴파일러, ts 문법 지원을 위해 필요한 라이브러리
- @types/react: react 라이브러리를 위한 타입 패키지
- @types/react-dom: react에서 dom element와 관련된 타입들을 모아놓는 패키지
  * @types/라이브러리 이름: 타입스크립트에서 라이브러리 설치할 때 사용하는 명령어(Definitely Typed 참고)
- esbuild/loader: 타입스크립트 트랜스파일링을 위한 패키지(속도가 매우 빠르다)
  * 본래는 babel-loader를 사용했으나, 최근 들어 webpack의 빌드를 빨리하기 위해 esbuild를 많이 사용하는 추세다
```

2. tsconfig.json 설정

```javascript
1. tsconfig.json 파일 생성 
  * tsc --init 혹은 npx tsc --init 입력 시 tsconfig.json의 기본적인 컴파일러 옵션을 설정해준다.

{
  "compilerOptions": {
    "target": "es5",  // 트랜스파일링을 할 경우 어떤 버전으로 변환 할 것인지(IE 지원은 es5로 설정)
		"outDir": "./dist/",  // 컴파일 후 어떤 경로로 저장할지?
		"sourceMap": true,  // 디버깅을 위한 소스맵이 필요한 경우에 설정
    "module": "esnext",  // 모듈 코드를 ESM(ECMAScript Module: import, export), CJS(Common JS: require, exports.module) 모드로 설정할것인가?
    "jsx": "react-jsx"  // jsx파일을 js파일로 변환하도록 하는 설정, react 설정시 jsx파일이 js로 변환된다.
  }
}

jsx 옵션은 preserve, react, react-native 3가지 옵션을 설정할 수 있습니다.
1. preserve: 바벨이나 swc 같은 다른 트랜스파일러가 변환할 수 있도록 jsx 문법을 트랜스파일링하지 않고 그대로 둡니다. 따라서 트랜스파일링 결과는 .tsx에서 .jsx 파일이 됩니다.

2. react: jsx 문법을 js로 변환시킵니다. 트랜스파일링 결과는 .js 확장자 파일입니다.

3. react-native: preserve 모드처럼 jsx 문법을 그대로 두지만 트랜스파일링 결과는 .js 확장자 파일이 됩니다.
```

3. 사용하는 라이브러리들 중 @types 패키지 추가(타입 전환)

```javascript
1. npm i -D @types/<library name>: DefinitelyTyped 오픈소스에 등록된 타입 선언 파일 설치
2. git repo에 index.d.ts에 있는 라이브러리면 설치 안해도 됨. 
3. npm에서 @types/패키지명 검색해보고 있으면 @types/패키지 설치하고 @types/패키지가 없다면 직접 모듈에 대한 타입을 선언해야 한다.
4. 모듈에 타입을 직접 선언했다면 다른 개발자도 사용할 수 있게 라이브러리에 DefinitelyTyped에 PR을 날려보자
```

4. `webpack` 설정 변경

```javascript
module.exports = {
  entry: {  // 앱을 시작할 파일
    main: "./src/index.js",
  },
  output: {  // 웹팩 번들링 결과에 대한 옵션, 기본 경로는 dist
    path: path.resolve(__dirname, "dist"),
    filename: "[name].js",
  },
  resolve: {  // 번들링할 확장자 설정
    extensions: [".js", ".jsx", ".ts", ".tsx"],
  },
  module: {  // 번들링 할 때 플러그인 설정 가능
    rules: [
      {
        test: /\.(t|j)sx?$/,
        loader: "esbuild-loader",  // 타입스크립트 변환을 위한 로더
        options: {
          loader: "tsx", // Or 'ts' if you don't need tsx
          target: "es2015",
        },
      },
      {
        test: /\.css$/,  
        use: ["style-loader", "css-loader"],  // style-loader: style 태그를 삽입해 dom에 css 추가, css-loader: css 확장자의 css파일을 읽기 위한 로더, css 확장자를 가져와서 style 태그를 삽입해 DOM에 css를 추가한다.
      },
    ],
  },
  externals: {  // 번들링 결과에서 제외할 라이브러리들
    react: "React",
    "react-dom": "ReactDOM",
  },
};
```

5. `jsx` → `.tsx` 로 확장자 변환

```javascript
- jsx 파일에서 tsx파일로 확장자 변경을 하고 이 과장에서 생기는 타입 오류들을 해결해야 마이그레이션이 끝난다.
```
### ❏ 함수형 컴포넌트에 `props` 타입 설정하기
1. component props에 타입 설정

```tsx
// {...props}`: 스프레드 연산자로 props를 button의 props에 모두 전달
// `React.PropsWithChildren`: 사용자가 넘긴 props 타입(P)와 props.children을 인터섹션
// type PropsWithChildren<P> = P & { children?: ReactNode | undefined };
// `props.children`: react에서 기본적으로 전달해주는 children props. 자식 노드들이 전달됨

export const Button = (props: React.PropsWithChildren<ButtonProps>) => {
	return <button {...props} }>{props.children}}</button> // {...props}로 children을 한꺼번에 전달 할 수 있으나 type이 맞아야 함
};
```

2. `React.FC` 사용해 더 간단히 표현

```tsx
// React.FC: 내부적으로 PropsWithChildren을 사용
// React.FC 타입을 사용하면 내부적으로 PropsWithChildren을 사용하여 제네릭의 Props 타입과 children 타입을 인터섹션.
// props에 React.PropsWithChildren을 선언하는 것과 같은 효과

export const Button: React.FC<ButtonProps> = (props) => {
	return <button style={props.buttonStyle>{props.children}</button>;
}

type FC<P = {}> = FunctionComponent<P>;

interface FunctionComponent<P = {}> {
	(props: PropsWithChildren<P>, context?: any): ReactElement<any, any> | null;
}
```

### ❏ style props에 타입 적용하기
1. 기존 방법

```css
/* 
1. 모든 button에 적용 됨
2. class로 만들어도 `background-color`, `font-size`, `font-weight` 등 자주 변경되는 것들을 위해 여러 개의 `class` 를 조합해야 함(ex, `className = button bg-black size-16 weight-700`)
3. `props` 로 전달하면 어떨까? 
*/

button {
	padding: 20px;
	border-radius: 5px;
	background-color: black;
	color: red;
	font-size: 25px;
	font-weight: 700;
}
```

2. `React CSSProperties`

```tsx
/* 
1. button 태그의 style props 타입
2. createButtonStyle: 반환 타입을 React CSSProperties로 하는 style 객체 팩토리 함수 생성
3. '...styles'로 다른 style 속성도 받을 수 있게 추가
*/

const createButtonStyle = (
	styles?: React.CSSProperties): React.CSSProperties => ({
	padding: 50,
	borderRadius: 4,
	border: "none",
	...styles,  // 기존 속성을 override 할 수 있음
});

interface ButtonProps {
	styles?: React.CSSProperties;
}

export const Button: React.FC<ButtonProps> = (props) => {
  const buttonStyles = createButtonStyle(props.styles);
	return <button style={buttonStyles>{props.children}</button>;
}
```

### ❏ event props에 타입 적용하기
1. button을 클릭했을 때 handleClick으로 전달하고 싶음
2. `React.MouseEvent<Element, Event>`: `<button onClick={e => console.log(e)} />` 상태에서 `e` 에 마우스 호버
3. `e` 의 타입을 복사해서 `ButtonProps` 인터페이스의 `handleClick event` 타입으로 붙여넣거나, `form` 처럼 `e`가 보이지 않을 때는 `BaseSyntheticEvent` 를 사용한다.

```tsx
interface ButtonProps {
	styles?: React.CSSProperties;
	handleClick: (e: React.MouseEvent<HTMLButtonElement, MouseEvent) => void;
}

export const Button: React.FC<ButtonProps> = (props) => {
  const buttonStyles = createButtonStyle(props.styles);
	return <button style={buttonStyles} onClick={props.handleClick}>{props.children}</button>;
}
```

4. 결과코드

```tsx
// MainScreen.tsx
import { Button } from "../components/Button";
import { useNavigate } from "react-router-dom";

export const MainScreen = () => {
  const navigate = useNavigate();
  return (
    <>
      <h1>타입스크립트 능력 고사</h1>
      <p>나의 타입스크립트 실력은 어느 정도일까?</p>
      <a
        className="App-link"
        href="https://www.typescriptlang.org/ko/docs/handbook/react.html"
        target="_blank"
        rel="noopener noreferrer"
      >
        Learn Typescript + React
      </a>
      <Button styles={{ marginTop: 50 }} handleClick={() => console.log('button click')}>
        테스트 시작하기
      </Button>
    </>
  );
};

// Button.tsx
import React from "react";

// 3. styles를 매개변수로 받아 styles 객체를 반환하는 style 팩토리 함수를 정의해주세요
// createButtonSylte의 매개변수와 반환 타입을 적어주세요
// styles는 React에서 제공하는 style 타입입니다. 
export const createButtonStyle = (
  styles?: React.CSSProperties
) => ({
  padding: 20,
  borderRadius: 5,
  border: "none",
  cursor: "pointer",
  fontSize: 25,
  fontWeight: 700,
  backgroundColor: "#61dafb",
  color: "#fff",
  margin: 10,
  ...styles,
});

// 1. component에 props 적용을 하기 위해 ButtonProps 인터페이스를 선언해주세요
interface ButtonProps {
  // React에서 제공하는 styles 타입을 적어주세요
  styles?: React.CSSProperties;
  // event를 매개변수로 받고, void를 반환하는 함수 타입을 적어주세요
  // event 타입은 onClick={e => props.handleClick(e)}에서 e에 마우스를 올리면 확인할 수 있습니다
  handleClick: (event: React.MouseEvent) => void;
}

// 2. props가 ButtonProps와 children 속성을 함께 가질 수 있도록 타입을 선언해주세요
export const Button: React.FC<ButtonProps> = (props) => {
  // 4. createButtonStyle 함수를 호출하여 buttonStyles 객체를 생성하고 style props에 전달해주세요
  // 5. props의 handleClick을 onClick props에 전달해주세요
  const buttonStyles = createButtonStyle(props.styles);
  return (
    <button style={buttonStyles} onClick={props.handleClick}>
      {props.children}
    </button>
  );
};
```

### ❏ Hook에 타입 적용하기
1. `useState` 에 타입 적용하기

```tsx
function useState<S>(initialState: S | (() => S)) : [S, Dispatch<SetStateAction<S>>];
function useState<S = undefined>(): [S | undefined, Dispatch<SetStateAction<S | undefined>>];

const [name, setName] = useState(null)  // 초기값으로 state 타입을 결정
const [name, setName] = useState()  // 초기값이 없다면 undefined로 설정

// 초기값 설정 시 초깃값의 타입을 추론해서 state와 setState의 타입을 결정
// 초깃값과 다른 타입의 데이터를 setState의 인자로 넘길 경우 에러
// 이런 경우 useState의 제네릭 타입 설정: useState<string | null>(null)

import React, { useState } from "react";

export const TestScreen = () => {
	const [ name, setName ] = useState(null);

	const handleChange = (e: React.ChangeEvent<HTMLInputElement>) => {
		setName(e.target.value);  // 타입 에러
	}

	return(
		<div>
			<input onChange={handleChange} />
		</div>
	)
}
```

2. `useReducer` 에 타입 적용하기

```tsx
// 문제점
// 의도한 타입과 다른 타입의 데이터를 case로 추가해도 에러가 나지 않음(ex case "CHANGEVALUE":)
// state가 어떤 타입인지 알 수 없음
// action에 어떤 프로퍼티가 있는지 알 수 없음
// reducer의 제네릭 타입은 Reducer<any, any>를 확장하므로 타입을 지정하지 않으면 state와 dispatch도 any 타입이 됨

import React from "react";

const reducer = (state, action) => {
	switch(action.type) {
		case "INCREMENT" :
			return state + 1;
		case "DECREMENT" :
			return state - 1;
		default:
			return state;
	}
}

export const ScoreCounter = () => {
	const [ score, dispatch ] = React.useReducer(reducer, { score: 0 });
	return <div>{score}</div>
}

// 타입 적용하기
// 1. state와 action type 선언
// 2. Action type은 action을 구분할 type외에는 자유롭게 구성
// 3. score, dispatch가 각각 ScoreState, React Dispatch<ScoreAction>로 type 결정
// 문제점: action.type에서 increment, decrement 외에 다른 action.type이 오지 못하게 해야 함

import React from "react";

type ScoreState = {
	score: number;
}

type ScoreAction = {
	type: string;
	score: number;
}

const reducer = (state: ScoreState, action: ScoreAction) => {
	switch(action.type) {
		case "INCREMENT" :
			return { score: state.score + action.score };
		case "DECREMENT" :
			const result = state.score - action.score;
			return { score: result < 0 ? 0 : result };
		default:
			return state;
	}
}

export const ScoreCounter = () => {
	const [ score, dispatch ] = React.useReducer(reducer, { score: 0 });
	return <div>{score}</div>
}

// strict type 적용하기
// 1. ScoreAction의 type을 string union type으로 선언
// 2. reducer에서는 literal type guard로 타입마다 다른 로직 실행
// 문제점: RESET 액션의 경우 score를 따로 받지 않아도 됨, 그러나 Action 타입에 의해 점수를 넣어줘야 함

type ScoreAction = {
	type: "INCREMENT" | "DECREMENT" | "RESET";
	score: number;
}

const reducer = (state: ScoreState, action: ScoreAction): ScoreState => {
	switch(action.type) {
		case "INCREMENT":
			return { score: state.score + action.score };
		case "DECREMENT":
			const result = state.score - action.score;
			return { score: result < 0 ? 0 : result };
		case "RESET":
			return { score: 0 };
		default:
			return state;
	}
}

// 해결
// 1. ScoreAction의 score를 optional로 바꾸면 RESET 액션의 경우 score를 따로 받지 않아도 된다.
// 2. 하지만, reducer의 case문에서 action.score를 사용하는 쪽에서 경고를 뿜는다
// 3. 따라서, 구별된 유니온을 으용하여 type을 단서로 score 필드가 들어갈지 안 들어갈지 swtich문에서 type guard 하도록 만든다.

type CounterAction = {
	type: "INCREMENT" | "DECREMENT";
	score: number;
}

type ResetAction = {
	type: "RESET";
}

type ScoreAction = CounterAction | ResetAction;

const reducer = (state: ScoreState, action: ScoreAction): ScoreState => {
	switch(action.type) {
		case "INCREMENT":
			return { score: state.score + action.score };
		case "DECREMENT":
			const result = state.score - action.score;
			return { score: result < 0 ? 0 : result };
		case "RESET":
			return { score: 0 };
		default:
			return state;
	}
}

export const ScoreCounter = () => {
  const [score, dispatch] = React.useReducer(reducer, { score: 0 });
  return (
    <div>
      <h3>Score: {score}</h3>
      <Button handleClick={() => dispatch({ type: "INCREMENT", score: 10 })}>
        정답
      </Button>
      <Button handleClick={() => dispatch({ type: "DECREMENT", score: 10 })}>
        오답
      </Button>
      <Button handleClick={() => dispatch({ type: "RESET" })}>초기화</Button>
    </div>
  );
};
```

### ❏ Context API에 타입 적용하기
1. 타입 적용 전

```tsx
// ScoreContext.ts
import React from "react";

export const ScoreContext = React.createContext({
	score: 0,
	dispatch: () => {}  // 에러 유발
})

// App.tsx
...
const [ counter, dispatch ] = React.useReducer(reducer, { score: 0 });
<ScoreContext.Provider value={{ score: counter.score, dispatch }}  // 타입 에러(구체적인 액션이 사용되어야 함)
```

2. 타입 적용 후

```tsx
// 1. createContext는 초깃값에 대한 타입을 제네릭으로 받는다
// 2. Context의 value에 대한 타입을 선언한 뒤 제네릭의 타입 파라미터에 넣어주면 된다.

import React from "react";
import { ScoreAction } from "../reducers/ScoreCounterReducer";

interface ScoreContextValue {
	score: number;
	dispatch: Dispatch<ScoreAction>;
}

export const ScoreContext = React.createContext<ScoreContextValue>({
	score: 0,
	dispatch: () => {}  // 에러 유발
})
```

### ❏ 타입스크립트와 리액트 상태 관리: Redux
1. `npm i redux @reduxjs/toolkit react-redux @types/react-redux`

```tsx
1. react, typescript와 함께 쓰기 위한 redux 라이브러리들을 설치
2. @reduxjs/toolkit은 RootState와 Dispatch 타입을 추출하는데 사용
3. react-redux의 경우 타입 선언 파일이 없어 @types 패키지를 따로 설치 해야 함
```

2. `redux toolkit`

```tsx
// configureStore: redux의 createStore를 사용성 높게 한 번 더 추상화한 것
// redux의 combineReducers를 쓰는 것보다 RootState, AppDispatch, AppThunk 등 타입 추론이 더 쉬워짐

// Reducers/store.ts
import { configureStore, ThunkAction, Action } from "@reduxjs/toolkit";

export const store = configureStore({
	reducer: { scoreCount },
})

export type AppDispatch = typeof store.dispatch;
export type RootState = ReturnType<typeof store.getState>;  // RootState라고 하는 이유는 configureStore에서 모든 리듀서를 한곳에서 관리하기 때문에 rootState라고 표현한다.
export type AppThunk<ReturnType = void> = ThunkAction<
	ReturnType,
	RootState,
	unknown,
	Action<string>,
>;

// selector: reducer의 state 추출(rootState에서 원하는 state를 추출)
// dispatch: reducer의 dispatch 추출
// useAppDispatch, useAppSelector: app의 모든 dispatch, selector 값을 사용할 수 있게 하는 hook
// TypedUseSelectorHook: 특정 State에 대한 타이핑이 된 useSelector를 생성할 수 있음
import { TypedUseSelectorHook, useDispatch, useSelector } from "react-redux";
import type { RootState, AppDispatch } from "./store";

export const useAppDispatch = () => useDispatch<AppDispatch>();
export const useAppSelector: TypedUseSelectorHook<RootState> = useSelector;

// redux store 적용을 위한 provider 사용
import { Provider } from "react-redux";
import { store } from "./reducers/store";

ReactDOM.render(
	<React.StrictMode>
		<Provider store={store}>
			<App />
		</Provider>
	</React.StrictMode>
)

// useAppSelector: TypedUseSelectorHook덕분에 RootState에서 자동 완성을 통해 특정 reducer에 대한 state 추출 가능
// useAppDispatch: 전역에서 관리되는 dispatch 사용
// dispatch({ type: "scoreCounter/RESET" }): 다른 reducer와 함께 쓰이기 때문에 reducer의 이름을 앞에 붙여서 구분해주는 것이 관습.

import { useNavigate } from "react-router-dom";
import { Button} from "../../componennts/Button";
import { useAppSelector, useAppDispatch } from "../../reducers";

export const ResultScreen = () => {
	const score = useAppSelector((state) => state.scoreCounter.score);
	const dispatch = useAppDispatch();
	const navigate = useNavigate();
	const handleReset = () => {
		dispatch({ type: "scoreCounter/RESET" })  // 다른 reducer와 사용했을 때 type이 겹쳐 action이 혼용되는 것을 방지하기 위해 prefix를 붙입니다. 타입을 강제하는 것은 아님. RESET이라고만 써도 타입 에러는 나지 않습니다.
		navigate("/");
	};

	return(
		<div>
			...
		</div>
	)
}
```

### ❏ 타입스크립트와 리액트 상태 관리: Jotai
1. `redux`: 자바스크립트 앱에서 사용 가능하고, 리액트 생태계에서 가장 많이 쓰이는 상태 관리 라이브러리
2. `recoil`: 리액트 팀에서 만든 상태 관리 라이브러리
3. `Jotai`: `recoil` 의 `atomic model` 기반의 상향식 접근에 영감을 받아 만든 상태 관리 라이브러리

![](https://images.velog.io/images/abcd8637/post/b42b3cbe-6090-454a-a966-4308afcb818e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-24%2013.48.40.png)

### ❏ Jotai에 사용되는 개념
1. `Atom`: 상태를 나타내는 단위, `recoil` 과 달리 `atom` 을 생성할 때 사용되는 문자열 `key` 가 필요 없다.
2. `config`: `atom`을 생성할 때 넣어주는 초깃값
3. `Provider`: `Atom` 이 쓰이는 범위(scope)를 나눌 때 사용
4. atom, hook 생성

```tsx
import { atom } from "jotai";

export const scoreAtom = atom(0);  // scoreAtom은 state처럼 사용됨
```

5. `useAtom` 을 사용한 `custom hook`

```tsx
// useAtom을 사용해 useState처럼 사용 가능
// setScore를 consumer(state를 가져다 쓰는 쪽)에서 타입에 따라 setScore로 매번 같은 코드를 반복해야 함
// 따라서, custom hook을 만들어서 dispatcher처럼 사용
// custom hook에서 use<hook이름>은 hook 네이밍 컨벤션이므로 따라야 함

export function useScoreHook(){
	const [score, setScore] = useAtom(scoreAtom);
	const dispatch = (action: ButtonAction): void => {
		switch (action.type) {
			case "INCREMENT" :
				return setScore(score + action.score)
			case "DECREMENT" :
				const newScore = score - action.score;
				return setScore(newScore < 0 ? 0 : newScore);
			case "RESET" :
				return setScore(0);
			default:
				return setScore(score);		
		}
	};
	return { score, dispatch };
}
```

6. `useScoreHook` 사용

```tsx
// screens/ResultScreen 
// 생성한 custom hook을 import해서 사용

export const ResultScreen: React.FC<ResultScreenProps> = () => {
	const navigate = useNavigate();
	const { score, dispatch } = useScoreHook();
	const handleReset = () => {
		dispatch({ type: "RESET" });
		navigate("/");
	}
	
	return (
		<div>
			...
		</div>
	)
}
```

---
## 📍 66일차 1.25.화.(14주차 2차 팀 프로젝트)
오늘부터 엘리스 교육이 끝나는 2월 20일까지는 2차 팀 프로젝트 기간이다. 작년 크리스마스에 1차 팀 프로젝트를 끝냈는데, 벌써 2차 프로젝트라니.. 시간이 참 빠른것 같다. 아마도 나의 기억력이 좋다면 지금까지 배운내용들을 기억했겠지만, 그렇지 못하기에 지금까지 남겨놓은 약 66개의 기록들을 보며 떠올려야겠다. 이번엔 팀원이 아니라 팀장으로서 프로젝트를 진행하는데, 마음가짐을 다르게 가져야겠다고 생각했다. 또한 저번 프로젝트의 후속조치로 `webpack`을 공부했는데, `React`를 이용해 개발할 때 `CRA`가 아닌 직접 `webpack`을 이용해서 프로젝트를 구현해야겠다고 마음먹었다. 그리고 또 한가지 변수가 생겼는데, 바로 백엔드를 맡게 되었다. 처음부터 백엔드를 맡겠다고 한것은 아니었고, 원래는 프론트로 역할을 배정받았지만, 팀 미팅 때 팀원 모두 백엔드를 자주 다뤄보신분이 없다고 하셔서 내가 백엔드를 다루겠다고 얘기했다. 지금까지 항상 프론트만 다뤄와서 백엔드는 할 줄 모르는 내가 잘 할 수 있을지는 나조차도 의문이다. 누군가는 뭐하러 아무도 선택안하는 포지션을 하려고 비웃겠지만, 내가 안하면 누군가는 해야되는 분야고 하기 싫은 사람이 억지로 하는것보다는 차라리 하고 싶은 사람이 하는게 낫다는 생각이 들었다. 항상 개인 프로젝트를 하며 백을 다루기 싫어 라이브러리에 의지했다면 이번엔 직접 부딪혀보고싶다는 생각도 들었다. 왜 그랬는지 다시 생각하면 헛웃음만 나오지만 이미 엎질러진 물이기에.. 한번 도전해볼까 한다. 사용 스택은 `express + MondoDB`인데, 이전에 들었던 엘리스 강의에서 추가로 알아야겠다고 마음먹고 알라딘에서 <a href='https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=269942241'>관련 서적(한 권으로 끝내는 Node & Express)</a>을 구매했다. (생각보다 `express` 관련한 서적이 없었다.) 이제 무모한 나의 결정을 3주동안 기록해나가보자..

### ❏ 개발자의 역량
1. `소통역량`: 다른 개발자의 의견을 경청하고, 의견의 의도와 핵심을 이해한 후, 자신의 관점을 명확하고 논리 정연하게 설명하는 것입니다. 자신과는 다른 의견, 새로운 관점을 환영하고 더 나은 방향일 경우 겸허하게 받아들입니다. (말보다는 코드로 소통하라)
2. `시간, 태스크 관리 능력`: 특정 태스크를 위해 소요될 시간을 정확하게 파악할 수 있고, 이를 바탕으로 다른 개발자와 소통하여 일정 관리를 합니다. 사전에 정한 일정은 반드시 지키며, 지키기 어려운 경우 미리 소통하여 서프라이즈를 줄입니다. (특정 부분을 부각시키고 다른 부분을 포기한다든지..)
3. `논리력`: 사용하는 기술 스택과 코드의 작성 방식에는 논리가 필요하다. (주어진 목표를 더 효과적으로 달성하기 위한 개발 방향이어야 한다.), 왜 이 기술 스택을 선택했는지? 왜 이런 코드를 구성했는지를 논리적으로 설명할 수 있어야 한다.
4. `학습능력`: 특정 언어, 특정 프레임워크에서 벗어나더라도 개발할 수 있는 능력을 갖추어야합니다. 기본기와 문제 해결 능력을 갖추면, 언어와 프레임워크가 바뀌더라도 바로 대응할 수 있습니다. 개발 과정에서 추가적으로 기술 스택, 언어가 생긴 경우, 짧은 시간 내에 스스로 배울 수 있어야 합니다.

### ❏ 좋은 코드란?
1. 가독성: 코드를 읽으면서 쉽게 이해할 수 있고, 의도를 이해하기 위해 고민하지 않아도 되는 코드
2. 일관성: 사전에 정한 일관된 규칙을 따라야 합니다.

### ❏ GitLab 활용법(Git Flow)
1. `README.md`: 프로젝트를 관리하는 목적, 필요한 정보들만 작성하기
2. `Issue`: 프로젝트 진행 시, 어떠한 상황, 문제 또는 계획을 개발 할 예정이라는 것을 알려주는 이정표 해야 할 일을 이슈로 정리하자
3. `MR`

```
- Matser Branch(Main branch): 서비스로 출시될 수 있는 브랜치, 배포 가능한 생태의 코드를 관리
- Sprint Branch: 모든 기능이 추가되고 버그가 수정되어 배포 가능한 상태라면 MR
- Feature Branch: 새로운 기능 개발 및 수정하는 브랜치, 작업이 끝난 기능은 Sprint로 MR!
```

---
## 📍 67일차 1.26.수 프로젝트 2일차 TL;DR
오늘부터 2차 프로젝트가 끝나는 날까지 글을 길게 쓰지 않고 그날 배운내용이나 느꼈던 점들을 나열하겠다.

1. `configuration`: `secretKey`와 같은 값들은 소스코드에 포함하지 않고, `local`에서 보관한다. 이때, `dotenv`를 이용하면 쉽게 `config` 파일을 작성할 수 있다.
2. `express` 에러처리: 동기적으로는 마지막 `use`로 넘어가지만 비동기적인 처리시에는 콜백함수 내에서 에러처리를 해야한다.
3. `express.json()`: REST API, body parser
4. `express.urlencoded({ extended: false })`: HTML Form -> Body parser
5. `cors`

```javascript
app.use(
    cors({
        origin: ["http://127.0.0.1:5500"],
        optionsSuccessStatus: 200,
        credentials: true, // Access-Control-Allow-Credentials: true
    })
);
```

6. `morgan`: 요청시 어떤 요청을 받았는지, 얼마나 걸렸는지 log를 남겨주는 라이브러리
7. `helmet`: 보안에 필요한 헤더를 추가해준다.

```
/* helmet settings
	X-Content-Type-Options: nosniff
	X-DNS-Prefetch-Control: off
	X-Download-Options: noopen
	X-Frame-Options: SAMEORIGIN
	X-Permitted-Cross-Domain-Policies: none
	X-XSS-Protection: 0 
*/
```

---
## 📍 68일차 1.27.목 프로젝트 3일차 TL;DR
### ❏ JWT 토큰 인증 흐름
<a href='https://www.youtube.com/watch?v=p09YODnkSO8&list=PLanIiKDTgXLy4cZc5Ahfi_x443ZVKXb_5&index=12'>DFSW Labs Youtube 강의</a>

1. once user verified the email, password thry're going to get back a token using JWT
2. once they get that token they can send that along to access a protected route with passport, passport-jwt
3. JWT module creates the token passport will actully validate. it also extract the users information from it
4. we need to add login functionally, we need to accept a user's email
5. validate that email that it exists and validate the password 
6. JWT.sign include user info, because when that token gets sent to the server
7. we want decode it and it needs to know what user it is
8. we also need to send a secretOrKey & expiration if we want it to expire in a certain amount of time(expiration: no more than a week, permanently)
9. put it header as an authrization and send it to the server, the server will validate the user, it'll get ther user information and use it within our express server
10. once we have successful match. it gives a token and token includes user info
11. passport.Strategy, passport.ExtractJwt(extract payload which is userdata)
12. fromAuthHeaderAsBearerToken: bear string before token
13. once we call payload, find that user and validate it jwt-payload includes the user staff
14. token 확인 후 : then we tried to access a protected route we first did it without the token. you saw it was authorized then we added correct token and now responding with the user data

---
## 📍 69일차 1.28.금. 프로젝트 4일차 TL;DR
1. 백엔드 인증 로직: GitHub login -> GitHub 정보 획득 -> JWT 토큰 생성 -> 쿠키로 client 전달 -> 로그인 필요한 서비스에서 JWT 검증(검증은 req.user있는지 확인)
2. React CRA 설정을 override 하고 싶으면 React-app-rewired
3. redux처럼 API를 중앙에서 관리하고 싶다면 react-query 사용
4. rebase의 장. 단점: merge commit 이 없어져 history 가 깔끔해짐, 반대로 history 가 없어져 commit 이력이 남지 않아 confilct 가 나기 쉽다. `Git`의 숙련도에 따라 `rebase` 도입 여부를 고민하기
5. browser에서 mobile device 확인하는 방법: device-width, user-agent
6. 모바일에 사용성을 맞췄기 때문에 반응형 웹 디자인에서 모바일, 태블릿까지만 대응하기
7. redux는 state를 중앙에서 관리할 수 있다는 장점이 있으나, boilerplate의 작성이 오래걸린다. 프로젝트의 기간이 길지 않기 때문에 페이지별로 상태를 관리하는 방법을 사용하자.
8. 전통적인 flow는 back에서 api를 내려주는 방법을 사용했으나, 최근에는 back으로 한정짓지 않고 front에서도 api를 호출하여 사용한다.
9. `branch`에 `feature-TODO`만들고, issue에도 TODO 남기기 (cross-check)
10. React-query를 도입하여 API를 중앙에서 관리하는 식으로 구현하면 데스크탑 버전에서도 문제가 없을 것으로 보입니다. API.js에 API를 모아두고, 호출하는 부분에서 React-query를 이용하면 원활할 것입니다.
11. 검색 기능을 구현할 때, 서버에 보낼건지 프론트에서 처리할건지에 따라 나뉩니다. 랭크 정보는 백엔드에서 처리하면 되고, mongoDB 쿼리를 날리는 순간에 순위를 sorting 하면 됩니다.
12. Router -> mobile에서 PC화면으로 갈 때 고민해보셔야 할 것 같습니다. (ex: rank 페이지에서 화면을 확장하여 PC버전이 되었을 때는 /rank의 의미가 없어지기 때문)
13. 차트 -> 물론 직접 공부하면서 구현하면 좋겠지만, 시간적 비용을 줄이기 위해 우선은 라이브러리를 이용하여 작성하고 추후에 시간적 여유가 있을 때 직접 구현해보면 좋을 것 같습니다.

---
## 📍 70일차 1.29.토. 프로젝트 5일차 TL;DR
1. `firebase`로 간단하게 작은 사이즈의 프로토타입을 만들 때 빠르고 쉽게 사용할 수 있는 좋은 스택이지만, 현업에서는 `MERN` 스택도 사용하는 곳이 많다. 공부하는 입장에서 `MERN` 스택을 사용한다면 백과 프론트의 전반적인 흐름도 알 수 있고, `web framework`를 사용하게 될 상황도 많고, 확장성측에서도 `MERN` 사용하는 것을 추천한다.
2. 회원 인증, 권한 구현 할 때 `cookie`를 사용하면 미들웨어에 무조건 `cookie-parser`를 설치하자.. 이것때문에 2시간 고생함..
3. 프론트에서 `API`를 가져다 사용할 경우. 만약에 `API`가 에러가 나서 정상적인 `data`를 가져오지 못할 때는 어떻게 처리할 것인가? 404페이지로 이동 시킬수도 있지만 백에 미리 저장되어있는 `db`에서 값을 내려줘도 된다.
4. `Backend`에서 `API`를 가공한 다음에 처리하자. 화면에서 가공해야 하는 데이터들이 사용하는 `API`들만으로 가능하지 않은 경우가 있을 수 있어서 필요한 `API` 내용들을 받아주고, 가공해서 `Frontend`로 내려주는 것이 좋을 것 같다.
5. API처리 로직: 클라이언트 -> 서버(커밋 수 요청) -> 서버에서 API요청 -> 받아온 정보로 DB 갱신 -> 클라이언트에게 응답
6. 인증 / 권한 페이지 로직

```
1. 권한: `client`에 `JWT` 토큰 값을 `cookie`에 담아 `server`로 보냄. -> 토큰이 만료되었거나 일치하지 않으면 `status(401)`리턴
2. 인증: `GitHub OAuth` -> `db`에서 해당 `id`와 일치하는 `id`를 찾고 없으면 새로 만들어서 저장 -> `cookie`로 `JWT`토큰 값 `browser`로 전송
```

7. 서버는 프론트에서 요청한 결과가 올바른지 아닌지를 결과값으로만 내려준다. 그리고 프론트에서 결과값을 토대로 다음 로직을 구성한다.
8. 프론트에 `json`형태로 값을 내려줄거면 `res.send` 대신 `res.status(200).json({ isOk: true, postId });`와 같은 형태로 내려주자. `res.status(200).json`은 `json` 형태로 내려준다는 의미가 포함되어있으나, `res.send`는 의미가 불명확하다. 또한, `res.send`로 전송하게되면 불필요한 함수를 한번 더 호출하게 된다. 참고(<a href='https://haeguri.github.io/2018/12/30/compare-response-json-send-func/'>harguri.github.io</a>)

---
## 📍 방학 2. 3. 목
1. 백엔드의 폴더 구조는 보통 어떤식으로 구성하는지 유투브에`MERN` 스택을 사용한 영상을 많이 찾아보고 나름의 폴더 구조를 만들었다. 지난번 프로젝트에서 백엔드를 담당하신 세영님께서 작성하신 폴더구조가 많은 도움이 되었다.(감사합니다.)

```
├── config
│   ├── db.js
│   └── keys.js
├── middleware
│   └── error-handler.js
├── model
│   ├── index.js
│   └── schema
│       └── User.js
├── package-lock.json
├── package.json
├── passport
│   ├── index.js
│   └── strategy
│       └── GitHub.js
├── routes
│   ├── api
│   │   └── auth.js
│   └── index.js
├── server.js
└── utils
    ├── cookie-extractor.js
    └── create-token.js
```

---
## 📍 71일차 2.8.화. 프로젝트 6일차 TL;DR
1. mongoDB connect 주소는 localhost 대신 MongoDB Compass URI 사용하기 (mongodb+srv://<account>:<password>@<URI>.mongodb.net/<dbName>)
2. Database Access탭에서 접근 계정을 생성할 수 있다.
3. dotenv 파일에서 key=value에서 value에 ""를 붙이지 않아도 된다.
4. Promise.all 사용시 중간에 reject가 나게되면 실행을 중지한다. 그러나, Promise.allSettled를 사용하면 중간에 reject가 나도 멈추지 않는다. settled는 fulfilled, rejected 상태를 의미함.
5. GitHub API rest로 total commit을 구할 때 get요청 당 per_page가 100개가 limit이므로 100개가 넘을 때는 `@octokit/plugin-paginate-rest`의 paginateRest를 사용하자.
6. 외부 API를 사용하는 로직은 lib/api 폴더 안에 넣어두자
7. passport.authenticate('jwt', { session: false })에서 next()가 되지 않고 Unautorized가 나오면 jwt의 expiredIn 값을 제대로 적용했는지 살펴보자 (3600 => 1h)
8. `jest` 실행 시 `svg` 관련 오류가 난다면 `jest-svg-transformer` 라이브러리를 살펴보자

---
## 📍 72일차 2.9.수. 프로젝트 7일차 TL;DR
1. React에서 webpack과 함께 사용시 svg를 사용할 때 ["@svgr/webpack"]를 사용한다면 file-loader에는 svg를 제거해주자 
2. webpack alias로 jest test가 정상적으로 작동하지 않으면 "@/(.*)": "<rootDir>/src/$1"를 추가하자
3. mongoDB의 timestamps를 카멜케이스로 작성하면 작동하지 않는다.(timeStamps(x)) 주의하자
4. mongoDB에서 _v(이 키 값에는 문서의 내부 개정이 포함됩니다)를 없애려면 versionKey: false로 설정하자.
6. DB에 accessToken값을 그대로 저장하기보다는 암호화작업 혹은 yml, aws-secret-manager로 관리하자
7. API가 중복되더라도 Rest하고 그 양이 적다면 중복으로 보지 않아도 된다.
8. commit/today에서 한꺼번에 모으지 말고 계층화시키자. commit/today/detail, commit/today/repo-name, commit/today/list처럼
9. issue는 commit으로 포함시키는가? 도메인간의 포함관계를 따져 rest하게 작성하자.
10. 필요한 데이터만 추려서 db에 넣고 가공하자
11. 우리 서버에서 전송하는 api가 아니고 제 3의 api를 이용한다면 external-api와 같은 작명을 생각하자
12. service는 api를 호출해서 나온 결과를 가공해서 나온 결과를 db에 저장하는 용도, contoller는 client로 내려주는 용도(ex. res.json)
13. router가 controller의 기능을 가져갈 수도 있다.
14. router는 API path를 만들어준다.
15. /api의 존재여부가 restful의 차이를 만들기보다는 보통은 우리 서비스의 api를 호출할 때 사용한다.

---
## 📍 73일차 2.10.목. 프로젝트 8일차 TL;DR
1. populate는 mongoDB에서 _id를 통해 다른 컬렉션에 있는 데이터를 참조할 수 있다.
2. new User({}).save()와 User.create({})는 동일하다.
3. findById(id)는 findOne({_id: id})와 같다.
4. query 요청을 줄이기 위해 find() -> 수정 -> save()보다 where()를 활용하자.
5. upsert(): 존재하지 않는 문서의 경우 새로 생성하여 저장한다.
6. mongoDB에서 dataBase는 여러 collection을 담는 하나의 저장소, collection: 여러개의 document를 담는 공간, document: 여러개의 key-value로 이루어진 하나의 페이지, key-value: 이름 - 값

---
## 📍 74일차 2.11.금. 프로젝트 9일차 TL;DR
1. 함수 파라미터로 새로운 객체 key를 설정할 때는 다음과 같이 작성하자.

```javascript
const FindByKey = (key) => {
  const config = {};
  config[key] = value;
}
```

2. webpack에서 favicon 관련 설정은 `HtmlWebpackPlugin`의 option으로 설정할 수 있지만 manifest를 고려한다면 `FaviconsWebpackPlugin`으로 설정해주자.
3. GitLab에는 Default branch를 설정하여 MR요청을 보낼 때 target설정을 하지 않으면 default branch로 경로를 설정할 수 있다.
4. GitLab에는 Protected branches 설정이있어 함부로 해당 branch에 바로 commit하지 못하게 설정할 수도 있다.(force도 사용불가, MR로만 merge 가능)
5. eslint 설정시 `eslint-plugin-prettier` 패키지와 `eslint-config-prettier` 패키지가 정상적으로 설치되었는지 확인하자.
6. eslint 설정시 `test` 파일은 `eslint-plugin-jest` 패키지로 문법 검사하자.
7. DB에 저장하는 timestamp를 KST로 맞추지말고 UTC로 통일하자. 나중에 마이그레이션 혹은 서비스 복제시 불 필요한 행위를 방지한다.
8. GitHub API에서 응답시간을 고려해서 응답시간을 초과하면 DB에 있는 값을 내려주기
9. 매 요청마다 API를 주지말고 일정시간 이내 동일한 요청이오면 DB에 있는 값을 내려주어 불 필요한 API 요청을 막는다.
10. 객관적인 기준이 아니라 주관적인 기준을 시험해보고 싶다면 한번 시도해보고 장단점을 비교해서 나만의 기준을 세워놓자.
11. 현재 팀의 상황을 고려해서 브랜치 전략을 어떻게 구성할지 생각해보자 
12. 커밋 단위도 팀원들끼리 고려해서 적용하자.
13. GitHub API GET 요청시 time을 UTC로 변경해서 요청하는지는 doc를 참고하자
14. GitHub API에서는 timestamps 기능을 요청할 때만 사용할 수 있고, 값을 돌려받는 요청에서는 사용할 수 없다. (Note that these rules apply only to data passed to the API, not to data returned by the API. As mentioned in "Schema," timestamps returned by the API are in UTC time, ISO 8601 format.) <a href='https://docs.github.com/en/enterprise-server@3.0/rest/overview/resources-in-the-rest-api'>GitHub DOC</a>
15. mongoDB에서 UTC를 KST로 변경하는 방법
16. UTC에서 KST로 바꿀 때 Date.prototype.toLocaleTimeString()를 사용하면 간편하게 바꿀 수 있다.
17. JS 기본 Date는 UTC로 변환되기 때문에 UTC로 요청을 받는 GitHub API는 추가적으로 시간을 변환해줄 필요가 없다.

```javascript
const config = {
  timestamps: { currentTime: () => Math.floor(Date.now() + UTC_TO_KST) },
  versionKey: false,
};

const UTC_SEOUL_OFFSET = 9;
const MILLISECOND_TO_SECOND = 1000;
const MINUTES_TO_SECOND = 60;
const HOUR_TO_MINUTES = 60;
const UTC_TO_KST =
  UTC_SEOUL_OFFSET *
  HOUR_TO_MINUTES *
  MINUTES_TO_SECOND *
  MILLISECOND_TO_SECOND;
```

---
## 📍 75일차 2.12.토. 프로젝트 10일차 TL;DR
1. MR시 confilct가 난다면 새로운 branch를 하나 파서 내가 올리려는 branch를 git pull origin <내 브랜치>하고 다시 MR요청하자.
2. MR을 팀장만 보는것이 아니라 해당 팀원들과 같이 보면서 개선하고 싶은점, 느낌점등을 간단하게 코멘트로 남겨주고 merge하는 방법도 있다.
3. postman에서 POST요청을 보낼 때 cookie를 사용한다면 cookie 탭에 값을 추가하자. 이때 도메인은 host네임만 작성해도 된다.
4. 캘린더형식의 data에서 각각 일수를 더하는 로직

```javascript
const data = [
  [
    [0, 0, 1, 5],
    [2, 7, 1, 4],
  ],
  [
    [0, 0, 1, 5],
    [2, 7, 1, 4],
  ],
];

const answer = data[0].map((month, monthIndex) =>
  month.map((day, dayIndex) =>
    data.reduce(
      (prev, current, repoIndex) =>
        prev + data[repoIndex][monthIndex][dayIndex],
      0,
    ),
  ),
);

console.log(answer)
👉🏽 [ [ 0, 0, 2, 10 ], [ 4, 14, 2, 8 ] ]
```

5. 현재 달을 기준으로 며칠까지 있는지 리턴하는 함수작성(윤년포함)

```javascript
const checkLeapYear = (year) =>
  (year % 4 === 0 && year % 100 !== 0) || year % 400 === 0;

const getFebruary = () => {
  const isLeapYear = checkLeapYear(year);

  return isLeapYear
    ? Array.from({ length: 29 }, () => 0)
    : Array.from({ length: 28 }, () => 0);
};

export const getMonthCalendar = (month) => {
  const thirtyOneDaysMonth = ["01", "03", "05", "07", "08", "10", "12"];
  const february = "02";
  const monthReg = new RegExp(month);

  if (month === february) {
    return getFebruary(year);
  }

  if (monthReg.test(thirtyOneDaysMonth)) {
    return Array.from({ length: 31 }, () => 0);
  }

  return Array.from({ length: 30 }, () => 0);
};

console.log(getMonthCalendar("02"));
👉🏽 [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ]
```
---
## 📍 2.14.월. TL;DR
1. Suspense는 자식 컴포넌트의 비동기 작업이 처리되기 전에 fallback props가 렌더링 된다. 즉, 비동기 작업이 끝날 때까지 loading 컴포넌트를 보여주는 코드를 넣을 수 있다.
2. bcrypt에서 sync보다 async를 권장하는 이유: 간단한 script에서는 sync모드를 사용하는것이 좋으나, 서버에서 bcrypt를 사용하는 경우 비동기모드를 사용하는것이 좋다. bcrypt에 의해 수행된 해싱은 CPU를 많이 사용하므로 동기화는 이벤트 루프를 차단하기때문에 다른 이벤트를 처리하지 못한다. 비동기는 메인 이벤트 루프를 차단하지 않는 스레드 풀을 사용한다.
3. GitHub로 로그인하면 Backend에서 cookie에 담아서 Frontend로 보낸다.
4. Frontend에서 JWT토큰을 Header에 넣어서 req요청을 보내면 Backend에서 해당 jwt를 해석한다. 혹은 cookie에 담아서 보낸다.
5. jest test시 `expect(...).toBeA is not a function` 오류가 난다면 expect에 괄호가 제대로 작성되어있는지 살펴보자.
// correct expect(getApi()).toBe(answer);
// Incorrect expect(getApi().toBe(answer));
6. jest test시 `regeneratorRuntime is not defined`가 뜬다면 `npm i -D regenerator-runtime`를 설치하고 `import 'regenerator-runtime'`로 불러오자.

---
## 📍 76일차 2.15.화. 프로젝트 11일차 TL;DR
1. branch 전략

```javascript
  - Git-Flow: 단순하다, CI/CD가 자연스럽다, master(최종), 체계적인 분류 없이 master에 의존한다.
  - GitHub-flow: 상세한 리뷰와 토의, master(최종), develop(개발), release(QA 및 베타 테스트), hotfix(master에서 버그수정)
```

2. 우리팀은 GitHubFlow를 기반으로 하되 GitFlow의 방법을 조금 섞었다. commit convention을 정했고, MR올리면 해당 분야 팀원들이 코드리뷰 후 의견을 남긴다. emoji를 모두 남겼으면 팀장이 최종적으로 merge한다. merge가 완료된 branch는 삭제한다. commit의 개수를 모두 남기는것보다 squash 전략으로 여러개의 커밋을 하나로 뭉친다. (이와 비슷한 rebase 전략은 제일 마지막 commit만 사용한다. log가 깔끔해지는 장점이 있지만 반면에 기록이 남지 않으므로 git 숙련도가 낮으면 추천하지 않는다.) 급하게 수정하는 사항은 hotfix 브랜치를 사용했고, Back과 Front 연결은 release 0.0.x 버전의 브랜치를 만들어서 QA테스트를 진행한다. 
3. react에서 proxy를 사용할 때 CRA 대신 webpack을 사용한다면 webpack.config.js에서 devServer안에 다음과 같은 코드를 추가한다. 이렇게 작성하면 프론트에서 백으로 API요청을 할 때 host + port를 생략해도 target으로 요청이 넘어간다.

```javascript
proxy: {
      "/api": {
        target: "http://localhost:8888",
	},
}
```

4. 이왕 서버 배포해보는 김에 `Azure`, `Nginx`, `CI/CD` 도 공부해보자.
5. 서버에서 `GET,`, `POST` 와 같은 요청을 테스트하는 라이브러리는 `supertest`를 이용했다. 유닛 테스트는 `jest`
6. `jest coverage` 는 테스트 현황을 표로 한 눈에 볼 수 있다.

---
## 📍 77일차 2.16.수. 프로젝트 12일차 TL;DR
오늘은 내 생일이다. 어릴때의 생일은 특별한 날로 생각했지만 요즘은 특별한 날이 아니라는 생각이 든다. 프로젝트 마감이 4일이 채 남지 않았기 때문에 신경쓰지않고 작업중이다.

1. 동점자를 고려한 순위 매기기

```javascript
const calcRankWithConcurrentScore = (userData) => {
  const userRank = [...userData];

  userRank.sort((a, b) => {
    if (a.score === b.score) {
      if (a.username < b.username) return -1;
      if (a.username > b.username) return 1;
    }
    return b.score - a.score;
  });

  let rank = 1;
  let currentScore = 0;
  const result = userRank.map((user) => {
    const { score } = user;
    if (score >= currentScore) {
      const newUser = {
        ...user,
        rank,
      };
      currentScore = score;
      return newUser;
    }

    rank += 1;
    currentScore = score;
    return { ...user, rank };
  });

  return result;
};

userRank: [
  {
    username: "Jin1won",
    avatarUrl: "https://avatars.githubusercontent.com/u/54543013?v=4",
    score: 100,
    rank: 1,
  },
  {
    username: "YWTechIT",
    avatarUrl: "https://avatars.githubusercontent.com/u/54543013?v=4",
    score: 100,
    rank: 1,
  },
  {
    username: "cafeLatte",
    avatarUrl: "https://avatars.githubusercontent.com/u/54543013?v=4",
    score: 70,
    rank: 2,
  },
  {
    username: "coffee",
    avatarUrl: "https://avatars.githubusercontent.com/u/54543013?v=4",
    score: 50,
    rank: 3,
  },
  {
    username: "h1jun",
    avatarUrl: "https://avatars.githubusercontent.com/u/54543013?v=4",
    score: 50,
    rank: 3,
  },
  {
    username: "alice",
    avatarUrl: "https://avatars.githubusercontent.com/u/54543013?v=4",
    score: 30,
    rank: 4,
  },
  {
    username: "soo054141",
    avatarUrl: "https://avatars.githubusercontent.com/u/54543013?v=4",
    score: 30,
    rank: 4,
  },
];
```

2. develop에 최신 코드를 다른 브랜치로 내려받을 때는 git checkout develop 후 git merge <target-branch>를 해주면 된다.
3. routes에서 동일한 URI로 GET, POST요청을 보내는 코드는 다음처럼 한 줄로 줄일 수 있다.

```javascript
// before
router.get("/today/goal", getGoalController);
rotuer.post("/today/goal", postGoalController);

// after
router.route("/today/goal").get(getGoalController).post(postGoalController);
```

4. `nvm(node version manager)`: curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.36.0/install.sh | bash
5. `source ~/.bashrc` 파일로 이동 
6. `nvm install 14.18.1`: 원하는 노드 버전 설치 
7. `nvm ls`: 설치한 노드 목록 보기
8. `node -v` : 현재 노드버전 보기
9. 터미널 재부팅 후에도 노드 버전이 제대로 적용되어있는지 살펴보기
10. 백엔드 개선할 점: 써드파티 API를 이용하는 로직은 처음에 모두 긁어온다음 DB에 저장하고, 일정 시간마다 갱신했으면 더 좋을 것 같다.
11. `Nginx` 이용시 `proxy_pass` 값 설정하기 `도메인` -> `nginx` -> `server.js`
12. `release` 브랜치는 수정하지 않고 `develop` 브랜치의 수정사항을 가져오기만 한다. 만약, `release` 브랜치의 `history`를 관리하고 싶다면 `tag`를 남기거나 삭제하지 않거나..
13. 무겁지 않은 로직은 테스트코드로 남겨두기

---
## 📍 78일차 2.17.목. 프로젝트 13일차 TL;DR
1. cors credentials: HTTP Cookie와 HTTP Authentication 정보를 인식할 수 있게 해주는 요청이다. 클라이언트에서 서버로 요청을 보낸다면 `axios.defaults.withCredentials = true;`를 꼭!!!@#!@#!@#!@ 설정해주자.

```javascript
export const AXIOS = axios.create({
  baseURL: serverURL,
  withCredentials: true,
  axiosConfig,
});

app.use(
  cors({
    origin: "http://localhost:1111",
    credentials: true,
  }),
);
```

2. /bin/www 파일은 익스프레스의 설정 파일을 가져와 http와 연결하는 작업 (nginx를 붙인다면 이 파일과 연결하면 된다.)

---
## 📍 79일차 2.18.금. 프로젝트 14일차 TL;DR
1. webpack 사용시 public에 접근하려면 devServer.static에는 다음과 같이 작성하면 `localhost:port/assets/public`로 접속이 가능하다.

```javascript
static: {
      directory: path.resolve(__dirname, "public"),
      publicPath: "/assets", /
}
```

2. public에서 manifest.json의 경로는 다음과 같이 작성한다. `<link rel="manifest" crossorigin="use-credentials" href="/assets/manifest.json">`
3. GitLab에서 tag는 브랜치가 아니라 commit을 관리한다.
4. 응답을 JSON Parse를 사용할 때는 요청도 String으로 변환하고 보내야 한다.(데이터 타입이 배열이면 `[${badges}]` 처럼 보내기)
5. nginx를 사용하면 클라이언트에서 서버 URI의 자원을 볼 수 없다.(정해진API로 요청하면 리버스 프록싱을 통해 서버가 응답하는 주소로 바꿔주기 때문)

---
## 📍 80일차 2.20.토. 프로젝트 15일차 TL;DR
1. 클라이언트에서 요청할때는 가동서버(localhost)로 요청하는것이 아니라 배포하는 도메인으로 요청해야한다.(이후에 nginx에서 reverse proxy 처리함)
2. env의 callback URI는 도메인까지 포함해서 작성하자.
3. Git clone 버튼으로 눌러서 받는것은 최신의 브랜치를 받는것이다. 특정 브랜치를 받고 싶으면 다음 주소를 입력하자 `git clone -b <branchName> --single-branch <git clone URL>`