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

```javascript
const Button = styled.button`
	background: ${({ clicked }) => ( clicked ? "orangered" : "red" )};
	color: ${({ clicked }) => ( clicked ? "blue" : "orange" )};
	padding: 12px 40px;
	border: none;
`

const List = styled.ul`
	display: flex;
	flex-direction: column;
`

const ListItem = styled.li`
	padding: 20px 100px;
	background: orange;
	color: white;

	& + & {
		margin-top: 8px;
	}
`
```

---
## 📍 53일차 1.6.목. 실시간 강의
오늘은 `CORS`, `React-router-dom`에 대해서 배웠다. 실습강의 중 `React-router-dom`를 사용하지 않고 `useState`를 이용해 라우팅하는것처럼 구현하는 시간이 있었는데, 이해가 잘 안됐다. 그런데, `React-router-dom` 라이브러리를 사용하면서 코드를 줄여나가니까 이것들이 왜 사용되었는지 그리고 해당 라이브러리가 중요성에 대해 알게되었다. 결론: `React-router-dom` 최고.

1. `JS immutability`: 해당 라이브러리 사용시 객체 자료형은 값이 바뀌지 않는다.(얕은복사 후 객체 `value`을 변경하게 되면 원본 객체까지 변경되나, 해당 라이브러리를 사용하면 원본 객체의 값은 그대로 유지할 수 있다.), <a href='https://opentutorials.org/module/4075'>생활코딩님 강의영상 참고</a>
2. 구글 `element`에서 `className`에 `notranslate` 속성을 추가하면 한글 번역시 해당 `element`는 번역되지 않는다.
3. `bookmarklet`: 북마크에 `javascript:`로 시작하는 간단한 스크립트를 입력한다.
4. `React-Router-Dom`: `react`에서 `router` 기능을 사용하기 위한 라이브러리 최신버전은 `v6`이고, 자주 사용한 라이브러리는 `v5`이다. 변경된 명령어가 많으니 <a href='https://reactrouter.com/docs/en/v6'>공식문서</a>를 한번 읽어볼 것! 대표적으로 `useHistory`가 `useNavigate`로 바뀌었다.
5. `browserRouter`: `HTML5`의 `historyAPI`를 활용하여 `UI`를 업데이트 함
6. 네이버 검색 `API` 사용시 `CORS` 관련에러가 나오는데, 네이버에서는 `API` 요청을 브라우저에서 하지 말고 서버프로그래밍(python, jsp, php, node.js 등...)을 통해서 호출하도록 되어있다. 다른 클라이언트의 `id` 혹은 `secret`으로 `api` 호출하는것을 막기 위해서다. (<a href='https://developers.naver.com/forum/posts/26989'>네이버 개발자 포럼</a>) 로컬환경에 프록시를 설정하거나, 프록시 서버를 이용하는 방법이 있는데 이번에는 <a href='https://cors-anywhere.herokuapp.com/corsdemo'>`cors-anywhere`</a>사이트를 이용했다. `heroku`를 이용했는데, 내 계정으로 하나 만들고 싶다.

```javascript
useEffect(() => {
    axios
        .get(URL, {
            params: {
                query: "치킨",
            },
            headers: {
                "X-Naver-Client-Id": API_ID,
                "X-Naver-Client-Secret": API_PW,
            },
        })
        .then((res) => {
            setResult(res.status);
        });
});

// has been blocked by CORS policy: Response to preflight request doesn't pass access control check: No 'Access-Control-Allow-Origin' header is present on the requested resource.
```

7. `CORS(Cross-origin Resource Sharing)`: 교차 출처 리소스 공유, 다른 도메인의 자원에 접근할 수 있도록 권한을 부여하도록 브라우저에 알려주는 것, 서버의 도메인이 자신의 도메인과 다를 때 실행한다.

```
1. 브라우저는 SOP 정책을 준수한다. 같은 출처에서만 리소스에 접근할 수 있다.
  * a.com <-> a.com but, 다른 사이트와 접근할 수 있는데 이때는 CORS를 준수하면서 사용해야한다.
  * CORS 정책은 서버가 아니라 브라우저가 결정한다.
  * Access-Control-Allow-Origin: 허용된 페이지
  * 네이버는 API를 브라우저끼리 통신하는것을 권장하지 않고 서버(제 3서버: proxy server)에서 뿌려주는것을 선호한다.

2. script는 보안정책이 적용되지 않는 점을 이용한 JSONP를 사용한다.
3. 프록시를 이용해 서버 접근을 우회할 수 있다
4. 특정 도메인의 CORS를 허용한다. 자신이 만든 서버가 아니면 적용하기 어렵다.
```

* 교차출처 리소스 공유(CORS) - <a href='https://developer.mozilla.org/ko/docs/Web/HTTP/CORS'>MDN</a>
* 동일 출처 정책(SOP) - <a href='https://developer.mozilla.org/ko/docs/Web/Security/Same-origin_policy'>MDN</a>

---
## 📍 54일차 1.7.금. 온라인 강의
오늘은 `SPA`, `MPA`, `React-router-dom` 속성에 대해서 배웠다. 이후에 `useReducer`를 사용해 문제를 푸는데 `useReducer`를 사용해본적이 많지 않아 난이도가 조금 어렵게 느껴졌다.

### ❏ SPA(Single Page Application)
1. 하나의 페이지 요청으로 전체 웹앱을 사용하는 방식
2. 유저는 웹페이지를 사용하며 모바일 앱 같은 경험을 느낌(새로고침없이 화면전환이 된다.)
3. `html` 코드를 읽다가 `script` 태그를 만나면 다시 서버에 요청하고 서버에서 다시 브라우저로 넘겨준다. 브라우저에서 `JS` 코드를 파싱한 다음 `app.js` 가 렌더링된다.
4. `CSR` 기술을 활용하여, 페이지 진입 시 리로드없이 라우팅한다.
5. `AJAX` 기술을 활용, 페이지 이동 시 서버에 데이터만 요청하여 `JS` 로 페이지를 만듦 (`fetch` 등..)
6. `MPA` 와 다르게 여러 페이지를 하나의 앱의 구성요소로 보고 여러 페이지 간의 스타일, 컴포넌트를 재활용하는 방향으로 구현한다.
7. `JS` 만으로 전체 페이지를 만들기 때문에, 첫 요청 시 빈 페이지를 받게 된다.

```
장점
 - 서버에서 페이지를 만들 필요가 없으므로 CDN에 캐싱이 가능하다. 
  * CDN:콘텐츠 전송 네트워크(contents network delivery), 서버가 각 최종 사용자들에게 가장 가까운 서버를 기반으로 데이터 요청을 수행한다.
  * 더 빠른 서비스 제공 가능(HTML, CSS, JS 등...)
 - 매번 페이지 요청을 할 필요가 없어 네트워크 요청이 줄어듦(서버 입장), 마찬가지로, 데이터 요청 등을 캐싱하여 재사용하는 등 제약 조건이 줄어듦
 - 웹 사이트를 개별 페이지보다는 하나의 앱으로 보는 설계로 고도의 S/W 설계와 패턴을 적용할 수 있음

단점
 - MPA 방식보다는 SEO에 불리함
 - 하나의 JS 앱이 지속하므로, 메모리 관리, 성능, 데이터 활용 등이 중요하다.
 - 모든 페이지를 한번에 로드해야 하므로 코드가 많아질수록 로드 속도가 느려진다.
```

### ❏ MPA(Multi Page Application)
1. 서버에 미리 여러 페이지를 두고 유저가 네비게이션 요청 시 요청에 적합한 페이지를 전달한다.
2. 미리 서버에서 전체 페이지를 빌드해 브라우저로 전송된다.
3. 서버에 라우팅을 처리하는 기능이 있고, 서버에서 여러 페이지를 관리한다.
4. 페이지 요청마다 모든 리소스를 다시 받아오므로, 페이지 간 데이터를 재활용하기 힘듦
5. `res.send(page)` 를 받으면 `build` 된 페이지를 브라우저로 전달해준다.
6. MPA는 서버에서 build하기 때문에 CDN처리를 할 수 없다.

### ❏ SPA에서 라우팅이 중요한이유
1. 주로 `History API` 혹은 `URL Hash` (www.naver.com#a, #b, #c ,,,)를 이용해 페이지 리로드 없는 페이지 전환을 구현한다.
2. `history`, `location` 등 `HTML5 API` 를 활용한다.
3. `visibilitychange`, `popstate`, `beforeunload` 등 `window event` 를 활용하여 페이지 전환 등의 이벤트 시 핸들러 등록
4. `react-router`, `reach-router` 등의 라이브러리를 활용하면, 라우팅 관련 기능을 쉽게 사용할 수 있음.

### ❏ react-router
1. `declarative`: 서술문의(`<Link to=”/login”>` - JSX), `imperative`: 반드시 해야하는(`handleClick = () ⇒ push(’/login’)` - history API)
2. `Declarative routing for React`
3. React의 `JSX` 를 이용하거나, `History API` 를 사용하여 라우팅을 구현한다.
4. 웹에서는 `react-router-dom` 을 사용한다.(`react-router-native` 도 있음)
5. 적용시, 서버의 모든 `path` 에서 같은 앱을 서빙하도록 해야 한다.
6. `React` 컴포넌트를 특정 `path` 와 연결하면, 해당하는 `path` 로 진입 시 컴포넌트를 렌더링하게 한다.
7. `query`, `path variable` 등 `URL parameter` 를 얻어 활용한다.
8. 조건에 맞지 않을 경우 `redirect` 함 `<Redirect to ="/register" />`
9.  페이지 이동 시, 이벤트 핸들러를 등록함 `history.listen(cb)`
10. `/posts/my-post-1` 등의 `nested route` 를 구현한다.
11. `BrowserRouter` 로 감싸 `Router Context` 를 제공해야 한다.
12. `Route` 로 `path` 를 정의하고, 그 안에 렌더링하고자 하는 컴포넌트를 ㅓㄴㅎ음
13. `Link` 로 특정 페이지 이동 시, 리로드 없이 페이지가 이동함
14. `Switch` 로 매칭되는 라우트 하나를 렌더링하게 한다. (`exact` 혹은 `switch` 를 쓰지 않으면 모두 렌더링시킨다.)

```javascript
// 라우터는 동기적으로 확인한다.
<BrowserRouter>
	<Switch>
		<Route path="/about"><AboutPage></Route>
		<Route path="/contact"><ContactPage></Route>
		<Route path="/"><HomePage></Route>
	</Switch>
</BrowserRouter>
```

15. `NavLink` 의 특징은 매칭되는 `path` 가 자기 자신인 경우 강조처리해준다.

### ❏ BrowserRouter
1. 브라우저환경에서 라우팅 기능을 사용할 수 있는 컴포넌트
2. `HTML5` 의 `HistoryAPI` 를 사용하여, `UI` 와 `URL` 의 싱크를 맞추는 역할을 담당한다.
3. 모든 `URL` 에 대해 동작하게 하기 위해서는 서버 설정 필요
4. 모든 `path` 앞의 `basename` 을 지정할 수 있다. (`basename=”/ko”`)
5. `forceRefresh` 로 페이지 이동 시 리프레시할 것인지 지정할 수 있다.

### ❏ Switch
1. 여러 `Route` 중 매치되는 `Route` 위에서부터 하나를 선택하여 렌더링한다.
2. 매칭되는 `Route` 가 없으면 아무것도 보여주지 않음. `callback` 용으로 `404 Not Found Page` 를 추가함
3. `path="/"` 의 경우 모든 `path` 에 매칭되므로 `exact` 키워드를 추가하거나 가장 아래로 내린다.

### ❏ Route
1. `path` 와 컴포넌트를 매칭함
2. 매칭되는 컴포넌트는 `children` 으로 넣어주거나 `component prop` 으로 넘김
3. `exact` 키워드로 정확하게 매칭하는 `path` 를 설정함
4. `Route` 로 렌더링 되는 최상위 컴포넌트는 `match`, `location`, `history` 를 `prop` 으로 받음
5. `render prop` 으로 매칭되었을 때, 실제 어떤 컴포넌트를 렌더링할지 통제함

### ❏ Redirect
1. `Link` 와 비슷하나, 렌더링되면 `to prop` 으로 지정한 `path` 로 이동함
2. `Switch` 안에서 쓰일 경우 `from ,to` 를 받아 이동하게 만듬(from =”/” to=”/login”)

```javascript
// 선언방식(선호)
if (!users) return <Redirect to="/abc" />
return <div>userPage</div>

// 명령방식
if(!users) history.push("/abc")
return <div>userPage</div>
```

### ❏ Link, NavLink
1. `to prop` 을 특정 `URL` 로 받아 클릭 시 네비게이션 함
2. `anchor tag` 를 래핑함(a tag)
3. `NavLink` 의 경우, 매칭 시 어떤 스타일을 가질 지 등의 추가 기능이 있음 `<NavLink to ="/users"></>`
4. `to` 에 `location object` 나 함수를 받을 수 있다. (`hash`, `pathname`, `state` 객체 등...)

### ❏ useHistory, useLocation, useParams, useRouteMatch
1. 원래는 최상위 컴포넌트에서만 접근 가능했으나, `hook` 을 사용함으로써 `react-router` 관련 객체에 접근할 수 있다.
2. `history`, `location`, `params`, `match` 객체에 접근함

### ❏ react-router 응용
1. `private Route`: 특정 조건이 충족되지 않았을 때 다른 페이지로 `Redirect` 하도록 하는 기능, 유저의 상세페이지, 개인정보 변경 페이지 등을 만들 때 사용됨.

```javascript
// declarative(선언적) 방법
function PrivateRoute({ component: Component, ...props }){
	return <Route {...props} render={props => {
		const isLoggedIn = !!getUserInfo()
		if(!isLoggedIn){
			return <Redirect to="/login" />
		}
		return <Component {...props} />
	}}
}

// imperative(명령적) 방법
function usePrivateRoute(validateFunc){
	const history = useHistory();
	
	useEffectt(() => {
		if (!validateFunc()){
			history.push("/login")
		}
	}, [])
}

usePrivateRoute(getUserInfo);
```

---
## 📍 55일차 1.8.토. 온라인 강의
오늘은 `JS 비동기`, `동기`, `API 요청`, `callback`, `promise`, `async - await`, `OpenAPI`, `CORS` 에 대해서 배웠다. 이전에 한번 배운내용이었고, 오늘 다시 복습한다는 마인드로 공부하니까 이해가 잘됐다.

### ❏ 자바스크립트 비동기
1. 초기 웹 환경에서는 서버에서 모든 데이터를 로드하여 페이지를 빌드했으므로 JS에는 별도의 비동기 처리가 필요하지 않음
2. Ajax 기술의 등장으로 페이지 로드 없이 `client-side` 에서 서버로 요청을 보내 데이터를 처리할 수 있게 됨
3. `XMLHttpRequest` 객체를 이용해 서버로 요청을 보낼 수 있게 됨
4. `JS` 는 `single-thread` 이므로, 서버 요청을 기다려야 한다면 유저는 멈춰있는 브라우저를 보게 된다. 따라서 동기가 아닌 비동기 처리를 이용해 서버로 통신해야 한다.
5. 비동기 요청 후, `main thread` 는 유저의 입력을 받거나, 페이지를 그리는 등의 작업을 처리
6. 비동기 응답을 받으면, 응답을 처리하는 `callback` 함수를 `task queue` 에 넣음 (동기적인 처리는 call stack) 
7. `event loop` 는 `main thread` 에 여유가 있을 때 `task queue` 에서 함수를 꺼내 실행한다.
8. 브라우저에서 실행되는 `JS` 코드는 `event driven` 시스템으로 작동한다.
9. 웹앱을 로드하면 브라우저는 `HTML document` 를 읽어 문서에 있는 `CSS code`. `JS code`  를 불러옴
10. `JS` 엔진(`V8`, `blink`)은 코드를 읽어 실행
11. 서버에서 바이트 스트링을보내면 브라우저에서 해당 스트링을 파싱하여 DOM tree 구조로 만든다. `css`, `js` 코드를 서버에 요청한 다음 바이트 스트림을 넘겨 받으면 다시 읽어서 `code` 를 만들어낸다. 이후에 `JS` 엔진이 해당 코드를 실행한다.
12. 브라우저의 `main thread` 는 `JS` 코드에서 동기적인 코드외에도 웹 페이지를 실시간으로 렌더링하고, 유저의 입력을 감지하고, 네트워크 통신을 처리하는 등 수많은 일을 처리한다.
13. 비동기 작업을 할당하면 비동기 처리가 끝나고 브라우저는 `task queue` 에 실행 코드를 넣는다.
14. `main thread` 는 `event loop` 를 돌려 `task queue` 에 작업이 있는지 확인하고,  동기적인 작업이 끝나면 `call stack` 으로 이동시킨 후 `task` 를 실행한다.

```javascript
// async
request("user-data", (userData) => {
	console.log("userData 코드");
	saveUsers(userData)
}

consoel.log("DOM 변경")
consoel.log("유저 입력")
```

### ❏ Promise
1. 비동기 처리 후 실행될 코드를 `CB` 로 보내는 것
2. 비동기 처리가 고도화 되면서, `CB hell` 등이 단점으로 부각 됨
3. `Promise` 를 활용하여 비동기 처리의 순서 조작, 에러 핸들링, 여러 비동기 요청 처리 등을 쉽게 처리할 수 있게 됨

```javascript
// callback pattern
setTimeout(() => {
	console.log("Done");		
}, 1000)

// callback pattern - single request
function fetchUsers(onSuccess){
	return request('/users').then(onSuccess)
}

// Error handle 1
function fetchUsers(onSuccess, onError){
	return request('/users')
						.then(onSuccess)
						.catch(onError)
}

// Error handle 2
return request('/users').then(onSuccess, onError)

// callback pattern - multiple request
function fetchUserAddress(onSuccess){
		return request('/users', (userData) => {
			const userDataWithAddress = [];
			const userLength = userData.lenth;

			userData.map(user => request(`/users/${user.userId}/address`, (address) => {
				userDataWithAddress.push({ ...user, address })
				if(userDataWithAddress.length === userLegnth){
					onSuccess(userDataWithAddress)
				}
			})
		})
}

// promise pattern - multiple request
function fetchUserAddress(){
	return request("/users").then((userData) => 
		Promise.all(
			userData.map((user) => 
				request(`/users/${user.userId}/address`).then((address) => ({
					...user,
					address
				})
			)
		)
	);
}
```

4. `Promise` 객체는, 객체가 생성 당시 알려지지 않은 데이터에 대한 `Proxy` 
5. 비동기 실행이 완료된 이후 `then`, `catch`, `finally` 등의 핸들러를 붙여 각각 데이터 처리 로직, 에러 처리로직, 클린업 로직을 실행한다.
6. `then` 체인을 붙여 비동기 실행을 마치 동기 실행처럼 동작하도록 한다.

```javascript
function returnPromise(){
	return new Promise((resolve, reject) => {
		setTimeout(() => {
			const randomNumber = generateRandomNumber(100);
			if (randomNumber < 50) resolve(randomNumber)
			else reject(new Error("Random number is too big."))
		}, 1000)
	})
}

// 비동기 코드를 동기스럽게 작성 할 수 있다.
returnPromise()
		.then(num => {
			console.log("first random number:", num)
		})
		.catch(error => {
			console.error("Error occured", error)
		})
		.finally(() => {
			console.log("Promise returned")			
		})
```

7. `Promise` 객체는 `pending`, `fulfilled`, `rejected` 상태를 가짐
8. `fulfilled`, `rejected` 두 상태를 `settled` 라고 지칭
9.  `pending` 은 비동기 실행이 끝나기를 기다리는 상태 이후 `promise` 핸들러를 붙여 조작가능
10. `fulfilled` 는 비동기 실행이 성공한 상태
11. `rejected` 는 비동기 실행이 실패한 상태
12. `then`, `catch` 는 비동기, 동기 실행 중 어떤 것이라도 리턴할 수 있음
13. `promise.all()` 은 모든 프로미스가 `fulfilled` 되길 기다림, 하나라도 에러 발생시 모든 프로미스 요청이 중단됨
14. `promise.allSettled()` 는 모든 프로미스가 `settled` 되길 기다림
15. `Promise.race()`는 넘겨진 프로미스들 중 하나라도 `settled` 되길 기다림
16. `Promise.any()` 는 넘겨진 프로미스들 중 하나라도 `fulfilled` 되길 기다림

```javascript
// Promise.all
Promise.all(
	users.map((user) => request('/users/detail', user.name))
)
 .then(console.log)
 .catch(e => console.error("하나라도 실패했습니다."))

// Promise.allSettled
function saveLogRetry(logs, retryNum){
	if(retryNum >= 3) return;  // no more try

	Promise.allSettled(logs.map(saveLog))
		.then((results) => {
			return results.filter((result) => result.status === "rejected");
		})
		.then((failedPromises) => {
			saveLogRetry(
				failedPromises.map((promise) => promise.reason.failedLog),
				retryNum + 1
			);
		});
}

// Promise.race
function requestWithTimeout(request, timeout = 1000){
	return Promise.race([request, wait(timeout)].then((data) => {
		console.log("요청 성공");
		return data;
	}))
}

function wait(timeout){
	return new Promise((resolve, reject) => {
		setTimeout(() => {
			reject()
		}, timeout)
	})
}

requestWithTimeout(req)
	.then(data => console.log("data: ", data)
	.catch(() => console.log("타임아웃 에러!"))

// Promise.any
function getAnyData(dataList){
	Promise.any(dataList.map((data) => request(data.url)))
		.then((data) => {
			console.log("가장 첫 번째로 가져온 데이터 : ", data)
		})
		.catch((e) => {
			console.log("아무것도 가져오지 못했습니다.")
		});
}
```
17. `promise chaining` : `Promise` 객체는 `settled` 되더라도 계속 핸들러를 붙일 수 있다. 핸들러를 붙인 순서대로 호출된다. `catch` 뒤에 핸들러가 연속해서 붙어있다면, 에러를 처리한 후에 계속 진행된다. 이때는 `catch` 에서 리턴 값이 있다면 `then` 으로 전달된다.

### ❏ async / await
1. `Promise` 체인을 구축하지 않고 `Promise` 를 직관적으로 사용할 수 있는 문법
2. `try - catch` 문으로 에러를 직관적으로 처리
3. `async function` 을 만들고, `Promise` 를 기다려야 하는 표현 앞에 `await` 를 붙인다.
4. `then` 을 많이 붙이다보면 직관적이지 못할 수 있다.

```javascript
// async/await
async function fetchUsers(){
	try{
		const users = await request('/users')  // resolve data, then()
		console.log("users fetched")
		return users
	}catch(e){  // catch()
		console.log("error: ", e);
	}
} 

// Promise
function fetchUsers(){
	return request('./users)
		.then(users => console.log("users fetched"))
		.catch(console.log("error: ", e));
}
```

5. 여러 개의 await 을 순서대로 나열하여 `then` `chain` 을 구현할 수 있음

```javascript
async function fetchUserAddress(id){
	try{
		const user = await request('/user/)
		if(!user) throw new Error("No user found")  // 조건 만족시 catch절로 이동
	  const address = await request(`/user/${user.id}/address`);  // 위에서 작성한 user의 결과를 인자로 사용함
		return { ...user, address }
	}catch(e){  // promise의 모든 에러를 catch 할 수 있다.
		console.log(e)
	}
}
```

### ❏ async / await - Promise 조합
1. `Promise.all` 은 특정 비동기 작업이 상대적으로 빨리 끝나도, 느린 처리를 끝까지 기다려야 하는데 이와 달리 `async/await` 를 사용할 경우 `parallelism` 을 구현할 수 있다. 즉, 빨리 끝난 대로 먼저 처리가 가능하다

```javascript
async function fetchUserAddress(id){
	return await Promise.all([
		(async () => await request(`/users/${id}`))(),
		(async () => await request(`/users/${id}/address`))(),
	]);
}

fetchUserAddress("1234")
	.then(([user, address]) => ({...user, address}))
	.catch(e => console.log(e))
```

### ❏ POSTMAN, OpenAPI, CORS
1. 서버와의 통신을 위해 `API` 를 활용하는 경우, `React` 앱으로만 요청하는 것은 비효율적이다.
2. `POSTMAN`: `API` 를 테스트하기 위한 개발 도구

### ❏ OpenAPI
1. `RESTful API` 를 하나의 문서로 정의하기 위한 문서 표준
2. `OpenAPI Specification(OAS)` 로 정의됨
3. `Swagger` 등의 툴로, `Open API` 로 작성된 문서를 파싱해 테스팅 도구로 만들 수 있음
4. `FE`, `BE` 협업 시 중요한 도구로 사용
5. `API` 의 `method`, `endpoint` 를 정의한다.
6. `endpoint` 마다 인증 방식, `content type` , `body data`, `query string`, `path variable`등 정의

### ❏ CORS
1. 브라우저는 모든 요청 시 `Origin` 헤더를 포함
2. 서버는 `Origin` 헤더를 보고, 해당 요청이 원하는 도메인에서 출발한 것인지를 판단
3. 다른 `Origin` 에서 온 요청은 서버에서 기본적으로 거부함.
4. 본격적인 요청을 보내기 전에 `options` 에 `preflight` 를 통해 미리 서버에 요청을 보내본다. ( 서버 `option` 에서 처리 할 수 없다는 `CORS` 를 보내면 네트워크 요청을 실패하도록 한다.
5. 서버의 `endpoint` 와 홈페이지의 `domain` 은 다른 경우가 많다. 따라서, 서버에서는 홈페이지 `domain` 을 이용하여 다른 `domain` 이라 하더라도 요청을 보낼 수 있게 한다.
6. 서버는 `Accss-control-allow-origin` 외에 `Access-control-*` 을 포함하는 헤더에 `CORS` 관련 정보를 클라이언트로 보냄
7. 브라우저의 `same-origin-policy` 정책을 준수하기 위해 생겨난 개념
8. 웹사이트에 악성 `script` 가 로드되어, 수상한 요청을 하는것을 막기 위함
9. 반대로 익명 유저로부터의 `DDos` 공격 등을 막기 위함(여러가지 도메인을 만들어 특정 서버에 무차별적으로 요청을 보낸다. 그것을 브라우저가 1차적으로 방어해준다)
10. 서버에 직접 `CORS` 요청을 할 수 없다면, `Proxy` 서버 등을 만들어 해결한다.(`proxy server`: 클라이언트가 요청을 보낼 때 `CORS` 요청을 허용해준다. 요청을 보낼 때 `proxy` 서버는 `target.server` 에 요청을 보내고  `target.server` 는 `proxy` 에 요청정보를 응답한다. (`proxy` 서버는 브라우저가 아니므로 `SOP`, `CORS` 을 사용하지 않는다.) 그리고 `proxy` 서버는 `CORS` 설정을 허용했기 때문에 다시 요청받은 브라우저로 `target Server` 에서 받은 내용을 뿌려준다.

---
## 📍 56일차 1.11.화. 실시간 강의
오늘은 `React`에서 난이도가 어렵다고 느끼는 `Redux`에 대해서 배웠다. 이전까지 만들었던 프로젝트들은 규모가 작아 `Redux`를 사용해야 할 필요성을 느끼지 못했고, 어떤 예제로 `Redux`를 공부해야하나라고 생각하는 중에 커리큘럼에 `Redux`가 포함되어있어 깊게는 아니어도 발을 얕게나마 담글 수 있음게 감사함을 느꼈다. 

### ❏ Redux
1. `Redux`는 `React`에 사용하려고 만들어졌지만, 실제로 다른 UI 라이브러리 혹은 프레임워크와 함께 사용할 수도 있다.(`angular-redux`, `ember-redux` 등)
2. `Redux` 는 앱의 복잡성을 획기적으로 낮추어 예측가능하게 만들어주는 환상적인 도구이다.
3. 하나의 상태(객체)를 유지하여 앱의 복잡성을 낮춘다. 외부로부터 차단시켜 데이터를 함부로 수정하는것을 차단시킨다. 데이터의 접근은 인가된 함수(`redux` , `dispatch`)에서만 상태를 변경한다. 상태를 사용할 때도 함수를 이용해서만 접근한다.
4. 의도치 않게 `state` 값이 변경되는것을 막는다.
5. `store` 에 들어있는 `state`는 직접 접근할 수 없다. `getState()` 를 통해서 접근해야한다.

```javascript
// dispatcher는 state 값 변경하기
// getState는 state의 값 전체를 가져오기
// subscribe는 state가 바뀔 때 새로운 상태를 갱신해주기
// render는 state를 그려주기

function reducer(oldState, action){}

const store = Redux.createStore(reducer)

function render(){  // React의 return문 과 같음
	const store = store.getState();  // store에 있는 값 가져오기
	document.querySelector("#app").innerHTML = `<h1>WEB</h1>`
}

store.subscribe(render);  // state의 값이 바뀔 때마다 render 된다.
```

6. `render` 는 `UI` 를 만들어주는 개발자가 짜야하는 코드(`reducer` 도 마찬가지)

![](https://images.velog.io/images/abcd8637/post/ad69cbce-1970-469a-97e3-c3ad3e08dd91/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-11%2011.32.33.png)

7. 각각의 상태가 강하게 의존되어있다면?? `redux` 를 사용하지 않았을때는 상태 하나가 변경되었을 때 나머지 상태에도 적용시켜줘야한다. `redux` 를 사용하면 강하게 연결된 상태를 하나로 관리할 수 있다. 상태관리의 편의성 증가 곧, 코드의 가독성 증가
8. `redux cdn code`: `https://cdnjs.cloudflare.com/ajax/libs/redux/5.0.0-alpha.0/redux.min.js` 끝부분에 `min` 이 붙여져 있으면 코드를 한 줄로 표현한다.(`minimize`의 줄임말)
9. `dispatch` 에 값을 전달할 때 `type` 을 꼭 붙이자. (`store.dispatch({type: 'CHANGE_COLOR', color: 'red'})`)
10. `redux` 에서 값을 변경할 때는 `immutable` 한 상태로 변경하자.(객체를 복사 하고나서 수정하기, 객체의 구조가 복잡해지거나 배열도 함께 다루는 경우 `immer` 라이브러리를 사용하면 좀 더 쉽게 리듀서를 작성할 수 있다. 리덕스의 상태는 최대한 깊지 않은 구조로 진행하는 것이 좋다.)
11. 리덕스에서 불변성을 유지해야 하는 이유는 내부적으로 데이터가 변경되는 것을 감지하기 위해 얕은 비교(`shallow equality`) 검사를 하기 때문이다. 객체의 변화를 감지할 때 객체의 깊숙한 안쪽까지 비교하는 것이 아니라, 겉핥기 식으로 비교하여 좋은 성능을 유지할 수 있는 것이다.
12. `state` 가 바뀔때 자동으로 `render` 함수를 실행해주는 방법: `subscribe` 사용하기.
13. `redux` 를 사용하면 `decoupling` 이 쉽다.
14. 상태관리란? 한곳에서 상태를 관리하여 다른 컴포넌트끼리 상태 의존성을 줄인다.
15. `store`: 한 개의 프로젝트에서는 단 하나의 스토어만 가질 수 있다.
16. `reducer`: 변화를 일으키는 함수. 액션을 만들어서 발생시키면 리듀서가 현재 상태와 전달받은 액션 객체를 파라미터로 받아 온다.

```
Redux를 사용해야 할까요?
1. 계속해서 바뀌는 상당한 양의 데이터가 있다.
2. 상태를 위한 단 하나의 근원이 필요하다.
3. 최상위 컴포넌트가 모든 상태를 가지고 있는 것은 더 이상 적절하지 않다.
```

14. `props drilling`: 사용하지 않는 `props`를 전달 목적으로 계속 사용하는 것. 불 필요한 전달을 피하기 위해서 `context API`를 사용함
15. `contexnt API` 에서 `value`는 1개만 넣자. 2개 이상 넣고싶다면 `createContext` 에 객체 형태로 묶어서 넣자

```javascript
// Context API: props drilling을 방지하기 위해 사용한다.
// ContextAPI는 상태관리 역할은 하지 않는다. data만 가져다 사용하는 기능이다. 단독으로 수정은 불가)

import React, { useState, useContext } from 'react';

const TestContext = React.createContext();  // Context API 생성

function App() {
    let [content, setContent] = useState("a");
    return (
        <div>
            <TestContext.Provider value={content}>
                <FirstComponent />
            </TestContext.Provider>
        </div>
   )
}

function FirstComponent = () => <SecondComponent />;

function SecondComponent = () => {
    const data = useContext(TestContext);
    return(
        <div>{data}</div>
    )    
}

export default App;
```

1.  `contextAPI`를 사용해서 `value`를 넘겨받는 예제

```javascript
import React, { useState, useContext } from 'react';

const CircleSizeContext = React.createContext();

function CircleSizeProvider(props) {
  // 원의 크기를 지정해주고, 원의 크기는 변화할 수 있으므로 State로 지정.
  const [circleSize, circleSizeChange] = useState(20);
  return (
    <CircleSizeContext.Provider value={{ circleSize, circleSizeChange }}>
      {props.children}
    </CircleSizeContext.Provider>
  );
}

function Circle() {
  const { circleSize, circleSizeChange } = useContext(CircleSizeContext);
  
  return (
    <div
      onClick={() => circleSizeChange(circleSize + 20)}
      style={{
        width: circleSize + "px",
        height: circleSize + "px",
        background: "red",
        borderRadius: "50%",
      }}
    />
  );
}

function App() {
  return (
    <CircleSizeProvider>
      <div className="App">
        <h1>Click circle</h1>
        <div style={{ display: 'flex', justifyContent: 'center'}}>
          <Circle />
        </div>
      </div>
    </CircleSizeProvider>
  )
}

export default App;
```

---
## 📍 57일차 1. 12. 수. 온라인강의
오늘은 `상태관리`를 중심으로 `redux`, `contextAPI`, `prop drilling`, `MVC`, `Flux` 패턴에 대해서 배웠다. `MVC`과 `Flux`패턴의 가장 큰 차이는 상태가 연속적으로 바뀌는지 여부인데, `MVC` 패턴에서 만약, `view`의 특정 값이 업데이트 된다면, 해당 `view`를 관리하는 `model`이 업데이트되고 해당 `model`을 구독하는 `view`도 함께 업데이트되는 연쇄적인 모습이 일어난다. 만약에 앱의 사이즈가 클 때 이와 같은 연쇄적으로 동작하게 된다면 업데이트의 흐름을 따라가기 힘들다. 반면에 `Flux`는 하나의 `Action`이 하나의 `update`만을 만들도록 한다. (최종적으로는 데이터가 `store`에서 `view`로만 흐른다.) 이것의 장점은 업데이트가 한 방향으로만 흘러가기 때문에 `UI`의 업데이트를 예측하기 쉬워진다. 그리고 지나가다 용어가 헷갈려서 남긴다. `nextJS`: `react`로 사용하는 `SSR`, `nuxtJS`: `vue`로 사용하는 `SSR`, `nestJS`: `node`를 쓰는 프레임워크

### ❏ 상태관리
1. 앱 상에서의 데이터를 메모리(`localStorage`, `JS memory`) 등에 저장하고 하나 이상의 컴포넌트에서 데이터를 공유하는 것
2. 한 컴포넌트 안에서의 상태, 여러 컴포넌트 간의 상태, 전체 앱의 상태 관리를 모두 포함
3. `MPA`: 서버의 데이터를 이용해 페이지를 렌더링하므로, 클라이언트의 데이터와 서버의 데이터가 큰 차이를 가지지 않음
4. `SPA`: 자체적으로 데이터를 갖고, 서버와의 동기화가 필요한 데이터만을 처리한다. 그 외의 데이터는 `Client`만의 데이터로 유지 (서버에서 매번 `data` 를 받아오지 않는다.)
5. 상태가 많지 않거나, 유저와의 인터렉션이 많지 않다면 매 작업 시 서버와 동기화하더라도 충분함
6. 앱이 사용하는 데이터가 점점 많아지고, 유저와의 인터렉션 시 임시로 저장하는 데이터가 많아지는 경우 상태관리를 고려
7. 프론트엔드 뿐만 아니라, 백엔드와의 데이터 통신도 충분히 고려해야 함.(`GraphQL`)
8. `Children.toArray()`: `this.props.children`을 하부로 전달하기 전에 다시 정렬하거나 일부만 잘라내고 싶을 때에 유용합니다. `React.Children.toArray()`는 `children`을 평평하게(Flatten) 만들 때, 중첩된 배열들의 의미를 보존하기 위하여 `key`를 변경합니다. 즉, `toArray`는 반환되는 배열에 `key` 값을 덧붙여서 각 엘리먼트가 갖는 `key`가 평평해진 배열 내에서만 유효한 범위를 형성하도록 해줍니다.

### ❏ 상태관리 장, 단점
1. 높은 품질의 코드를 작성하는 데 유리(하나의 `store` 에서 관리)
2. 성능 최적화, 네트워크 최적화 등에 유리(타이핑을 했을 때 매번 서버와 통신할 필요가 없다.)
3. 데이터 관리의 고도화(`localStorage` 를 활용한 `persist state`, `offline` 일때 `localStorage` 사용 등)
4. `Boilerplate` 문제
5. 파악해야 할 로직과 레이어가 많아짐
6. 잘못 사용할 경우, 앱의 복잡도만을 높이거나, 성능을 악화시킨다. `global state` 의 잘못된 활용 시 앱 전체 리렌더링 발생
7. 즉, 상태관리 도입시 섬세하게 상태를 디자인하고 성능을 고려해야한다.

### ❏ 상태관리 기술이 해결하는 문제들
1. 데이터 캐싱과 재활용

```js
1. SPA에서 페이지 로딩 시마다 모든 데이터를 로딩한다면 사용자 경험 측면에서 MPA를 크게 넘어서기 힘듦
2. 오히려 네트워크 요청 수가 많아져 더 느릴 수도 있음.
3. 변경이 잦은 데이터가 아니라면, 데이터를 캐싱하고 재활용함
4. 변경이 잦다면, 데이터의 변경 시점을 파악해 최적화(ex, 일정 시간마다 서버에 저장, 타이핑 5초 후 서버에 저장)
```

2. `prop drilling`

```js
1. 컴포넌트가 복잡해지는 경우, 상위 부모와 자식 컴포넌트 간의 깊이가 커짐.
2. 최하단의 자식 컴포넌트가 데이터를 쓰기 위해 최상위 컴포넌트부터 데이터를 보내야 하는 상황이 발생한다.
3. Context API 등을 활용, 필요한 컴포넌트에서 데이터를 가져올 수 있음.
4. 컴포넌트 간의 결합성을 낮춘다.
```

### ❏ MVC, Flux 패턴
1. `MVC pattern`: 애플리케이션을 `Model`, `View`, `Controller` 로 분리하여 개발하는 소프트웨어 디자인 패턴 중 하나
2. `Flux pattern`

```js
- 2014년에 `META` 에서 제안한 웹 애플리케이션 아키텍쳐 패턴
- Unidirectional(일방향의(store -> view)) <-> Bidirectional(양방향의(store <-> view)), data flow를 활용하여 데이터의 업데이트와 UI반영을 최소화 시킨다.
- React의 UI패턴인 합성 컴포넌트와 어울리도록 설계한다.
- redux, react-redux 라이브러리의 Prior art, 나오기 이전에 연구된 패턴
- 하나의 유저 인터렉션이 무조건 하나의 업데이트만 만들 수 있는 것은 아닙니다. 예를 들어 특정 버튼을 클릭했을 때 여러개의 액션을 만들 수 있기 때문입니다.
- MVC 패턴의 경우, 하나의 유저 인터렉션 발생 시 그 인터렉션으로 발생한 업데이트가 다른 연쇄 업데이트를 만들어낼 수 있습니다. 따라서 업데이트의 근원을 추적하기 힘든 반면 Flux 패턴은 연쇄 업데이트가 아닌 단방향 업데이트만을 만들어낼 수 있습니다.
```

3. `MVC` 패턴에서는 `View` 에서 특정 데이터를 업데이트하면, 연쇄적인 업데이트(`view` 가 업데이트되면 해당 `view` 를 관리하는 `model` 이 업데이트되고 해당 `model` 을 구독하는 `view` 도 업데이트되고... )가 일어난다. 즉, 앱이 커질 때 업데이트의 흐름을 따라가기 힘들다
4. `flux` 는 하나의 `Action` 이 하나의 `Update` 만을 만들도록 한다.(최종적으로 데이터는 `store` 에서 `view` 로만 흐른다.) 업데이트가 한 방향으로 흐르므로 UI의 업데이트를 예측하기 쉬움.

### ❏ Flux 구조
1. `action` → `dispatcher` → `store` → `view` 순으로 데이터가 흐름
2. `store` 는 미리 `dispatcher` 에 `callback` 을 등록해, 자신이 처리할 `action` 을 정의
3. `action creator` 는 `action` 을 생성하여 `dispatcher` 로 보냄
4. `dispatcher` 는 `action` 을 `store` 로 넘김
5. `store` 는 `action` 에 따라 데이터를 업데이트 후, 관련 `view` 로 변경 이벤트 발생
6. `view` 는 그에 따라 데이터를 다시 받아와 새로운 UI를 만듬
7. 유저 인터렉션이 발생하면 `view` 는 `action` 을 발생

![](https://images.velog.io/images/abcd8637/post/1d73ad39-0983-49c2-9745-7748810384b4/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-12%2010.39.25.png)

![](https://images.velog.io/images/abcd8637/post/d2e10031-2dae-4da4-ae49-943eff781417/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-12%2010.42.34.png)

### ❏ 상태관리에 사용되는 훅
1. 외부 라이브러리 없이 `React` 가 제공하는 훅 만으로 상태 관리를 구현한다.
2. 함수형 컴포넌트에 상태를 두고, 여러 컴포넌트 간 데이터와 데이터 변경 함수를 공유하는 방식으로 상태를 관리한다.

### ❏ useState
1. 단순한 하나의 상태를 관리하기에 적합하다.

```js
const [state, setState] = useState(initState | initFn);
```

2. 상위 컴포넌트에서 `state` 와 `setState` 를 정의하고 해당 `state` 를 사용하는 `component` 까지 `prop` 으로 내려준다. 중간에 `state` 가 변경되면, 중간에 `state` 를 넘기기만 하는 컴포넌트들도 모두 리렌더링 된다.(리렌더링을 고려하면 `contextAPI` 가 나은 선택 일 수도 있다.) 상태와 상태에 대한 변화가 단순하거나, 상대적으로 소규모 앱에서 사용하기에 적합하다.

### ❏ useRef
1. 상태가 바뀌어도 리렌더링하지 않는 상태를 정의함 즉, 상태가 UI 변경과 관계없을 때 사용한다. (`setTimeout` 의 `timerID` 저장)
2. `uncontrolled component` 의 상태를 조작하는 등, 리렌더링을 최소화하는 상태관리에 사용(ex, `dynamic Form`)

### ❏ useContext
1. 컴포넌트와 컴포넌트간 상태를 공유할 때 사용
2. 부분적인 컴포넌트들의 상태관리, 전체 앱의 상태 관리를 모두 구현
3. `content provider` 안에서 렌더링되는 컴포넌트는, `useContext` 를 이용해 깊이 `nested` 된 컴포넌트라도 바로 `context value` 를 가져옴
4. `context value` 가 바뀌면 내부 컴포넌트는 모두 리렌더링 됨.
5. `Provider` 단에서 상태를 정의하고, 직접 상태와 변경 함수를 사용하는 컴포넌트에서 `useContext` 를 이용해 바로 상태를 가져와 사용하는 패턴
6. `useReducer` 와 함께, 복잡한 상태와 상태에 대한 변경 로직을 두 개 이상의 컴포넌트에서 활용하도록 구현 가능
7. `state` 는 필요한 곳에서만 사용하므로, 불 필요한 컴포넌트 리렌더링을 방지
8. `Prop drilling(plumbing)` 을 방지하여 컴포넌트 간 결합도를 낮춤

```javascript
// TodoContext.jsx
const TodoContext = createContext(null);

const initialState = {
	todos: [],
	filter: "all",
	globalId: 3000,
}

function useTodoContext(){
	const context = useContext(TodoContext);
	if (!context){
		throw new Error("Use TodoContext inside Provider")
	}
	return context;
}

function TodoContextProvider({ children}){
	const values = useTodoState();
	return (
		<TodoContext.Provider value={values}>
			{children}
		</TodoContext.Provider>
	)
}

function reducer(state, action){
	switch (action.type){
		case "change.filter":
			return { ...state, filter: action.payload.filter };
		case "init.todos":
			return { ...state, todos: action.payload.todos };
		case "add.todo":
			return { ...state, todos: [{ title: action.payload.title, id: state.globalId + 1 }], globalId: state.glbalId + 1 };
		case "delete.todo" : {
			return { ...state, todos: state.todos.filter((todo) => todo.id !== action.payload.id) };
		case "toggle.todo" : {
			return { ...state, todos: state.todos.map((t) => t.id === action.payload.id ? { ...t, completed: !t.completed } : t)};
		}
		default: return state;
  }
}

function useTodoState(){
	const [state, dispatch] = useReducer(reducer, initialState);
	const toggleTodo = useCallback( (id) => dispatch({type: "toggle.todo", payload: { id } }), []);
  const deleteTodo = useCallback( (id) => dispatch({type: "delete.todo", payload: { id } }), []);
  const addTodo = useCallback( (title) => dispatch({type: "add.todo", payload: { title } }), []);
  const changeFilter = useCallback( (filter) => dispatch({type: "change.filter", payload: { filter } }), []);
  const initializeTodos = useCallback( (todos) => dispatch({type: "init.todos", payload: { todos } }), []);

	return { state, toggleTodo, deleteTodo, addTodo, changeFilter, initializeTodos };  // dispatch 활용, 사용하기 편리해짐
}

// TodoApp.jsx
function TodoApp(){
	return(
		<TodoContextProvider>
			<TodosPage />
		</TodoContextProvider>

	)
}

// TodosPage.jsx
function TodosPage(){
	const { initializeTodos } = useTodoContext();

	useEffect(() => {
		console.log("useEffect");
		fetchTodos().then(initializeTodos);  // component 처음 mount 후 state todo로 업데이트하기
	}, [ininitializeTodos])

// 하위 컴포넌트들과의 커플링이 없음(props가 없다.)
	return(  
				<div>
					<TodoForm />
					<TodoFilter />
					<TodoList />	
				</div>	
	)
}

// TodoFilter.jsx
function TodoFilter(){
	const { state, changeFilter } = useTodoContext();
	const { filter } = state;

	return(
		<div>
			<label htmlFor="filter">Filter</label>
			<select
					onChange={(e) => changeFilter(e.target.value)}
					id="filter"
					name="filter"
					value={filter}
			>
		</div>
	)
}
```

### ❏ useReducer
1. `useState` 보다 복잡한 상태를 다룰 때 사용
2. 별도의 라이브러리 없이 `flux pattern` 에 기반한 상태관리를 구현.
3. `nested state` 등 복잡한 여러 개의 상태를 한꺼번에 관리하거나, 어떤 상태에 여러가지 처리를 적용할 때 유용하다.
4. 상태가 복잡하다면, `useState` 에 관한 `callback` 을 내려주는 것보다, `dispatch` 를 `prop` 으로 내려 리렌더링을 최적화하는 것을 권장한다.

```javascript
// dispatch로 action을 넣으면 reducer로 흘러간다. reducer에서 update된 state를 return하고 state가 업데이트 되고 해당 state를 구독하는 다른 component가 업데이트 된다.
const [state, dispatch(update Fn)] = useReducer(reducer, initState)  // reducer와 initState는 필수 값

const handleClick = useCallback(() => {
	setCount(count => count + 1);
})
```

---
## 📍 58일차 1.13.목. 실시간 강의
오늘은 기존에 `vanilla JS`를 연동하여 `redux`로 상태관리를 진행한것에 이어서 `react`로 `redux`, `react-redux` 라이브러리를 사용하여 상태관리 하는법을 배웠다. 실습을 위주로 강의를 진행했기때문에 글로 남길만한 내용이 별로없다. 그리고 마지막에는 `test` 코드 작성하는 법을 배웠는데, 이 과정은 내일이나 내일모레 이론강의 수강이후에 작성하겠다.

### ❏ 리덕스의 3가지 규칙
1. `단일 스토어`: 나의 애플리케이션 안에는 하나의 스토어가 들어가있다. 여러 개의 스토어를 사용할 수 있지만 상태관리가 복잡해질 수 있으므로 권장하지 않는다.
2. `읽기 전용 상태`: 리덕스 상태는 읽기 전용이다. 리덕스의 상태를 업데이트할때는 기존의 객체는 건드리지 않고 새로운 객체를 생성해주어야 한다. 불변성을 유지하는 이유는 내부적으로 데이터가 변경되는것을 감지하기 위해 얕은 비교(`shallow copy`) 검사를 하기 때문이다. 객체의 변화를 감지할 때 객체의 깊숙한 안쪽까지 비교하는것이아니라 겉핥기 식으로 비교하여 좋은 성능을 유지할 수 있는 것이다.
3. `순수 함수`: 변화를 일으키는 리듀서는 순수한 함수여야한다.

```
1. 리듀서는 이전 상태와 액션 객체를 파라미터로 받는다.
2. 파라미터 외의 값에 의존하면 안된다.
3. 이전 상태는 절대 건드리지 않고, 변화를 준 새로운 상태 객체를 만들어 반환한다.
4. 똑같은 파라미터로 호출된 리듀서 함수는 언제나 똑같은 결과 값을 반환해야 한다.
5. 리듀서 함수 내에서 랜덤값을 만들거나 Date 함수를 사용하여 현재 시간을 가져오거나, 네트워크 요청을 한다면 파라미터가 같아도 다른 결과를 만들어 낼 수 있기때문에 사용하면 안된다. 
이러한 작업은 리듀서 함수 바깥에서 처리하자. 액션을 만들때 처리해도되고, 리덕스 미들웨어에서도 처리해도 된다.
6. 네트워크 요청과 같은 비동기 작업은 미들웨어를 통해 관리한다.
```

### ❏ React-redux
1. 보통 프레젠테이셔널 컴포넌트(`props` 를 받아와서 화면에 `UI` 를 그려주기만 하는 컴포넌트)와 컨테이너 컴포넌트(리덕스와 연동되어있는 컴포넌트, 리덕스로부터 상태를 받아오거나, 리덕스 스토어에 액션을 디스패치하기도 한다.)를 분리한다. 필수 사항은 아님
2. `connect` vs `useSelector`, `useDispatch` 의 차이: `connect` 함수를 사용하여 컨테이너 컴포넌트를 만들 경우, 해당 컨테이너 컴포넌트의 부모 컴포넌트가 리렌더링 될 때 해당 컨테이너 컴포넌트의 `props` 가 바뀌지 않았다면 리렌더링이 자동으로 방지되어 성능이 최적화됩니다. 반면, `useSelector`를 사용하여 리덕스의 상태를 조회했을 때는 이 최적화 작업이 자동으로 이루어지지 않으므로, 성능 최적화를 위해서는 `React.memo` 를 컨테이너 컴포넌트에 사용해 주어야 합니다.\

```javascript
const TodosContainer = () => {(...)}

export default React.memo(TodosContainer);
```

3. `combineReducers`: `reducer`가 여러개 있다면, 하나로 합쳐주는 메소드
4. `reducer`를 구현할 때 `reducer`는 순수함수여야한다. `global variable`의 값을 수정하면 안된다.

### ❏ Test
1. `TDD`: 레이아웃을 짜고 테스트코드를 작성한 다음에 로직을 구현하는 경우가 많다. 테스트 주도만을 위하다보면 생산성이 저하될수도 있다.
2. `unit test`: 하나의 모듈을 기준으로 독립적으로 동작하는 가장 작은 단위의 테스트 → `react` 에서 `component` 단위로 테스트 할 수도 있다. 기능마다 대응하는 테스트코드 작성
3. `intergration test`: 한번에 모아서 테스트

---
## 📍 59일차 1.14.금. 온라인 강의
오늘은 `redux`, `react-redux`, `react-redux`에서 비동기 처리를 담당하는 `redux-thunk`, `redux-saga` 그리고 `react-redux`를 쉽게 작성할 수 있는 `react-toolkit`에 대해서 배웠다. 이전에 단순하게 `redux`만 배운것에 비하면 난이도가 상당히 올라갔다. 그래도 현업에서 자주 사용되는 상태관리니까 잘 알아둬야겠다. 

### ❏ Redux 소개
1. 앱 전체 상태를 쉽게 관리하기 위한 라이브러리
2. `Redux` 의 많은 개념들이 `Flux pattern` 에서 차용됨
3. 주로 `React` 앱과 많이 사용한다.

### ❏ Redux를 언제 사용할까?
1. 앱 전체 상태 관리가 필요할 때
2. 복잡한 비동기 처리가 있는 상태관리가 필요할 때(`redux-thunk`, `redex-saga`, `redux-observable` 등)
3. 앱의 상태가 복잡하고, 이를 체계적으로 관리하고 싶을 때(`redux-orm(state를 DB화 시키는 기능)`, `normalizer`)
4. 상태 관리 패턴을 도입하여, 여러 개발자와 협업하고 싶을 때
5. `logger`, `devtool` 등을 활용하여 상태를 관리할 필요가 있을 때

### ❏ Redux 핵심원칙
1. `Single source of truth`: `store` 는 단 하나이며, 모든 앱의 상태는 이곳에 보관됨
2. `Immutability`: 상태는 오로지 읽을 수만 있다. 변경하려면 모든 상태가 변경되어야 함
3. `Pure function`: 상태의 변경은 어떠한 사이드 이펙트도 만들지 않아야 함

### ❏ Action
1. 상태의 변경을 나타내는 개념
2. 어떤 형태든지 상관없으나, 주로 `type`, `payload` 를 포함하는 객체형태로 주로 사용됨

```js
// 상태변경외에 다른 일을 하면 안된다.
const action1 = {
	type: 'namespace/getMyData',
	payload: {
		id: 123
	}
}
```

### ❏ Action Creator
1. `Action` 을 생성하는 함수
2. 직접 `Action` 을 생성하는 것보다 `Action Cretaor` 를 활용하면 재사용성이 좋고, 하나의 레이어를 추가할 수 있음

```js
const addObj = (id) => ({
	type: 'namespace/getMyData',
	payload: {
		id: String(id).slice(1)  // layer
	}
})
```

### ❏ Store
1. 앱 전체의 상태를 보관하는 곳
2. `Action` 에 따라 `reducer` 에서는 새로운 상태를 만들어내며, `Store` 는 그 상태를 저장한다.
3. `Store` 의 상태는 불변하며, 매 액션이 발생할 때마다 새로운 객체가 만들어짐

```js
const store = createStore(reducer, initialState);
```
### ❏ Reducer
1. Action을 받아 새로운 State를 만든다.
2. `(state, action) => state` 의 인터페이스를 따름
3. 상태 변경 시 사이드 이펙트가 없어야 한다.

```js
const reducer = (state, action) => {
	switch (action.type){
		case 'namespace/getMyData',:
			const obj = { id: action.payload.id }
			return { ...state, obj }
		default:
			return state
	}
}

const store = createStore(reducer, initialState);
```

### ❏ Dispatch

1. `Action`을 `redux`로 보내는 함수
2. `dispatch` 후에 `action`은 `middleware`를 거쳐 `reducer`에 도달

```jsx
function MyApp(){
	const dispatch = useDispatch();
	return(
		<button
			onClick={
				() => dispatch(addObj(123))}
		>submit</button>
	)
}
```

### ❏ Selector
1. 특정 state 조각을 store로부터 가져오는 함수
2. store의 state는 raw data를 저장하고, 계산된 값 등을 selector로 가져오는 등의 패턴을 구사할 때 유용하다.
3. `Action creator`는 데이터를 리듀서를 보낼 때 로직을 넣어주고, `selector` 는 데이터를 얻어올 때 로직을 넣어준다.

```js
function MyApp() {
	const obj = useSelector(state => state.boj);
	return(
		<div>{JSON.stringify(obj)}</div>
	)
}
```

### ❏ Redux의 구조
1. `redux` 는 자유롭게 확장하여 사용할 수 있음
2. 내부적으로 `action` 과 데이터가 어떻게 흐르는지 이해하고 `middleware`, `enhancer` 등을 이용하여 `redux` 를 확장함
3. `middleware`: `action` 은 `dispatch` 이후 모든 `middleware` 를 먼저 통과한 후에 `reducer` 에 도달한다. 관련 라이브러리로는 `redux-thunk`, `redux-logger` 등이 있다.
4. redux-devtools같이, Enhancer는 전체 state의 상태를 중심으로 redux 동작을 확장한다.
5. redux-thunk는 Middleware의 예로, action object가 Promise를 리턴하는지 체크한다.

![](https://images.velog.io/images/abcd8637/post/4979f66b-0278-43fb-85e3-766eafc1cd13/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-14%2010.19.15.png)

### ❏ redux-toolkit
1. `redux` 라이브러리에서 공식적으로 추천하는 `helper` 라이브러리
2. 기존에 만들어야 하는 수많은 보일러 플레이트를 제거하고, 유용한 라이브러리를 포함하여 `redux` 코드를 쉽게 작성하게 도와 줌
3. `redux-devtools`, `immerjs`, `redux-thunk`, `reselect` 등의 라이브러리가 미리 포함됨

```js
// configureStore
// named parameter: 객체의 이름으로 쉽게 store 생성
// reducer 객체를 받아 combineReducers를 적용함.
// reducer를 여러개 넘기고 싶을 때 하나의 리듀서로 묶어준다. combineReducers를 사용하지 않아도 됨
// createStore를 사용할 때보다 간단하고 코드가 깔끔해지는 장점이 있다.
const store = configureStore({
	reducer: {
		posts: postsReducer,
		users: usersReducer
	}
})

// createAction
// action creator 함수를 만드는 함수
// 만들어진 action creator에 데이터를 넘기면 payload 필드로 들어감
// 생성된 action creator는 toString() 메서드를 오버라이드해, 자신이 생성하는 액션의 타입 String을 리턴
const addPost = createAction('post/addPost');
addPost({ title: 'post 1' })

/*
{
	type: 'post/addPost',
	payload: { title: 'post 1'}
}
*/

// createReducer
// reducer를 만들어주는 함수, initState를 넘기고 builder를 인자로 받는 콜백 함수
// addCase 메서드를 이용하여 action마다 state의 변경을 정의한다.
// immerjs를 내부적으로 사용하므로 mutable code를 이용해 간편하게 변경 코드를 작성 할 수 있다.(따로 복사하는 수고를 덜음)
const postsReducer = 
	createReducer(initState,
			builder => {
				builder.addCase(addPost,
					(state, action) => {
						state.posts
							.push(action.payload)
				})
	})

// createSlice
// Action creator, reducer 등 별도로 만들어야 하는 여러 Redux 구현체를 하나의 객체로 모은 것
// createSlice 함수를 이용하여 많은 보일러 플레이트를 없애고 쉽게 action creator, reducer를 만듬
// slice를 반환한 객체.actions에는 actionCreator가 있고, .reducer에는 정의된 reducer가 들어간다.
const postsSlice = createSlice({
	name: 'posts',
	initialState,
	reducers: {
		addPost(state, action) {
			state.posts
				.push(action.payload)
		}
	}
})

const { addPost } = postsSlice.actions;
const reducer = postSlice.reducer;

// createSelecor
// state를 이용한 특정 데이터를 리턴하도록 함
// 내부적으로 데이터를 캐시하며, 데이터가 변동이 없다면 캐시된 데이터를 리턴함(성능 향상)
const postsSelector = state => state.posts;
const userSelecor = state => state.user;
const postsByUserIdSelector = createSelector(
	postsSelector,
	useSelector,
	(posts, user) => 
		posts.filter(post =>
			post.username === user.username
	)
)
```

### ❏ react-redux
1. redux를 react앱에 연결하게 하는 라이브러리
2. 리액트에서 상태가 변화해도 `redux` 에서는 알 수 없다. 그래서 `react-redux` 로 연결해줘야 한다.
3. `redux`에서 관리하는 상태, `dispatch` 함수 등을 가져올 수 있음
4. 클래스, 함수 컴포넌트 모두 연결 가능

```js
// Provider
// Redux store를 react와 연결하기 위해서는 반드시 Provider로 컴포넌트를 감싸야 한다.
// Provider 안에서 렌더링된 컴포넌트들은 state, dispatch 등에 접근할 수 있음
// contextAPI를 내부적으로 사용하는 Provider, value 대신 store를 넣어준다.
const store = configureStore({
	reducer: rootReducer
})

function App(){
	return(
		<Provider store={store}>
			<MyPage />
		</Provider>
	)
}

// useDispatch
// redux의 dispatch 함수를 가져오기 위한 API
// dispatch로 action creator가 생성한 action을 보내면 redux 내부로 보내지게 된다.
// dispatch(addPost()) -> middleware -> reducer -> store
const addPost = createAction('addPost');
function MyPage(){
		const dispatch = useDispatch();
		const handleClick = () => dispatch(addPost());
		return(
			<button 
					onClick={handleClick}
			>Submit</button>
		)
}

// useSelector
// Redux store로부터 데이터를 얻기 위한 API
// selector function을 인자로 넘기면 state를 받아오는 변수
// selector function은 데이터에 어떤 변경을 가하면 안됨, 단지 값을 가져오는 용도로만 사용한다.
// 데이터를 특정 형태로 계산하여 읽을 수 있음
function MyPage(){
	const posts = useSelector(state => state.posts);
	
	return posts.map( post => <Post {...post} />)
}
```

### ❏ Redux를 이용한 비동기 처리
1. `redux` 는 비동기 처리를 자체 내장하지 않고 ,`redux-thunk` 같은 외부 익스텐션이 필요하다.
2. `redux` 비동기 처리를 위해서는 비동기를 위한 `middleware` 를 추가해야 함
3. `redux-toolkit` 에는 `redux-thunk` 가 내장되어있다.
4. `redux-thunk` 는 `Promise` 를 이용한 비동기 `Action` 을 쉽게 처리하도록 하는 `middleware`
5. `redux-toolkit` 에는 정해진 `convention` 이 있고, 그것을 따라야 한다.
6. `redux-thunk` 이외에도 `redux-sage` 의 `saga 패턴`, `redux-observable` 의 `rxjs` 가 있다. 복잡한 비동기 처리가 필요하면 `redux-sage`, `redux-observable` 를 동시에 사용해서 처리할 수 있다.

```js
// createAsyncThunk
1. redux-toolkit에서는 thunk middleware를 디폴트로 추가
2. redux-toolkit은 createAsyncThunk API를 제공함 fulfilled, rejected, pending 3가지 상태에 대해 각각 reducer 작성
3. Typescript 환경에서 reducer 작성 시, builder callback을 사용하여 작성해야 정확한 타이핑이 가능하다. 

// createAsyncThunk는 두 인자 action type, async callback(payload creator)를 받음
// action type을 주어지면, pending, fulfilled, rejected가 각각 postfix로 붙어 reducer로 들어옴 (posts/addPost/pending)
const addPost = createAsyncThunk('posts/addPost', 
	async (title) => {
		const result = await PostAPI.addPost({ title })
		return result.data
	}	
)

useEffect(() => {
	dispatch(addPost('post 1'))
})

// createAsyncThunk로 만들어진 action creator는 4가지 함수로 구성
// addPost - async 함수를 dispatch하는 함수
// addPost.pending - promise를 생성했을 때 발생하는 액션
// addPost.fulfilled - promise가 fulfilled 일 때 발생하는 액션, fulfilled시 데이터는 payload로 들어옴(action.payload.todos)
// addPost.rejected - promise가 rejected 일 때 발생하는 액션, rejected시 에러는 action.error로 들어오며, payload는 undefined가 된다.
// extraReducers 함수를 이용해, builder에 각 상황에 대한 리듀서를 추가
// 공식적으로 builder pattern을 추천하는데 타입스크립트에서 타이핑이 용이하기 때문임
const postsSlice = createSlice({
	extraReducers: builder => {
		builder
			.addCase(addPost.pending. state => ...)
			.addCase(addPost.fulfilled. state => ...)
			.addCase(addPost.rejected. state => ...)
	}
})

// 연속적인 비동기 처리
// thunk 함수를 dispatch하면 promise가 리턴 따라서, then() 메서드로 연속적인 비동기 처리를 이어 실행
dispatch(addPost('post1'))
	.then(() => )

dispatch(updatePost('post1'))

// 동시 비동기 처리
// Promise.all을 이용해, 여러 비동기 처리를 동시에 실행한다.
// 주의할 점은 thunk의 promise가 rejected 되어도 .then()으로 들어온다는 것
Promise.all([
	dispatch(addPost('post1')),
  dispatch(updatePost('post2')),
])
	.then(() =>
		console.log("DONE"))
```

---
## 📍 60일차 1.15.토. 온라인 강의
오늘은 `testing`, `jest`에 대해서 배웠다. 취업 공고를 보다보면 `jest`도 사용 스택에 포함되어있는것을 많이 봤는데, 언제 공부하나 이런생각이 들었다. 이번을 계기로 `test`와 많이 친해지고, `jest`도 많이 다뤄야 겠다는 생각이 들었다.

### ❏ React 테스팅
1. 코드 테스트가 필요한 경우

```js
1. 코드를 작성하고 나면, 원하는 대로 동작하는지 알기 위해 테스트를 함
2. 코드에 버그가 있으면, 어떤 상황에서 버그가 발생하는지를 알기 위해 테스트를 함
3. 코드를 리팩토링하면, 원래대로 동작하는지 테스트함
4. 리액트 앱의 컴포넌트가 늘어날수록, 컴포넌트끼리 서로 영향을 미치는 경우가 많아짐
5. 특정 코드가 수정되면, 어떤 컴포넌트에 에러가 발생할 수 있음 
```

2. 테스팅 코드 작성의 이점

```js
1. 언급한 상황들에 대한 테스팅 코드를 작성하며, 미연의 에러를 방지
2. TDD(Test Driven Development) 등의 방법론을 적용하여 생산성을 향상
3. 테스트가 늘어나면서 테스트 코드가 구현 코드에 대한 문서화가 됨
4. 테스트가 용이하게 코드를 작성하여, 코드 품질과 신뢰성을 높임
```

3. 테스터블한 코드 작성하기

```js
1. 코드가 영향을 미치는 범위를 최대한 줄인다. 사이드 이펙트(함수 내에서 외부 변수 값을 변경하는 기능 등)를 줄임
2. 하나의 함수가 너무 많은 일을 하지 않게 함
3. 기능들을 작게 분리함
```

4. 주요 테스팅 용어

```js
1. Mocking: 특정 동작을 흉내 내는 것(실제 API를 호출하는 게 아니라 가짜 payload를 반환하는 mocking function을 만듦, unit test에 적합하게 끔 데이터를 만든다.)
2. Stubbing: 더미를 채워 넣는 것(Child 컴포넌트를 렌더링하지 않고, 대신 그 자리에 <div>등을 채워 넣음)
```

5. 테스트의 구성

```js
1. setup: 테스트하기 위한 환경을 만든다. mock data, mock function 등을 준비함
2. expectation: 원하는 테스트 결과를 만들기 위한 코드를 작성함
3. assertion: 정말 원하는 결과가 나왔는지 검증함
```

6. 예제 코드

```js
// 테스트 할 함수
const transformUser = (user) => {
	const { name, age, address } = user
	return [ name, age, address ];
}

// 테스트 코드(jest)
test('Test transformUser', () => {
	// setup
	const mockUser = { name : 'testName', age: 20, address: 'testAddress' }

	// expectation
	const result = transformUser(mockUser)

	// assertion
	expect(result).toBe(['testName', 20, 'testAddress'])
})
```

7. `white-box testing`: 컴포넌트 내부 구조를 미리 안다고 가정하고 테스트 코드를 작성
8. `black-box testing`: 컴포넌트 내부 구조를 모른 채 어떻게 동작하는지에 대한 테스트 코드를 작성, 단순하게 컴포넌트가 렌더링한 무언가를 인터렉션했을 때 어떤 결과가 나오는지를 테스트한다.
9.  테스팅 범위에 따른 분류

```js
1. Unit 테스팅
2. Integration 테스팅
3. end-to-end(e2e) 테스팅
```

10. Unit Testing

```js
1. 다른 부분과 분리된 작은 코드를 만들고 그것을 테스트 함
2. 작은 코드는 function, module, class 등을 의미
3. 각 부분이 원하는 대로 동작함을 보장하기 위함
4. 테스트는 서로 분리되어야 함(특정 컴포넌트가 데이터에 따라 잘 렌더링되는지를 테스트하는 경우)

function getUpperCaseTesting(str){
	return str.toUpperCase();
}

expoect(getUpperCaseTesting('lower')).toBe('LOWER');
```
11. Intergration Testing

```js
1. 앱의 특정 부분이 동작하는지 테스트함
  - 여러 컴포넌트가 한꺼번에 동작하거나, 어떤 페이지의 부분이 잘 동작하는지를 테스트하는 경우
  - react-router, redux 등이 특정 컴포넌트와 함께 잘 동작하는지를 테스트하는 경우
```

12. End-to-end Testing

```js
1. 유저가 어떤 시나리오를 가지고 그 시나리오의 end-to-end로 잘 동작하는지 테스트함
2. 필요한 경우 웹서버, 데이터베이스를 실행함
3. 범위가 너무 넓어서 에러가 발생했을 때 특정 기능이 안 된다는 것은 알 수 있지만 정확히 어떤 부분에 문제가 생겼는지 알기 힘듬
4. 유저가 회원가입 후 로그인하여 유저 정보 페이지를 볼 수 있는지 테스트 하는경우
5. 전체 큰 범위를 확인하기 때문에 side-effect가 얼마든지 가능하다.
```

### ❏ Jest
1. facebook에서 오픈소스화한 테스팅 프레임워크
2. assertion 함수들, test runner, mock 라이브러리 등을 모두 제공
3. create-react-app에서 기본적으로 사용됨
4. 사용성이 좋고, 가장 인기있는 프로젝트

```jsx
// jest의 핵심 기능들
1. assertion matchers(toBe, toEqual)
2. async assertion(async/await, done)
3. mock functions(jest.fn().mockReturnValueOnce(), jest.mock('axios'))
4. testing lifecycle functions
5. grouping(컴포넌트 별 grouping, describe())
6. snapshot testing(스냅샷을 저장한 값이 리턴 값과 같은지 확인)
```

5. Assertion matchers

```js
1. jest는 풍부한 matcher를 제공하여, 여러 상황에서 match를 체크함
2. expect()는 expectation object를 리턴한다. 이 object의 메서드를 이용해 여러 매칭상황을 assert함
3. not을 prefix로 붙여 negative 상황도 매칭할 수 있다.

expect("hi").toMatch("hi")
expect(true).toBe(false)
expect(user).toBeDefined()
expect(fn).toHaveBeenCalledWith()
expect().not.toBe()
```

6. Async Assertion

```js
1. 비동기 상황의 테스트를 처리할 수 있는 여러 방법 제공
2. callback, promise, async / await를 모두 활용할 수 있음

useEffect(() => {
	fn()
		.then(setData)
}, [])
```

7. Mock functions

```js
1. mock function을 만듬
2. 모듈 전체를 mocking 함
3. 라이브러리 전체를 mocking 함

jest.mock('../mocks/api.js');  // 특정 컴포넌트가 사용하는 모듈을 mock처리한다.
```

8. lifecycle functions

```js
1. 각 테스트의 시작과 끝, 전체 테스트의 시작과 끝에 원하는 작업을 할 수 있다.
2. beforeEach, afterEach, beforeAll, afterAll 함수를 활용함
3. describe 블록 안에 사용하면 별도의 scope를 가짐  
4. 무거운 data를 load하고 test하는 경우: beforeAll
5. 함수 실행 후 무언가를 처리할 때, 메모리 해제 등: afterAll

// 안쪽 beforeEach는 scope안에서만 작동한다.
describe("~", () => {
	beforeEach(() => {})
	descibe("~"), () => {
		beforeEach(() => {})
	}
})
```

9. Grouping

```js
1. describe 함수를 이용해 여러 test()함수를 논리적으로 나눔
2. describe 함수 안에 describe 함수가 중첩될 수 있음
```

10. Snapshot Testing

```js
1. 특정 함수, 모듈, 컴포넌트 등의 결과를 seializable 한 형태의 snapshot으로 저장하고, 추후 변경이 발생했을 대 이전의 snapshot과 새로운 snapshot을 비교하여 변경이 발생했는지 추측함
2. jest의 주요기능으로, 코드의 변경이 컴포넌트의 렌더링 결과에 영향을 미치는지를 파악하기에 적합함
3. TDD는 테스트기능을 정의하고 구현한다. (결과를 테스트하기 때문에 TDD와 적합하지 않다)
```

11. jest함수의 실행순서

```js
1. beforeAll, beforeEach, afterEach, afterAll의 순서로 Lifecycle 함수들이 실행됨
2. 다만, describe 블록 안에 있는 before-*, after-* 함수는 해당 블록의 범위 안에서 실행됨
3. describe 함수는 모든 test() 함수 이전에 실행된다. 따라서 test() 함수들은 순차적으로 한꺼번에 실행된다.
```

12. 테스팅의 구성

```js
test('User component', () => {
	// setup
	const mockProps = {
		name: 'test-username',
		age: 20,
	}

	// expectation
	const { container } = render(<User {...mockProps} />)

	// assertion
	expect(container.firstChild).toMatchSnapshot()
})
```

### ❏ Jest 활용

1. Assertion Matchers 활용

```js
// toBe()는 객체의 내용을 비교하고, toEqual()은 객체 자체를 비교할 때 사용한다.
// example 1: toBe()
function isPythagorean(a, b, c){
	return a * a + b * b + c * c === c * c
}

test('Should 3, 4, 5 pythagorean', () => {
	expect(isPythagorean(3, 4, 5)).toBe(true)  // JS의 Object.is로 테스트한다.
})

test('Should 3, 4, 6 not pythagorean', () => {
	expect(isPythagorean(3, 4, 6)).toBe(false)
})

// example 2: toEqual(), toMatch()
function createTodo(id, title, content){
	return { id, title, content }
}

test('Should create user', () => {
	const id = 1, title = "Test todo", content = "Test content";
	expect(createUser(id, title, content).toEqual({id, title, content})  // deep Equality check(nested object)
})

test('Should create user', () => {
	const id = 1, title = "Test todo", content = "Test content";
	expect(createUser(id, title, content).title).toMatch("Test todo")  // check string, reg
})

// example 3: toContain()
function transformUser(user){
	const { name, age, address } = user;
	return [ name, age, address ]
}

test('Should contain name after transformUser', () => {
	const user = { name: 'test name', age: 20, address: 'test address' }
	expect(transformUser(user)).toContain('test name')  // 포함여부를 확인(in)
})

test('Should contain name after transformUser', () => {
	const user = { name: 'test name', age: 20, address: 'test address' }
	expect(transformUser(user)).not.toContain(30)
})
```

2. Async assertion

```js
1. callback 패턴의 경우, test()함수가 제공하는 done() 함수를 활용하여 콜백이 끝나고 done()을 호출, 에러가 발생하면 done()의 인자로 에러를 넘김
2. Promise 패턴의 경우 async/await을 활용하거나, Promise를 리턴

function isPythagoreanAsync(a, b, c){
	return new Promise(resolve => {
		setTimeout(() => {
			const result = isPythagorean(a, b, c)
			if(result) return resolve(result)
			reject(new Error("Not pythagorean"))
		}, 500)
	})
}

test('Should 3, 4, 5 be pythagorean async', (done) => {
	isPythagoreanAsync(3, 4, 5).then(done).catch(done)
})

test('Should 3, 4, 5 be pythagorean async', (done) => {
	return expect(isPythagoreanAsync(3, 4, 5)).resolves.toBe(true)  // resolve 된 값이 true인지?
})

test('Should 3, 4, 6 be pythagorean async', (done) => {
	return expect(isPythagoreanAsync(3, 4, 6)).rejects.toBe('Not pythagorean')  // reject 된 값이 message와 같은지?
})
```

3. mock functions

```js
1. jest.fn()을 활용하여 mock function 객체를 만듬
2. mockReturnValueOnce() 등으로 리턴하는 값을 임의로 조작한다. 여러번 호출하면 순서대로 세팅된 값을 반환함
3. mockResolvedValue() 로 promise가 resolve하는 값을 조작함
4. jest.mock()으로 특정 모듈을 mocking 함
5. toHaveBeenCalled - 이 함수가 호출되었는지 검증.
6. toHaveBeenCalledWith(arg1, arg2...) - 이 함수가 특정 인자와 함께 호출 되었는지 검증
7. toHaveBeenLastCalledWith(arg1, arg2...) - 마지막으로 특정 인자와 함께 호출되었는지 검증
```

4. Lifecycle functions

```js
// beforeEach()
beforeEach(() => {
	setupMockData()
})

// afterEach()
afterEach(() => {
	clearMockData()
})
```

5. Grouping

```js
// describe(), block으로 묶어서 관리
describe('This is group 1', () => {
	describe('This is inner group 1', () => {
		test('Test 1', () => {})

	describe('This is inner group 2', () => {
		test('Test 2', () => {})
	})
})
```

6. snapshot testing

```js
1. toMatchSnapshot()을 호출하면, 기존에 스냅샷이 없었을 경우 .snap 파일을 만듬
2. 기존 스냅샷이 있을 경우, 새로운 스냅샷과 비교하여 변경 사항이 있으면 테스트는 실패함
3. toMatchInlineSnapshot()을 호출하면 별도의 스냅샷 파일을 만들지 않음. 이 경우, 어떻게 스냅샷이 쓰였는지를 하나의 파일 안에서 알 수 있게 됨

test('Snapshot test form', () => {
	const { container } = render(<MyForm />)
	expect(container.firestChild).toMatchSnapshot()
})

test('Snapshot test form', () => {
	const { container } = render(<MyForm />)
	expect(container.firestChild).toMatchInlineSnapshot()
})

expect(container.firstChild).toMatchInlineSnapshot(`
	<div>
		<form>
		...
		</form>
	</div>
`)
```

### ❏ react-testing-library
1. 테스트가 소프트웨어가 사용되는 모습을 닮을수록, 테스트를 더욱 신뢰할 수 있게 됨
2. The more your tests resemble the way your software is used, the more confidence they can give you
3. React 컴포넌트의 특정 메서드나 상태를 테스트하는게 아니라 실제 유저가 사용하는 방식대로 테스트하는 접근
4. 유저가 페이지에서 어떤 DOM 요소에 접근하는 방법을 흉내냄 이러한 방식으로 테스트 코드를 작성하면, 내부 구현이 바뀌어도 테스트가 깨지지 않는다.
5. React 컴포넌트가 렌더링한 결과에 대한 접근만 가능함
6. 쿼리는 내부 상태나 내부 메서드에 접근할 수 없게 설계됨, 결과에 대한 접근만 가능

```js
// get
1. getBy: 원하는 요소를 찾지 못할 경우나 여러개의 요소를 찾을 경우 에러를 던짐
2. getAllBy: 여러 요소를 찾아 배열을 반환, 원하는 요소를 찾지 못할 경우 에러르 던짐
3. 원소가 반드시 페이지에 존재해야만 하는 경우 활용함

// find
1. findBy 관련 쿼리는 원하는 원소가 없더라도 비동기적으로 기다림
2. 여러 원소를 찾거나, 정해진 timeout동안 찾지 못하면 에러를 던짐
3. findAllBy 관련 쿼리는 여러 원소를 검색해 배열을 반환한다. 정해진 timeout동안 찾지 못하면 에러를 던짐
4. Promise를 리턴하며, 실패시 reject, 성공시 resolve
5. 어떤 유저의 동작 후에 등장하는 원소 등을 테스트하고자할 때 활용함

// query
1. queryBy 관련 쿼리는 getBy와 비슷하게 원소를 찾아 반환하나, 못찾을 경우 에러를 던지지 않고 null을 반환함. 여러 원소를 찾으면 에러를 던짐
2. queryAllBy 관련 쿼리는 getAllBy와 비슷하게 여러개의 원소를 찾아 배열로 반환하거나, 하나도 찾지 못하면 에러 대신 빈 배열을 반환함
3. 특정 요소를 찾을 수 없음을 assertion의 기준으로 둘 때 활용됨

// container
1. container는 컴포넌트를 렌더한 결과를 감싸는 원소
2. queryselector(), querySelectorAll()을 이용해 selector문법으로 원소를 선택할 수 있음

// jest-dom
1. react-testing-library는 jest를 확장하여, 좀 더 쓰기 편한 assertion을 제공함
2. toBeInTheDocument(), toHaveValue(), toBeDisabled(), toBeVisible() 등 DOM 테스팅에 특히 유용한 assertion 메서드를 제공함 
```

### ❏ 쿼리의 우선순위
7. 유저가 페이지를 이동하는 방식에 가까운 쿼리일수록 우선순위가 높음
8. 접근성 높은 HTML을 작성할 수록 테스트가 용이한 코드가 됨(sementic web)

```js
// ByRole
1. accessibility tree에 있는 요소들을 기준으로 원소를 찾음
2. 유저가 웹 페이지를 사용하는 방식을 가장 닮은 쿼리
3. 동일한 role을 가진 경우, accessible name을 이용해 원소를 구별함
4. 임의로 role 혹은 aria-*을 부여하는 것을 지양함
5. 자주 사용되는 role - button, checkbox, listitem, heading, img, form, textbox, link
6. 자주 사용되는 accessible name (button - 텍스트), (label - 텍스트), (a - 텍스트), (img - alt 텍스트)

<button role="button">submit</button>
<input type="checkbox" role="checkobx" />

test('제출 버튼을 찾아 클릭하면, username 인풋이 비워진다.', () => {
	const { getByRole } = render(<TestForm />);
	const usernameInput = getByRole('textbox', { name : 'Username' })
	const submitButton = getByRole('button', { name : 'Submit' })
	userEvent.type(usernameInput, 'test username')
	userEvent.click(submitButton)
	
	expect(usernameInput).toHaveValue("")  // jest-dom 
})

// Text
1. 유저가 볼 수 있는 Text 값을 기준으로 쿼리로 찾음
2. ByLabelTest - label과 연관된 원소를 찾음
3. ByPlaceholderTest - placeholder과 연관된 원소를 찾음
4. ByText - 주어진 Text와 연관된 원소를 찾음
5. ByDisplayValue - input, textarea, select 등의 value를 기준으로 원소를 찾음

test('제출 버튼을 찾아 클릭하면, username 인풋이 비워진다.', () => {
	const { getByLabelText, getByText } = render(<SimpleTestForm />);
	const usernameInput = getByLabelText('username')
	const submitButton = getByText('Submit')

	userEvent.type(usernameInput, 'test username')
	userEvent.click(submitButton)
	
	expect(usernameInput).toHaveValue("")  // jest-dom 
})

// semantic queries
1. 유저에게 보이지 않지만 접근성 스펙에 적합한 alt, title을 이용하여 원소를 검색함
2. ByAltText - img, area, input 등의 alt 속성으로 원소를 검색함
3. ByTitle - title 속성으로 원소를 검색함

// Test ID
1. data-testid 속성을 원하는 원소에 지정하고, 쿼리를 이용해 찾음
2. 유저가 해당 속성을 기반으로 화면의 요소를 찾는게 아니므로 우선순위가 낮음
3. 다른 쿼리로 테스트를 작성할 수 없을 때 이 쿼리를 백도어로 활용함

test('제출 버튼을 찾아 클릭하면, username 인풋이 비워진다.', () => {
	const { getByTestId } = render(<SimpleTestForm />);
	const usernameInput = getByTestId('username-input')
	const submitButton = getByTestId('submit-button')

	userEvent.type(usernameInput, 'test username')
	userEvent.click(submitButton)
	 
	expect(usernameInput).toHaveValue("")  // jest-dom 
})
```

### ❏ user-event
1. 내장 이벤트함수인 `fireEvent`, `createEvent`를 좀 더 직관적이고 범용적으로 사용할 수 있도록 만든 라이브러리
2. `click`, `type`, `keyboard`, `upload`, `hover`, `tab` 등 유저가 실제로 웹페이지를 사용하며 만드는 이벤트를 메서드로 제공함

```js
// click
userEvent.click(submitButton)
userEvent.click(submitButton, { shiftKey: true })
userEvent.click(submitButton, { shiftKey: true }, { clickCount : 5 })

test('숨은 텍스트를 보여준다', () => {
	const text = "Hidden text!";
	
	const { getByRole, queryByText } = render(<Expansion text={text} />);
	expect(queryByText("Hidden text!")).toBe(null);
	
	const showButton = getByRole("button", { name: "Expand" }):
	expect(showButton).toBeInTheDocument();  // jest dom assertion

	userEvent.click(showButton);
	expect(queryByText(text)).toBeInTheDocument();
})

function Expansion({ text }){
	const [expanded, setExpaned] = useState(false);
	
	return(
		<div>
			<button onClick={() => setExpanded(b) => !b)}>Expand</button>
			{expanded && <div>{text}</div>}
		</div>
	);
}

// type
userEvent.type(inputElement, 'react advanced')
userEvent.type(inputElement, 'react{space}advanced{enter}')  // 어떤 곳들에 입력하는지 지정가능
await userEvent.type(inputElement, 'react advanced', { delay: 300 })  // 비동기적인 테스트 가능

test('Typeahead에서 쿼리에 따른 검색 겨롸를 보인다.', () => {
	const mockSearchData = ['kim', 'ted', 'an', 'jeong'];
	
	const { getByPlaceholderText, getAllByRole } = render(
		<Typeahead searchData={mockSearchData} />
	);
	
	const inputElement = getByPlaceholderText('type name...');
	userEvent.type(inputElement, 'a');

	expect(getAllByRole('listitem').length).toBe(2);

	userEvent.clear(inputElement);
	expect(getAllByRole('listitem').length).toBe(mockSearchData.lengh);
});
```