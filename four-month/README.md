## ๐ 61์ผ์ฐจ 1.18.ํ. ์ค์๊ฐ ๊ฐ์
์ด๋ฒ์ฃผ๊ฐ ๋ง์ง๋ง ์ ๊ท ์์์ด๊ณ  ๋ค์์ฃผ๋ถํฐ ๊ต์ก๊ณผ์ ์ด ์ข๋ฃ๋๋ ์ฃผ๊น์ง๋ 2์ฐจ ํ๋ก์ ํธ ๊ธฐ๊ฐ์ผ๋ก ์งํ๋๋ค. ๋ฒ์จ ๊ต์ก์ ๋ค์์ง๋ 4๊ฐ์์ด ๋์ด๊ฐ๋ค๋... ์๊ฐ์ด ์ฐธ ๋น ๋ฅธ๊ฒ ๊ฐ๋ค. ์๋ฆฌ์ค ๊ต์ก์ ๋ค์ผ๋ฉฐ ํ๋ก ํธ๋ถํฐ ๋ฐฑ์๋๊น์ง ๋คํธ์ํฌ ํต์ ์ ๋ํด ๋๋ต์ ์ธ ํฐ ํ๊ณผ ํ๋ก ํธ์๋์์ ์ฌ์ฉํ๋ ์ธ์ด, ํ๋ ์์ํฌ ๋ฑ ๋ค์ํ ๋ด์ฉ๋ค์ ๋ฐฐ์ ๋ค. ์ฐธ์ผ๋ก ๋์์ด ๋ง์ด ๋์๋ค. ๊ต์ก์ด ๋๋  ๋๊น์ง ์ด์ฌํ ๊ณต๋ถํด์ ํ์์์ ํจ๊ป ์ผํ๊ณ  ์ถ์ ๊ฐ๋ฐ์๊ฐ ๋๊ณ  ์ถ๋ค. ๊ทธ๋ผ `SSR`, `CSR`, `style-components`, ๋ฐฐํฌ์ ๋ํด์ ๋ฐฐ์๋ณด์. ๋ง๋ถ์ฌ ์ค๋์ `json-server`, `github-action`, `CI-CD`, `webhook`, `nginx`์ ๋ํด์๋ ๋ฐฐ์ ๋ค.
 
### โ ์ด๋ก  ๊ฐ์
`development` ๋จ๊ณ์์ `API`๋ฅผ `RESTful`ํ๊ฒ ํต์ ํ  ์ ์๋ ๊ฐ๋จํ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๊ฐ ์๋๋ฐ ๋ฐ๋ก `json-server`๋ค. ์ฌ์ฉ๋ฒ๋ ์ด๋ ต์ง ์์๋ฐ, `npx json-server --watch <์คํ ํ  ํ์ผ ๋ช>` ์ ํฐ๋ฏธ๋์ ์น๋ฉด ๊ณง๋ฐ๋ก ์ฌ์ฉํ  ์ ์๋ค. ๋๋ `db.json` ํ์ผ์ ์์ฑํ๊ณ  ๋ค์๊ณผ ๊ฐ์ด ์์ฑํ๋ค. ์ด๋ ๊ฒ ๊ฐ๋ฐ๋จ๊ณ์์ ์์์ ์ผ๋ก `API`๋ฅผ ๋ง๋ค์ด ํต์ ํ๋ ์๋ฒ๋ฅผ `mock server`๋ผ ๋ถ๋ฅด๋๋ฐ, ํ๋ก์ ํธ ์งํ์ค์ ๋ฐฑ์๋์์ `API`๊ฐ ๋ง๋ค์ด์ง์ง ์์์ ๋ ์ฌ์ฉํ๋ฉด ๊ด์ฐฎ์ ๊ฒ ๊ฐ๋ค. `db.json`์์ ์ฌ๋ฌ๊ฐ์ ๋ฐ์ดํฐ๋ฅผ `collection`์ด๋ผ ๋ถ๋ฅด๊ณ , ๋จ์ผ ๋ฐ์ดํฐ๋ฅผ `element`๋ผ๊ณ  ๋ถ๋ฅธ๋ค.

```javascript
{
    "topics":[
        {"id":1, "title":"html", "body":"html is ..."},
        {"id":2, "title":"css", "body":"css is ..."}
    ]
}

// POST
const URL = 'http://localhost:3000/topics';
const data = {id: 4, title: 'gimotti', body: '์ค๋ง์์ ๋ชจ ์ ๋ฐ์ด๋ฃจ..'};

response = await fetch(URL, {
        method: 'POST',
        headers: {
            'Content-Type': 'application/json',
        },
        body: JSON.stringify(data)
    });
result = await response.json
```

์ง๊ธ์ `POST`๋ง ๊ตฌํํ์ง๋ง ์ด์ฒ๋ผ `fetch` ํน์ `axios`๋ฅผ ์ด์ฉํด ๋ฐ์ดํฐ๋ฅผ `CRUD` ํ  ์ ์๋ค.

### โ ์ค์ต ๊ฐ์
1. `CI/CD`: `commit` ํ๋ฒ๋ง์ผ๋ก ์๋์ผ๋ก  `discord` ์ ์๋ฆผ ์ค์ ํ๊ณ  ๋ฐฐํฌ๊น์ง ํ๋ค. 
2. ํด๋น ์์ด์ฝ์ ๋ฐฐํฌ์ฉ์ผ๋ก ์ ํฉํ์ง ์๋ค๋ ๋ป, ๊ฐ๋ฐ์ฉ์ผ๋ก๋ง ์ฌ์ฉํ๊ธฐ

![](https://images.velog.io/images/abcd8637/post/8d63ca10-fb19-493c-ab7b-dae63589a436/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-18%2015.24.10.png)

3. `development`: ๋๋ฒ๊น ๋ฐ ๊ฐ๋ฐ ํ๊ฒฝ
4. `production`: ์ค์  ๋ฐฐํฌ ํ๊ฒฝ
5. `node.js`๋ก `development`๋ก ๋ฐฐํฌํ๋ค๋ฉด ์ค๋ฅ๊ฐ ์ด๋์์ ๋ฌ๋์ง ์ ์ ์๊ธฐ ๋๋ฌธ์ ๋ณด์์ ์ทจ์ฝํ๋ค
6. `front`์์ `development`๋ก ๋ฐฐํฌํ๋ฉด `production`๋ณด๋ค ๋๋ฆฌ๋ค. `development`์์๋ `warning`์ด ์ ๋ณด์ธ๋ค. ๋ฐ๋ฉด์, `production` ์์๋ `warning` ๊ฐ์๊ฒ์ด ๋จ์ง ์๋๋ค. `production`์ ๊ฐ๋ณ๋ค. ๊ฐ๋ฐ๋ชจ๋์ ๋ฐฐํฌ๋ชจ๋์ ์๋์ฐจ์ด๋ ์ฝ 4๋ฐฐ(2017๋ ๊ธฐ์ค)
7. `npm run build`๋ฅผ ์์ฑํ๋ฉด `production`๋ชจ๋๋ก `build` ํด์ฃผ๋๋ฐ, `build` ํด๋์์ ํ์ผ์ ํด๋ฆญํ๋ฉด ์ฝ๋๊ฐ ํ์ค๋ก ์์ฑ๋์ด ์ฝ๋๋ฅผ ์ฝ๊ธฐ ํ๋ค๋ค. 
8. `scripts` ๊ฐ์ฒด์์ ๋ช๋ น์ด๋ฅผ ์ฌ์ฉํ๋ ค๋ฉด `npm run`์ ์์ฑํ์
9. `serve -s build`: ๋ฐฐํฌ์ฉ ๋ฒ์  ํ์ธ

```javascript
// ๋ฐฐํฌ์ฉ์์๋ง ํ์ธ ํ  ์ ์๋ ์ฝ๋
if(process.env.NODE_ENV === "production"){
	console.log("ํ์ฌ Production ๋น๋๋ก ๋์๊ฐ๊ณ  ์์ด์!")
}
```

10. `<script src=""></script>`๋ก `js` ํ์ผ์ ๋ถ๋ฌ์ค๋ฉด `window`์ธ ์ ์ญ๊ฐ์ฒด์ ์์ฑ๋๋ฏ๋ก ๋์ค์ ์์ฑํ ํ์ผ์ด ์ด์ ์ ์์ฑํ ํจ์์ ๊ฐ์ ๋ณ๊ฒฝํ  ์๋ ์๋ค. ์ด๋ฅผ ๋ณด์ํ๊ธฐ์ํด `webpack`์ผ๋ก ๋ฒ๋ค๋งํ์ฌ ๋ณด๊ดํ๋ค.
11. `cloud`, `web hosting`: ๊ฐ์ธ์ ์ผ๋ก ์๋ฒ๋ฅผ ๋น๋ ค ์ด์ํ๋ฉด ๊ฐ๊ฒฉ์ด ๋น์(`VM`), ๋ฐ๋ฉด์, `heroku`์ ๊ฐ์ด `PasS`๋ฅผ ์ด์ฉํ์ฌ ์๋ฒ์ ์ผ๋ถ์์์ ์ด์ฉํ๋ ์์์ ์์ค์ฝ๋๋ฅผ ์ฌ๋ ค์ฃผ์ด ํ์ด์ง๋ฅผ ๋์ฐ๋ ์์์ด๋ผ ๋น์ฉ์ด ๋ค์ง ์๋๋ค. 
12. `AWS`: ์ ์ ์จ์ด ๋๊ณ , ๋งค์ฐ ์์ ์ ์ด๋ฉฐ ๋ค์ํ ๊ธฐ๋ฅ์ ์ ๊ณตํ์ง๋ง ๊ฐ๊ฒฉ์ด ๋น์ธ๋ค...
13. `oracle`, `google cloud`: ๊ฐ์์ ํ๋ฆฌํฐ์ด ๋ฌด๋ฃ ์ ๊ณต
14. `ํ๋ก ํธ๋ง ์ฉ์ผ๋ก ๋๋ฆฐ๋ค.`: `Github Page`, `Netlify`, `Vercel`
15. `Node.js`๋ ๋๋ฆฐ๋ค: ์๊ฐ์ ํ์ด ๊ด์ฐฎ๋ค๋ฉด `Heroku`
16. `Nginx`๊ฐ์ ์น ์๋ฒ๋ ๋๋ฆฌ๊ณ , ๋ค์ํ ์์์ ํ๋ค: `2G`, `1 Core`๋ก ์ถฉ๋ถ
17. `Docker`๋ ๋๋ฆฌ๊ณ  ์ถ๋ค: ์ต๋ `8G`, `4 Core`..
18. ์ค๋ฌผ์๋ฒ์ ๋จ์ : ๋ฐ์ดํฐ ๋ณต๊ตฌ์ ์ ์ฐจ๊ฐ ๊น๋ค๋กญ๋ค. 
19. `NGINX`(web server): http๋ฅผ ํตํด ์น ๋ธ๋ผ์ฐ์ ์์ ์์ฒญํ๋ HTML๋ฌธ์๋ ์ค๋ธ์ ํธ์ ์ ์กํด์ฃผ๋ ์๋น์ค ํ๋ก๊ทธ๋จ์ ๋งํ๋ค. `SSL`, `forward proxy`, `reverse froxy`, `cache`, `๋ก๋ ๋ฐธ๋ฐ์`, `์ ์ ์ด๊ณ  ๊ฐ๋ฒผ์ด ๋ฐ์ดํฐ ์ ๊ณต`์ ์ฌ์ฉํ๊ธฐ์ ์ ๋นํ๋ค.
20. `proxy-server`: ํด๋ผ์ด์ธํธ์ ์๋ฒ ์ค๊ฐ์์ ๋ฌด์ธ๊ฐ๋ฅผ ํด์ฃผ๋ ์๋ฒ
21. `reverse-proxy`: ํด๋ผ์ด์ธํธ๊ฐ ์์ฒญํ๋ฉด `Nginx`๊ฐ ๋์ ํด์ ์๋ตํด์ค๋ค. ์๋ฒ์ ๋ณด์์ ๋์ผ ์ ์๋ค
22. `Docker`: ํ ์๋ฒ์์ ์๋ก ๊ฐ์ ๋ ๊ฐ์ ์๋น์ค๋ฅผ ๋ง๋ค๋ ค๋ฉด? ์๋ฒ๋ฅผ ์ปจํ์ด๋๋ก ๋๋๋ค๋ฉด ๊ฐ๋ฐํ๊ฒฝ์ ๊ตฌ์ถํ๋ค๊ฐ ์ถฉ๋์ด ๋ฐ์ํ๊ฑฐ๋, ์์กด์ฑ์ด ๊ผฌ์ผ ํ์๊ฐ ์๋ค.(๊ฐ์ํ)
23. `CI(Continuous Integration) / CD(Continuous Deployment)`: ํตํฉ, ๋ฐฐํฌ๋ฅผ ์๋์ผ๋ก ํด์ฃผ๋ ๊ณผ์ , ๋จ์ํ๊ฒ ์ปค๋ฐ๋ง ํ๋ฉด ๋ฐฐํฌ๊น์ง ํ๋ฒ์ ๋๋ค. ์๋๋ `GitLab` ์ ๊ธฐ๋ฅ์ด์์ผ๋ `github` ์์  `github-action` ๋ฅผ ๋ง๋ค์ด ์ ๊ณตํ๋ค. ํ์์์ `Jenkins` ๋ฅผ ์ฃผ๋ก ์ฌ์ฉํ๋ค. `Jenkins` ๋ ๋ณ๋์ ์๋ฒ๋ฅผ ์๊ตฌํ๋ค. `Travis CI`: ์ํฉ์ ๋ฐ๋ผ ์ ๋ฃ์ธ์ ์ ๊ฐ์ํ๊ธฐ
24. `web-hook`: ํน์  ์ด๋ฒคํธ๊ฐ ๋ฐ์ํ์ ๋ ํ ์๋น์ค๋ ์์ฉํ๋ก๊ทธ๋จ์ผ๋ก ์๋ฆผ์ ๋ณด๋ด๋ ๊ธฐ๋ฅ(๋ค๋ฅธ ํ์์ด ์ปค๋ฐํ๋ฉด ํด๋น ์ฝ๋๋ฅผ ๋ฐ๋ก ๋ณผ ์ ์์)
25. `web-hook` ๋์ค์ฝ๋๋ก ์ค์ ํ๊ธฐ: ์๋ฒ ์์ฑ โ ์ด ์๋ฒ ์ค์  โ ์น ํํฌ โ URL ๋ณต์ฌ โ `github settings/webhook` โ `payloadURL`์ ๋ถ์ฌ๋ฃ๊ณ  ๋์ `/github` ๋ถ์ฌ์ฃผ๊ธฐ
26. `yml`: ๋ค์ฌ์ฐ๊ธฐ๋ฅผ ์ ๊ฒฝ์ฐ๋ ๋ฌธ๋ฒ
27. `git action` ๋น๋ ์ค ์ค๊ฐ์ ์๋ฌ๊ฐ ๋ฐ์ํ๋ฉด ๊ทธ ์ดํ์ ์์์ ์ํํ์ง ์๋๋ค.

---
## ๐ 62์ผ์ฐจ 1.19.์. ์จ๋ผ์ธ ๊ฐ์
์ค๋์ `SSR`๊ณผ `CSR`, ๊ฐ๋จํ๊ฒ `Next.js`๋ฅผ ์ฌ์ฉํ๋ ๋ฒ์ ๋ํด์ ๋ฐฐ์ ๋ค. ์ด์ ์ ๋ณ๊ณผํ์คํธ ํ๋ก์ ํธ๋ฅผ react๋ก ๊ตฌํ ํ๋ฉด์ SSR์ ๋ํด์ ๊ด์ฌ์ด ์๊ฒผ๋๋ฐ ์ด๋ฒ์ ๊น๊ฒ๋ ์๋์ด๋ ์๋ํ๋ ์๋ฆฌ, ๊ฐ๋จํ ์์ ๋ฑ์ ๋ฐฐ์ธ ์ ์์ด์ ์ข์๋ค.

### โ Server Rendering
1. React, Vue, Angular ๋ฑ ์๋ฐ์คํฌ๋ฆฝํธ ํ๋ ์์ํฌ๊ฐ ๋์ค๊ธฐ ์ด์  ์ด๊ธฐ ์น ํ๊ฒฝ์์๋ ๋ชจ๋  ํ์ด์ง๋ฅผ ์๋ฒ์์ ๋น๋
2. ํด๋ผ์ด์ธํธ๋ ๋ณ๋์ ์ฒ๋ฆฌ ์์ด ์นํ์ด์ง ๋ธ์ถ ์ด๋ฅผ, `Server Rendering` ์ด๋ผ๊ณ  ํจ

### โ Client Side Rendering
1. `Ajax` ๋ฑ์ ๊ธฐ์ , ์๋ฐ์คํฌ๋ฆฝํธ ํ๋ ์์ํฌ๋ฅผ ํ์ฉํ์ฌ, ๋ฐ์ดํฐ๋ฅผ ๋ฐ์ ์๋ฐ์คํฌ๋ฆฝํธ๋ก ํ์ด์ง๋ฅผ ๋์ ์ผ๋ก ๋ง๋ค ์ ์๊ฒ ๋จ(`XMLHTTPRequest`)
2. ๋ฐ์ดํฐ๋ `XML`, `JSON` ํํ๋ก ํด๋ผ์ด์ธํธ์ ์ ์กํ๋๋ฐ, ์ด๋ฅผ `CSR`์ด๋ผ๊ณ  ํจ

### โ CSR์ ์ฅ์ 
1. CSR์ ์๋ฐ์คํฌ๋ฆฝํธ๋ง์ผ๋ก ์์ ํ ํ์ด์ง๋ฅผ ๋ง๋ค ์ ์๋ค.
2. ์๋ฐ์คํฌ๋ฆฝํธ๋ฅผ ์ต๋ํ๋๋ก ํ์ฉํ์ฌ HTML, CSS๋ฅผ ๋์ ์ผ๋ก ์์ฑ
3. ์ปดํฌ๋ํธ ๋จ์๋ก ์ฝ๋๋ฅผ ๋๋๊ณ , ๋ค์ํ ๋์์ธ ํจํด์ ์ ์ฉํ๋ ๋ฑ ํด๋ผ์ด์ธํธ ๊ฐ๋ฐ์ ์์ค์ ํ ๋จ๊ณ ๋์ด์ฌ๋ฆผ.
4. Full page load ์์ด ๋ผ์ฐํ(ํ์ด์ง ์ด๋์ ๋งค๋ฒ ์๋ก๊ณ ์นจ์ ํ  ํ์๊ฐ ์์)

### โ CSR์ ๋จ์ 
1. `JS` ์ฝ๋๊ฐ ๋ง์ผ๋ฉด ์ฑ ๋ก๋ฉ์ด ๋๋ ค์ง
2. `SEO` ๊ฐ ์ข์ง ์์(๊ฒ์์์ง์ด ์์)
3. `crawler` ๋ ์๋ฒ์ ํ์ด์ง๋ฅผ ์์ฒญํ๊ณ  ์๋ฒ๋ HTML, CSS, JS๋ฅผ ๋ด๋ ค์ค ์ ์์ง๋ง `crawler` ๋ HTML๋ง์ ์ฝ์ด์ ํ์ด์ง์ ์ด๋ค ์ ๋ณด๊ฐ ์๋์ง ํ๋ณํจ `crawler` ๊ฐ HTML์ ์ฝ์ด์ ์ป์ ์ ๋ณด๋ฅผ DB์ ์ ์ฅํ๊ณ , ๋์ค์ user๊ฐ search engine์ ๊ฒ์ํ์ ๋ DB์์ ์ ๋ณด๋ฅผ ๊บผ๋ด๊ฒ ๋๋ค. CSR์ ๊ฒฝ์ฐ JS์์ ํ์ด์ง๋ฅผ ๋ง๋ค๊ธฐ ๋๋ฌธ์ ์ด๊ธฐ HTML์ ๋ด๋ ค์ค๋๋ ์ ๋ณด๊ฐ ๋ณ๋ก ์๋ค.

### โ SSR
1. ์๋ฒ์์ ์๋ฐ์คํฌ๋ฆฝํธ(`js engine`)๋ฅผ ์ด์ฉํด ํ์ด์ง๋ฅผ ๋ฏธ๋ฆฌ ๋น๋
2. ์ปดํฌ๋ํธ ์์ฑ์ ํ์ํ `API ์์ฒญ`, `routing`, `redux store` ์์ฑ ๋ฑ์ ์ฒ๋ฆฌ.
3. ํด๋ผ์ด์ธํธ๋ ๋น๋๋ ํ์ด์ง์ ์๋ฐ์คํฌ๋ฆฝํธ๋ฅผ ๋ฐ์ ์น์ฑ์ CSR์ฒ๋ผ ๋์ํ๊ฒ ํจ(`hydration`)
4. ์ด๋ฐ ํน์ง์ผ๋ก, `Universal Rendering`์ด๋ผ๊ณ ๋ ํจ
5. `server rendering` ์ `MPA` ๋ผ๊ณ ๋ ๋ถ๋ฆ.
6. CSR์ ์๋ฐ์คํฌ๋ฆฝํธ ํ๋ ์์ํฌ๋ฅผ ํ์ฉํ์ฌ, ๋ฐ์ดํฐ๋ฅผ ๋ฐ์ ์๋ฐ์คํฌ๋ฆฝํธ๋ก ํ์ด์ง๋ฅผ ๋์ ์ผ๋ก ๋ง๋ค ์ ์๊ฒ ๋๋ค.

![](https://images.velog.io/images/abcd8637/post/4befebbc-69ae-42ca-9a6d-d7bd41722b38/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-19%2010.52.09.png)

### โ SSR์ ์ฅ์ 
1. `Crawler`๋ ํ์ด์ง๋ฅผ `Indexing`ํ๊ธฐ ์ํด ํ์ด์ง์ ๊ดํ ๋ง์ ์ ๋ณด๊ฐ ํ์
2. `SSR`์ ํ์ฉํ์ฌ ๋ฏธ๋ฆฌ ํ์ด์ง๋ฅผ ๋น๋ํ๋ฉด, `Crawler`์๊ฒ ๋ง์ ์ ๋ณด๋ฅผ ์ค ์ ์์
3. `SEO`(Search Engine Optimization)์ ์ ๋ฆฌ

### โ SSR์ ๋จ์ 
1. `CSR`์ ๋นํด `TTFB(Time To First Byte)`์ ๋ถ๋ฆฌํจ(์๋ฒ์์ ๋ฏธ๋ฆฌ ๋น๋๋ฅผ ํ๊ณ  ์์ด์ผ ํ๊ธฐ ๋๋ฌธ, ์๊ฐ์ด ์ค๋๊ฑธ๋ฆฌ๋ฉด ์คํ๋ ค CSR๋ณด๋ค ๋๋ ค์ง ์ ์๋ค.)
2. ๋ณ๋์ ์๋ฒ๋ฅผ ์ ์งํ๋๋ฐ ๋น์ฉ(์ ์ ๊ฐ ๋ง์ ๊ฒฝ์ฐ ์๋ฒ๋ฅผ ์ฌ๋ฌ ๋ ์ ์งํด์ผํ  ์ ์์)์ด ๋ฆ
3. `CSR` ๋ณด๋ค `CDN Caching`์ ๋ถ๋ฆฌํจ(๊ฐ์ ์์ฒญ ์ `CDN`์ ์ง์  ์์ฒญํ  ์๋ ์์, ๋๋ฉ์ธ ๊ด๋ฆฌ ์๋ฒ์์ ์ง์  ์๋ฒ๋ก ์์ฒญํ ๊ฒ์ธ์ง CDN์ผ๋ก ์์ฒญ์ ๋ณด๋ผ ๊ฒ์ธ์ง ๊ด๋ฆฌ๋ฅผ ํ  ์ ์๋ค.)

### โ ์น ํผํฌ๋จผ์ค
1. ์น ํ์ด์ง๊ฐ ๋ก๋๋๊ณ  ์ ์ ์ ์ํธ์์ฉํ๋ ๋ชจ๋  ๊ฒ๋ค์ ์ธก์ 
2. ์ฑ๋ฅ์ ์ธก์ ํ์ฌ ์น์ฑ์ ์ฌ์ฉ์ฑ์ ๊ฐ์ ํ  ์ ์์
3. ์ด์ํ ๋คํธ์ํฌ ํ๊ฒฝ์์๋ ์ฌ์ฉ ๊ฐ๋ฅํ ์ฑ์ ๋ง๋๋ ๋ฑ ์ข์ ์ ์  ๊ฒฝํ์ผ๋ก ์ ์ ์ ๋ง์กฑ์ ์ป์
4. `Time To First Byte` , TTFB

```
1. ๋ธ๋ผ์ฐ์ ์์ ์๋ฒ๋ก ํ์ด์ง ์์ฒญ ํ ์๋ฒ๊ฐ ๋ธ๋ผ์ฐ์ ์๊ฒ ์ฒ์ ๋ฐ์ดํฐ๋ฅผ ์ ๋ฌํ  ๋ ๋์ฐฉํ๊ธฐ๊น์ง ๊ฑธ๋ฆฌ๋ ์๊ฐ
2. ์์ฒญ์ ๋ฐ์์ ๋, ์๋ฒ์์ ์ฒ๋ฆฌํ๋ ์๊ฐ์ด ์ค๋ ๊ฑธ๋ฆฌ๊ฑฐ๋, ๋คํธ์ํฌ๊ฐ ๋๋ ์ด๋๋ ๋ฑ์ ์ํฉ ๋ฐ์ ์ ์งํ๊ฐ ์ํ๋จ
3. ๋ธ๋ผ์ฐ์ ์ ์์ฒญ์ด ์๋ฒ๊น์ง ๊ฐ๋ ์๊ฐ
4. ์๋ฒ์์ ์์ฒญ์ ์ฒ๋ฆฌํ๋ ์๊ฐ
5. ์๋ฒ์์ ๋ธ๋ผ์ฐ์ ๊น์ง ์๋ต์ด ๊ฐ๋ ์๊ฐ
```

5. `First Contentful Paint`: FCP

```
1. ํ์ด์ง์ ์ง์ํ๊ณ ๋ถํฐ, ๋ธ๋ผ์ฐ์ ๊ฐ ์ด๋ค DOM Content๋ฅผ ๋ง๋ค ๋๊น์ง ๊ฑธ๋ฆฌ๋ ์๊ฐ
2. ํ์ด์ง ์ง์ ํ FCP(๋ญ๋ผ๋ paint๋๋ ์๊ฐ)๊น์ง ํ๊ท  3์ด ์ด์ ๊ฑธ๋ฆฌ๋ฉด ์ฑ๋ฅ ๊ฐ์ ์ด ํ์
3. ๋ธ๋ผ์ฐ์ ์์ HTML, CSS, JS ๋ฑ์ ํ์ฑํ๋ ์๊ฐ
4. ๋ธ๋ผ์ฐ์ ์์ ํ์ด์ง๋ฅผ ๊ทธ๋ฆฌ๋ ์๊ฐ
```

6. `Time to Interactive`: TTI

```
1. ์น ํ์ด์ง ์ง์ ํ, ์ ์ ๊ฐ ํด๋ฆญ, ์คํฌ๋กค, ์ธํ ๋ฑ์ ํ์๋ฅผ ํ๊ธฐ๊น์ง ๊ฑธ๋ฆฌ๋ ์๊ฐ
2. ์๋ฐ์คํฌ๋ฆฝํธ๊ฐ ๋ก๋๋๊ณ  ๋์, ์ด๋ฒคํธ ํธ๋ค๋ฌ ๋ฑ์ด ๋ถ์ฐฉ๋์ด ์๋ ฅ์ ์ฒ๋ฆฌํ  ์ ์๊ธฐ๊น์ง์ ์๊ฐ
3. JS๊ฐ ์ฒ๋ฆฌ๋์ด DOM์ ์ด๋ฒคํธ๋ฅผ ๋ถ์ฐฉํ๋ ์๊ฐ
```

### โ CSR, SSR์ ํ์ด์ง ๋ก๋๋ฐฉ์
1. ๋จผ์  CSR์ ํ์ด์ง ๋ก๋๋ฐฉ์์ ๋ค์๊ณผ ๊ฐ๋ค.

```
1. ๋ธ๋ผ์ฐ์ ์์ HTML์ ์์ฒญํ๋ค.
2. ์๋ฒ์์ HTML์ ์๋ตํ๋ค.(TTFB)
3. ๋ธ๋ผ์ฐ์ ์์ JS๋ฅผ ์์ฒญํ๋ค.(scriptํ๊ทธ๋ฅผ ๋ง๋๋ฉด)
4. JS ์๋ต
5. JS ์์ง์ผ๋ก ํ์ด์ง ๋น๋
6. data ์์ฒญ(axios, API ๋ฑ๋ฑ)
7. data ์๋ต
8. ํ์ด์ง ๋ก๋ ์๋ฃ(FCP, TTI)
9. CSR์ ๋ธ๋ผ์ฐ์ ์์ JS๋ฅผ ๋๊ณ  ๋ฆฌ๋ก๋ฉ์ ํ๋ฉด ๋ด์ฉ๋ฌผ์กฐ์ฐจ ๋ณด์ด์ง ์๋๋ค.
```

![](https://images.velog.io/images/abcd8637/post/62c5a210-dd2d-4dc3-8ebe-f3f6c83a1e0e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-19%2011.01.17.png)

2. SSR์ ํ์ด์ง ๋ก๋ ๋ฐฉ์

```
1. ๋ธ๋ผ์ฐ์ ๊ฐ HTML์ ์์ฒญํ๋ค.
2. ์๋ฒ์์ ํ์ด์ง๋ฅผ ๋น๋ํ๋ ์๊ฐ์ด ์์๋๋ค(CSR๊ณผ ๋ค๋ฅธ ๋ถ๋ถ), ๊ฒฝ์ฐ์ ๋ฐ๋ผ API ๋ฐ์ดํฐ ์์ฒญ, routing, redux store ์ฒ๋ฆฌ, dom ์์ฑ ๋ฑ
3. HTML ์๋ต(TTFB, FCP)
4. JS ์์ฒญ
5. JS ์๋ต
6. Rehydration(TTI): input, navBar๊ฐ ์๋ฒฝํ๊ฒ ๋์ํ์ง ์์(js๊ฐ ๋ชจ๋ ํ์ฑ๋๊ธฐ ์ ๊น์ง)
7. data ์์ฒญ
8. data ์๋ต
9. ํ์ด์ง ๋ก๋ ์๋ฃ
10. SSR์ ๋ธ๋ผ์ฐ์ ์์ JS๋ฅผ ๋๊ณ  ๋ฆฌ๋ก๋ฉ์ ํ๋ฉด ๋ด์ฉ๋ฌผ์ ๋ณด์ฌ๋ ๋์ํ์ง ์๋๋ค.
11. ์ ์ ๊ฐ ๋น ๋ฅด๊ฒ ํ์ด์ง์ ๋ด์ฉ์ ๋ณผ ์ ์๋๋ก HTML์ ๋ฏธ๋ฆฌ ๋น๋ํ์ฌ FCP๋ฑ์ ํค ๋ฉํธ๋ฆญ์ ๊ฐ์ ํ๋ค.
12. ์๋ฒ ์์์ ํ์ฉํ์ฌ, ์ด๊ธฐ ํฐ ์ฑ๋ฅ์ด ํ์ํ๊ฑฐ๋ ๋ด์ฉ์ด ๋ง์ ํ์ด์ง ๋ฑ์ ๋ฏธ๋ฆฌ ๋น๋ํ๋ ๋ฐ ํ์ฉํ๋ค. 
```

![](https://images.velog.io/images/abcd8637/post/171124ca-4102-4336-8676-340d17a6670e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-19%2011.05.05.png)

### โ React๋ฅผ ํ์ฉํ์ฌ SSR๊ตฌ์ถํ๊ธฐ
1. `ReactDOMServer`๋ฅผ ํ์ฉํ์ฌ, ํน์  `React Component`๋ฅผ ๊ฐ์์ DOM์์ HTML๋ก ๋น๋
2. `Node.js` ์๋ฒ์์ `JSX`๋ฅผ ์ฌ์ฉํ์ฌ ํ์ด์ง ๋น๋

```
1. `renderToString`: `React component`๋ฅผ `HTML`๋ก ๋ณํ, ํ๊บผ๋ฒ์ ๋ชจ๋  ํ์ด์ง๋ฅผ ๋ง๋ค์ด์ ๋ฆฌํดํ๊ธฐ ๋๋ฌธ์ ๋ธ๋ผ์ฐ์ ๊ฐ ๊ธฐ๋ค๋ ค์ผํ๋ค.(`ReactDOMServer.renderToString(<App />)`)
2. ํด๋ผ์ด์ธํธ์ ํ์ด์ง ์์ฒญ ์, ๋ณํ๋ HTML string์ ์ ๋ฌ
3. `renderToNodeStream`์ DOM์๋ฒ๊ฐ ์กฐ๊ธ์ฉ ํ์ด์ง๋ฅผ ๋ง๋ค์ด์ `readable stream` ์ ์ ๋ฌํจ.๋ธ๋ผ์ฐ์ ๊ฐ ๋ฐ์์ ์ ์ง์ ์ผ๋ก ํ์ด์ง๋ฅผ ๋ถ๋ถ์ ์ผ๋ก ๋ณด์ฌ์ค ์ ์์
4. ReactDOM.hydrate: CSR์์ ๋์ํ๋ ๊ฐ์ฒด, renderToString์ผ๋ก ์์ฑํ HTML์ root๋ฅผ ๊ธฐ์ค์ผ๋ก, ๋ฐ์์จ React code๋ฅผ ํตํด markup์ ์ด๋ฒคํธ ํธ๋ค๋ฌ๋ฅผ ๋ฑ๋กํ๋ ๋ฑ ์ปดํฌ๋ํธํ
5. Hydration ์ ์ฃผ์ํ  ์ 
  - ์๋ฒ์์ ์์ฑํ ์ปดํฌ๋ํธ์ ๋ธ๋ผ์ฐ์ ์์ Hydration์ ๊ฑฐ์น ํ์ ๋งํฌ์์ด ๋ค๋ฅด๋ฉด, React runtime์ ๊ฒฝ๊ณ ๋ฅผ ๋ณด๋ (ex, ํ์ฌ ์๊ฐ์ ๋ณด์ฌ์ฃผ๋ ์ปดํฌ๋ํธ)
  - ๊ฒฝ๊ณ  ๋ฐ์ ์, ์ด๋ ๋ถ๋ถ์์ ์ฐจ์ด์ ์ด ์๊ธฐ๋์ง ๋ฐ๋์ ํ์ํด์ผ ํจ
  - componentDidMount ์ญํ ์ ํ๋ useEffect์ ๊ฒฝ์ฐ, SSR์ ์๋ฒ์์ ๋์ํ์ง ์์, ์ด๋๋ getInitialProps๋ก ์ด๊ธฐ ๋ฐ์ดํฐ๋ฅผ ์ฑ์ด ๋ค์์ ํ์ด์ง๋ฅผ ๋ณด๋ด๋ ๋ฐฉ๋ฒ์ ์ฌ์ฉํ  ์ ์๋ค.
  - data loading ๋ฑ์ ์ฒ๋ฆฌ๋ฅผ ๋ณ๋๋ก ํด์ฃผ์ด์ผ ํ  ํ์๊ฐ ์์
```
6. ์ค์ต1: div root ๋ด๋ถ์ html ์ปดํฌ๋ํธ ์์ฑ: <a href='https://github.com/YWTechIT/ssr-with-react-node-practice'>github</a>
7. ์ค์ต2: next.js router ํด๋ณด๊ธฐ: <a href='https://github.com/YWTechIT/next-js-init-practice'>github</a>

### โ React ์ฑ ๋ฐฐํฌ overview
1. ์ธํฐ๋ท์์ ๋ด๊ฐ ๋ง๋  ์ฑ์ ์ ๊ทผํ  ์ ์์ด์ผ ํจ
2. ์ง์์ ์ผ๋ก ์ฑ์ ์์ ํ๊ณ  ๋ฐฐํฌํด์ผ ํจ(bug, feature ๋ฑ...)
3. Public IP ์ฃผ์ ํน์ DNS๋ก ์ง์  ์ ๊ทผํ  ์ ์๋๋ก ํจ

![](https://images.velog.io/images/abcd8637/post/690b688d-f9ac-4589-9689-915c58033ec9/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-19%2014.37.25.png)

4. ์๋ฒ์ ํต์ ์, CORS๊ฐ ํ์ฉ๋์๋์ง ์ ๊ฒ
5. ๋ธ๋ผ์ฐ์ , ๋๋ฐ์ด์ค๋ณ๋ก ์ฑ์ด ์ ์์ ์ผ๋ก ๋์ํ๋์ง ์ ๊ฒ
6. ์ฑ์ ๋ก๋ฉ ์๋, ๊ฐ ๋์ ์ ์ฑ๋ฅ, ๋ฒ๊ทธ ๋ฑ์ ์ ๊ฒ
7. IP๋ฅผ ๋ถ์ฌ๋ฐ์ ์๋ฒ(VM)์ React์ฑ์ ๋ฐฐํฌ โ ์ฑ์ ๋น๋ํ๊ณ , ์น์๋ฒ๋ฅผ ์ธํ โ ์ฑ์ ์๋นํ๋ ์น์๋ฒ๋ฅผ ํตํด ์ฌ์ฉ์์๊ฒ ์ฑ์ ์ ๋ฌ โ ์ฌ์ฉ์๋ ํ์ํ ๋ฐ์ดํฐ๋ฅผ ๋ฐ์ ์ฑ์ ๋ก๋ฉ

```
git clone ${url}
cd ${project_name} 
npm i 
sudo npm i -g serve  # build ํ ๊ฐ๋จํ ์น์๋ฒ๋ฅผ ๋์์ค
npm run build
sudo -s(serve) -p(port) 80 build(directory)  # serve ์น ์๋ฒ๋ฅผ ์ฌ์ฉํด ํ๋ก์ ํธ๋ฅผ 80๋ฒ ํฌํธ์์ ์๋นํจ
```

### โ React ์ฑ ์ค๋น
1. `yarn.lock`, `package-lock.json` ์ด ๋์์ ์กด์ฌํ์ง ์๋์ง ์ ๊ฒ(npm๊ณผ Yarn dependency๊ฐ ์ถฉ๋์์ build๊ฐ ์คํจํ  ์ ์์)
2. ๋ก์ปฌ์์ `npm run build` ๋ฅผ ์คํํ์ฌ, ๋น๋ ์ ์๋ฌ๊ฐ ๋ฐ์ํ์ง ์๋์ง ์ ๊ฒํ์.(๋ก์ปฌ์์ ๋น๋์ ์๋ฌ๊ฐ ๋ฐ์ํ๋ฉด ์๋ฒ์ ๋ฐฐํฌํ์ ๋์๋ ์๋ฌ๊ฐ ๋ฐ์ํ  ์ฌ์ง๊ฐ ์๋ค.)
3. ๋ก์ปฌ์์ ๋ฐฐํฌํ์ฌ, `production build` ๊ฐ ์ ๋๋ก ์คํ๋๋์ง ์ ๊ฒํ๊ธฐ.

### โ Gitlab ์ฐ๋
```bash
> git remote add origin ${git repository url}
> git push --set-upstream origin master
```

---
## ๐ 63์ผ์ฐจ 1.20.๋ชฉ. ์ค์๊ฐ ๊ฐ์
์ค๋์ ํ์์ผ์ ๋ฐฐ์ ๋ `CI/CD`, `github-actions`, `Heroku`, ๊ทธ๋ฆฌ๊ณ  ๋ฐฑ์๋ ์๋น์ค๋ฅผ ๊ตฌ์ถ ํ  ๋ ์๋ฒ ์ธํ๋ผ ๊ตฌ์ถ์ ์ฝ๊ฒ ํ  ์ ์๋๋ก ๋์์ฃผ๋ `firebase`์ ๋ํด์ ๋ฐฐ์ ๋ค. ์ด ๊ฐ์๋ฅผ ๋ฃ๊ธฐ ์ ์ `CI/CD` ๊ด๋ จํ ๋ด์ฉ์ ๋ดค์ ๋ ์ ๊ฒ ๋์ฒด ์ ํ์ํ์ง? ๋ผ๋ ์๊ฐ์ด ๋ค์๋๋ฐ, ์ง์  ํด๋ณด๋๊น ์๋ํ ๊ตฌ์ถ์ด ์ฃผ๋ ํจ๊ณผ๋ ๊ต์ฅํ๋ค!! `CI/CD`๋ฅผ ๋ฐฐ์ ์ง๋ง ์ฌ๊ธฐ์ ๊ทธ์น์ง ์๊ณ  ๋ด๊ฐ ์ง์  ํ๋ก์ ํธ๋ฅผ ๋ง๋ค ๋ ์ฌ์ฉํ  ์ ์์ ์ ๋๊น์ง ๊ณต๋ถํ๊ณ  ์ถ๋ค๋ ์๊ฐ์ด ๋ค์๊ณ  `firebase`๊ฐ ๋ฌด์์ธ์ง ๋ฐฐ์ฐ๋ฉด์ `Authentication`, `NoSQL`, `Storage`, `Hoisting`์ ์ ์ฉํด๋ณด๊ณ  ์ถ๋ค๋ ์๊ฐ์ด ๋ค์๋ค. ๊ฐ๋์ ์๋ก ๋ฐฐ์ธ ๋๋ง๋ค ์ด๋ก ์์ ๊ทธ์น์ง ์๊ณ  ์ด๋ป๊ฒ ์ค์ ์ ์จ๋จน์ด ๋ด๊ฒ์ผ๋ก ๋ง๋ค๊น ์๊ฐํ์ง๋ง, ๋ฐฐ์ด๋ด์ฉ์ด ๋ง์์ ํ๊บผ๋ฒ์ ์ ์ฉํ๋ ค๋๊น ๋ฒ๊ฑฐ์ ๋ค. ์ฒ์ฒํ ํ ๊ฐ๋์ฉ ์ ์ฉํ๋ค๋ณด๋ฉด ์ธ์  ๊ฐ ์์ ์ต์ง ์์๊น? 

1. `react` ๊ฐ๋ฐํ๊ฒฝ์์ `proxy` ๋ฅผ ์ฐ๋ ์ด์ 

```js
 1. ์ ๋๊ฒฝ๋ก(ex `https://www.example.com/todos`) ๋์  proxy๋ฅผ ์ฌ์ฉํ์ฌ ์๋๊ฒฝ๋ก(`/todos`)๋ก ์์ฒญํด๋ React์์๋ ์๋ฌ๊ฐ ๋์ง ์๋๋ค.
  * ์๋๊ฒฝ๋ก๋ก ์์ฑํ๋ฉด ๋์ค์ URL์ด ๋ฐ๋ ๋ ์ผ์ผ์ด ๋ฐ๊พธ๋ ๊ฒ๋ณด๋ค package.json์์ URL๋ง ๋ฐ๊พธ๋ฉด ๋ชจ๋ ์ ์ฉ๋๋ฏ๋ก ๊ฐํธํ๋ค.
 2. ์๋ฅผ ๋ค์ด, ๋ธ๋ผ์ฐ์ ๋ `localhost:8080`์ด๊ณ  ์๋ฒ์์ ๋ฐ์ดํฐ๋ฅผ ๋ฐ์์ค๋ URL์ `localhost:8888/todos` ๋ผ๋ฉด, ์๋๊ฒฝ๋ก๋ฅผ '/todos'๋ก ์์ฑํ์ ๋ react๋ ๋ธ๋ผ์ฐ์  ์๋ฒ์ธ `localhost:8080/todos`๋ก ์์ฒญํ๊ฒ ๋๋ค. ๋ถ๋ช ํด๋น ์ฃผ์๋ ๊ฐ์ด ์๊ธฐ๋๋ฌธ์ ์๋ฌ๋ฅผ ๋ด์ง๋ง, `package.json`์ `proxy`๋ฅผ ๋ณด๊ณ  react๊ฐ `proxy(์ค๊ณ)`์ญํ ์ ๋์ ํ๋ค. ๋ฐ๋ผ์ `localhost:8888/todos`๋ก ์์ฒญํ๊ฒ ๋๊ณ  ํด๋น ์ฃผ์์ ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ ธ์ฌ ์ ์๊ฒ ๋๋ค.
  * ์ด์ ๊น์ง๋ `๋ธ๋ผ์ฐ์  <-> react`, `๋ธ๋ผ์ฐ์  <-> ๋ฐฑ์๋`์ ํต์ ์ ์ง์ํ์ง๋ง, react๊ฐ `proxy(์ค๊ณ์๋ฒ)`์ญํ ์ ํ๋ฉด์ `๋ธ๋ผ์ฐ์  <-> react <-> ๋ฐฑ์๋` ์์ผ๋ก ํต์ ์ ํ๊ฒ๋๋ค.
 3. ์ด๋ ๊ฒ ํต์ ํ  ๋์ ์ฅ์ ์ `CORS`์ ์ ์ฉ๋์ง ์๋๋ค๋ ์ ์ด๋ค. (์๋ฒ์ ์๋ฒ๊ฐ์๋ `SOP`๊ฐ ์ ์ฉ ๋์ง ์๋๋ค. ๊ทธ๋ ๊ธฐ ๋๋ฌธ์ ๋ฐฑ์๋์์ ๋ฐ์ดํฐ๋ฅผ `react`๋ก ๊ฐ์ ธ์ค๊ณ  `react`๋ `browse`r๋ก ๊ฑฑ์ ์์ด ๋ฐ์ดํฐ๋ฅผ ๋ฟ๋ ค ์ค ์ ์๊ฒ ๋๋ค.)
```

2. `mui.com(material UI)`: ๋์์ธ ์์คํ์ ์ ๊ณตํ๋ React UI Framework
3. `npm install @mui/material @emotion/react @emotion/styled`
4. `git reset --hard hash`: ํด๋น ์ปค๋ฐ์ผ๋ก ์ด๋

### โ ์ค์ต
1. <a href='https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions#overview'>Git Actions</a>
2. CI(Continous Intergration): ํตํฉ์ํค๋๋ฐ ์ด์ 
3. CD(Continous Deployment): ๋ฐฐํฌํ๋๋ฐ ์ด์ 
4. `Github - actions`:  ๋น๋, ํ์คํธ ๋ฐ ๋ฐฐํฌ ํ์ดํ๋ผ์ธ์ ์๋ํํ  ์ ์๋ `CI/CD`(์ง์์  ํตํฉ ๋ฐ ์ง์์  ์ ๋ฌ) ํ๋ซํผ. `PR` ํน์ `Merge` ์ ๊ฐ์ ์ด๋ฒคํธ๊ฐ ์ผ์ด๋  ๋ workFlow๋ฅผ ํธ๋ฆฌ๊ฑฐ ํ  ์ ์๋ค. ๊ฐ ์์์ ์์ฒด ๊ฐ์ ๋จธ์  ์คํ๊ธฐ ๋ด๋ถ ๋๋ ์ปจํ์ด๋ ๋ด๋ถ์์ ์คํ๋๋ฉฐ, ์ฌ์ฉ์๊ฐ ์ ์ํ ์คํฌ๋ฆฝํธ๋ฅผ ์คํํ๊ฑฐ๋ ์์์ ์คํํ๋ ํ๋ ์ด์์ ๋จ๊ณ๊ฐ ์๋ค.
5. `workFlow`: ํ๋ ์ด์์ ์์์ ์คํํ๋ ์๋ ํ๋ก์ธ์ค, `YAML` ์ผ๋ก ํ์ผ์ ์์ฑํ๋ฉฐ, PR, merge์ ๊ฐ์ ์ด๋ฒคํธ, ์๋ ์ค์ , ์ค์ผ์ฅด์ ์ํด ํธ๋ฆฌ๊ฑฐํ๊ฒ ์ค์ ํ  ์ ์๋ค.

![](https://images.velog.io/images/abcd8637/post/060f2c32-0f94-49cf-8344-8d84facddffe/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-20%2015.12.36.png)

6. ๋จ๊ณ๋ณ๋ก ๋๋ ์ `build` ํ  ๋๋ ๋๋ฆฝ๋ ํํ๋ก `build` ํ๋ค.

```yaml
name: first-CI-practice  # ์ด๋ฆ: ์ดํ์ CI๊ฐ ๋์ํ๋ ๊ณผ์ ์์ ์ด๋ฆ์ผ๋ก ๋ฌ๋ค.

on:  # ์ด๋ค ๊ฒฝ์ฐ์ ์๋ ๋์์ ์ํํ  ๊ฒ์ธ๊ฐ?
  push:  # code push ํ  ๋
    branches: [ master ]
  pull_request:  # code PR ํ  ๋
    branches: [ master ]

jobs:  # ์ค์  ๋์

  build:  # ๋์์ ์ด๋ฆ(๋ฐ๊ฟ๋ ๋จ), ์ฒซ๋ฒ์งธ CI
    runs-on: ubuntu-latest  # ์ฐ๋ถํฌ ์ต์  ๋ฒ์  ์ ์ฉ
    strategy:  # ๋งค๊ฐ๋ณ์ ๋ค์ด๋ฐ์ ์ฌ์ฉ
      matrix:
        node-version: [12.x, 14.x, 16.x]
        # See supported Node.js release schedule at https://nodejs.org/en/about/releases/

    steps:  # ์ค์ ๋ก ๋์๊ฐ๋ ๋์
    # '-'๋ ๊ฐ๊ฐ์ ๋์์ ์๋ฏธํจ.
    - uses: actions/checkout@v2  # ํ๋ฌ๊ทธ์ธ ์ฌ์ฉ, ์ํฌํ๋ก๊ฐ ์คํ๋  ๋๋ง๋ค ์ฒดํฌ์์ ์์์ ์ฌ์ฉํ๋ค.
    - name: Use Node.js ${{ matrix.node-version }}
      uses: actions/setup-node@v2
      with:
        node-version: ${{ matrix.node-version }}
        cache: 'npm'
    - run: npm ci
    - run: npm run build --if-present
    - run: npm test

	test:  # ๋๋ฒ์งธ CI
	  runs-on: ubuntu-latest
		needs: build  # build ๋จ๊ณ ์ดํ ์คํ
	  strategy:
	    matrix:
	      node-version: [12.x, 14.x, 16.x]
	
	  steps:
	    - uses: actions/checkout@v2  # ํ๋ฌ๊ทธ์ธ ์ฌ์ฉ
	    - name: Use Node.js ${{ matrix.node-version }}
      uses: actions/setup-node@v2
      with:
        node-version: ${{ matrix.node-version }}
        cache: 'npm'
	    - run: npm ci
	    - run: npm run build --if-present
	    - run: npm test
```

7. `actions/cache`: `actions`์ ์์กด์ฑ์ ๋งค๋ฒ ์๋ก ์์ฑํ๊ฑฐ๋ ๋น๋ํ ๊ฒฐ๊ณผ๋ฌผ์ ๋ค๋ฅธ๋ฐ์ ์ฌ์ฉํ๊ณ  ์ถ๋ค. 
8. `yml` ๋ก ํ์ผ์ ๋ง๋ค๊ณ  ์์ (์ฐํ)๋ฒํผ์ ๋๋ฅด๋ฉด `marketplace` ๊ฐ ๋ฌ๋ค. ์ฌ๊ธฐ์ ์ํ๋ `CI/CD` template๋ฅผ ๊ฐ์ ธ ์ฌ ์ ์์
9. `Heroku`

```js
1. ์ ๋ฝ๋ณด๋ค ๋ฏธ๊ตญ์ด ํํ์์ ๋ฐ๋ก ์ง๋  ์ ์์ด์ ์๋๊ฐ ์กฐ๊ธ ๋ ๋น ๋ฅด๋ค.
2. Heroku๊ฐ cloud์ ๊ธฐ๋ฅ์ ๋์  ํด์ค(Load balance, Auto scaling ๋ฑ...)
3. Heroku CLI: git <-> heroku, git Action์ ์ธ ์ ์์
4. Github Action + Heroku plugin
5. Github Actions์์ heroku_api_key๋ ๊ทธ๋๋ก commitํ์ง ๋ง๊ณ  secret์ ๋ฃ์ด์ ${{secrets.api_key}}๋ก ์ฌ์ฉํ์ ๋์  actions์ ํ๋ฒ secret์ ์๋ก๋ํ๋ฉด ์์ฑ์์กฐ์ฐจ ๋ฌด์จ ๊ฐ์ธ์ง ๋ค์ ๋ณผ ์ ์๋ค.
6. ๊ฐ๋ฐ -> commit -> Github -> Action -> Test -> Heroku
7. ๊ฐ๋ฐ -> commit -> P/R -> Test(์ฝ๋๋ฆฌ๋ทฐ) -> build -> deployment
8. actions๋ฅผ ์ฌ์ฉํ๋ ํฐ ์ด์ : ๊ฐ์ข ํ์คํธ๋ก ์ ์์ ์ผ๋ก ๋ฐฐํฌ ํ  ์ ์๋ ์ํ์ธ์ง ํ์ธํ  ์ ์๋ค. ํน์ ์ํฉ์์ ๋ฐฐํฌ, ์ถ๊ฐ์ ์ธ ๋ช๋ น์ด ์ค์  ๋ฑ ์ํ๋์กฐ๊ฑด์์ ๋ฐฐํฌ ํ  ์ ์๊ฒ๋ ์ปค์คํฐ๋ง์ด์ง์ด ๊ฐ๋ฅํ๋ค.

- name: Generate.env file
  run: |
      echo "DISCORD_TOKEN=$DISCORD_TOKEN" >> .env
      echo "WEATHER_API_KEY=$WEATHER_API_KEY" >> .env
    env:
      DISCORD_TOKEN: ${{ secrets.DISCORD_TOKEN }}
      WEATHER_API_KEY: ${{ secrets.WEATHER_API_KEY }}
```

9. `firebase`: ๊ธฐ๋ณธ์ ์ธ ์๋น์ค ๊ตฌ์ถํ๊ธฐ ์ํ ์๋ฒ ์ธํ๋ผ ๊ตฌ์ถ, ์๋ฒ๋จ ์ธํ ๋ฑ์ ๊ณ ๋ฏผํ์ง ์๊ณ  ํด๋ผ์ด์ธํธ ๋จ์ ์์๋ง ์งํํ์ฌ ์๋น์ค๋ฅผ ์ ์ํ  ์ ์๋ ํ๋ซํผ, ์ ํต์ ์ธ ์๋ฒ ๊ตฌ์ฑ์ฒ๋ผ ๋งค๋ฒ ์๋ฒ - DB๋ฅผ ๋๋์ด ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ ธ์์ ๊ด๋ฆฌํด์ผํ๋ ๋ถํธํจ์ ๋์ ์์. `Baas(Backend as a Service)`, `RealTimeDB`, `Cloud Firestore(NoSQL DB)`, `Storage`, `OAuth`, `Hosting`, `CDN`, `Cloud Functions` ๋ฑ ์ง์ํ๋ ๊ธฐ๋ฅ์ด ์๊ฐ๋ณด๋ค ๋ง๋ค. ๋ฐฑ์๋๋ฅผ ๊ด๋ฆฌํ  ํ์์์ด ํด๋ฆญ ๋ช๋ฒ์ผ๋ก ์๋ฒ๋ฅผ ๊ด๋ฆฌํ  ์ ์๋ค.
10. `npm i firebase`, `npm i -g firebase-tools`
11. `firebase login`
12. `firebase deploy`
13. `firebase ์ฌ์ฉ ์์ ์ฝ๋`

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
## ๐ 64์ผ์ฐจ 1.21.๊ธ. ์จ๋ผ์ธ ๊ฐ์
์ค๋์ `CSS Module`, `UI Framework`, `CSS framework`, `CSS-in-JS`, `Styled-components`์ ๋ํด์ ๋ฐฐ์ฐ๊ณ  ์ ๋ฐ์ ์ธ ์ฌ์ฉ ์ญ์ฌ(?)์ ๋ํด์ ๋ฐฐ์ ๋ค. ๊ธฐ์กด์ ์ฌ์ฉํ๋ ๋ฐฉ์์ ๋จ์ , ๋ถํธํจ ๋๋ฌธ์ ์๋ก์ด ๋ฐฉ์์ด ๋์๊ณ , ์๋ก์ด ๋ฐฉ์์์ ์๊ฒจ๋ ๋จ์ , ๋ถํธํจ์ ํตํด ์๋ก์ด ๋ฐฉ์์ ์ฌ์ฉํ๊ณ .. ์ด๋ ๊ฒ ์ผ๋ จ์ ๊ณผ์ ๋ค์ ๋ฐฐ์ฐ๋๊น ์ดํด๊ฐ ์ ๋๋ค. ๊ทธ๋ฆฌ๊ณ  ํ์์ ๊ด์ฌ์๋ ๋ฆฌํฉํ ๋ง์ ๋ํด์๋ ๋ฐฐ์ ๋๋ฐ ์ผ๋ จ์ ๊ณผ์ ๋ค์ ๋ณด๋ฉด์ ๋ฆฌํฉํ ๋ง์ `before / after`๋ฅผ ๋ณด๋ฉฐ ๊ฐ๋์ฑ์ด ์ด๋ป๊ฒ ์ฆ๊ฐ๋์๋์ง ํ๋ฒ ์ดํด๋ณด์. ๋ง์ง๋ง์๋ `figma`์ ์กฐ์๋ฒ์ 3๊ฐ์ง์ ๋๋ง ์์ฑํ๋ค. ํ๋ฒ ์ดํด๋ณด์.

### CSS Module
1. ๊ธฐ์กด `CSS`์ ๋จ์ : ํ๋์ ์คํ์ผ `sheet`๊ฐ ์ฌ๋ฌ ์ปดํฌ๋ํธ์ ์ํฅ์ ๋ฏธ์น๋ค.
2. CSS module์ ์ฌ์ฉํ๋ฉด `class`, `id` ๋ฑ ์ ํ์๊ฐ ๊ฒน์น  ์ฐ๋ ค๊ฐ ์์ (`hash`๊ฐ ์ฌ์ฉ)
3. ์คํ์ผ ์ถฉ๋์ ๋ฐฉ์งํ๊ณ  ์ฝ๋๋ฅผ ๊ฒฉ๋ฆฌํ์ฌ ์ฒด๊ณ์ ์ผ๋ก CSS ์ค๊ณ๊ฐ ๊ฐ๋ฅ
4. CSS module์ ๋จ์ ์ ๊ฐ๋ฐ์๊ฐ ์คํ์ผ๋ง์ ์ง์  ํ๋ํ๋์ฉ ํด์ผํ๋ค๋ ์ ์ด๋ค. 

```javascript
// App.jsx
import styles from "./app.module.css";

export default function App(){
	return(
		<div>
			<h1 className={ styles.title }>Pink Hello world</h1>  // hash๊ฐ ๋ถ์ด์์
			<h1 className={ "title" }>Hello world</h1>  // ๊ทธ๋ฅ title
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
1. ์ข๋ฅ: `MUI(material UI)`, `Ant design`
2. ์ฅ์ ์ ์ด๋ฏธ ๋ง๋ค์ด์ ธ ์๋ ์คํ์ผ์ด๊ธฐ ๋๋ฌธ์ ๊ฐํธํ๊ณ  ์ฝ๊ฒ ์ฌ์ฉํ๊ธฐ ์ข๋ค.
3. ๋จ์ ์ผ๋ก๋ ์ด๋ฏธ ๋ค ๋ง๋ค์ด์ ธ ์๊ธฐ ๋๋ฌธ์ styling์ ํ์ต ๋ฐ ํ๋ จ์ด ํ์ํ ์ด์ฌ์๋ค์๊ฒ๋ ๋น์ถ์ฒํ๋ค. ๋ํ ํด๋น framework์ ๋์์ธ์ฒ ํ์ ๋ฒ์ด๋๊ธฐ ์ฝ์ง ์๊ณ , ์ปดํฌ๋ํธ๋ค์ ์ปค์คํฐ๋ง์ด์งํ๊ธฐ ์ด๋ ค์

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
1. ์ข๋ฅ: `Tailwind CSS`, `w3.css`
2. ๊ฑฐ๋ํ CSS ํ์ผ ํ๋๋ฅผ ๊ฐ์ ธ์ค๋ ๊ฒ
3. ์ฅ์ : ๊ฐ๋ฐ์๊ฐ ๋ฐ๋ก CSS ํ์ผ์ ์์ฑํ์ง ์์๋ HTML์ ํด๋์ค๋ง ์ ์ด์ฃผ๋ฉด ์ ํด์ง ๊ท์น๋๋ก ์คํ์ผ๋ง์ด ์ ์ฉ๋จ.
4. ๋จ์ : CSS์ ๋ํ ์ดํด๋ ฅ์ด ์์ด๋ ํด๋น framework๋ฅผ ์ฌ์ฉํ๊ธฐ ์ํ ํ์ต์ ๋ ๋ค์ ํด์ผํจ, ์ด๋ฏธ ๋ค ๋ง๋ค์ด์ ธ ์์ด์ styling์ ํ์ต ๋ฐ ํ๋ จ์ด ํ์ํ ์ด์ฌ์๋ค์๊ฒ๋ ๋น์ถ์ฒ

```javascript
// W3CSS ์์
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
1. ์ข๋ฅ: `Styled-components`, `emotion`
2. ๋ฐ๋ก CSS ํ์ผ์ ๋ง๋ค์ง ์๊ณ  JSX ํ์ผ ์์์ ์คํ์ผ๋ง๊น์ง ํด๊ฒฐ ๊ฐ๋ฅํจ
3. ์ปดํฌ๋ํธ ์ฌ์ฌ์ฉ์ฑ์ด ์ฌ์์ง
5. JS ๊ฐ์ props๋ก ๋๊ฒจ์ค์ ํด๋น JS ๊ฐ์ ์๋๋ styling์ ๋ฐ๋ก ์ ์ฉํ  ์ ์๋ค.
6. class ์ด๋ฆ์ hash๊ฐ์ ์์ฑํ์ฌ ์ ํ์ ์ด๋ฆ์ด ๊ฒน์น  ์ฐ๋ ค๊ฐ ์๋ค.
7. ์คํ์ผ๋ง์ ๊ฐ๋ฐ์๊ฐ ์ง์  ํด์ผํจ

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

### โ ๊ธฐ์กด CSS ๋ฌธ๋ฒ์ SCSS๋ก ๋ฆฌํฉํ ๋งํ๊ธฐ
๋ฆฌํฉํ ๋งํ๋ฉด์ ๋๋๊ฒ์ด์ง๋ง `SCSS`๋ก ์์ฑํ์ ๋์ ์ฅ์ ์ ์ฝ๋๋ฅผ ๊ณ์ธต์ ์ผ๋ก ์์ฑํ  ์ ์๋ค๋ ๊ฒ์ด์๋ค. ๋ฐ๋ผ์, ๋ถ๋ชจ - ์์๊ฐ์ ๊ด๊ณ๋ฅผ ์ฝ๋๋ฅผ ํตํด ์ ์ถ ํ  ์ ์์๊ณ , ๋์ผํ ์ ํ์๋ฅผ ๋ถํ์ํ๊ฒ ์ฌ๋ฌ๋ฒ ์ฌ์ฉํ  ํ์์์ด `&`์ผ๋ก ๋์ฒดํด์ ์ฌ์ฉํ๊ฑฐ๋, ํ์ฌ ์ ํ์ ์ด์ธ์ ๋ค๋ฅธ ์ ํ์๋ง ์ฌ์ฉํ๋ ๋ฑ ๊ฐํธํ๊ฒ ์ฌ์ฉํ๋ ์ ์ด ์ข์๋ค.

```scss
/* ๊ธฐ์กด CSS ๋ฌธ๋ฒ */
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

/* SCSS ๋ฆฌํฉํ ๋ง */
/* ์ด๋ค ํด๋์ค์์ ์ข์๋์ด์๋์ง ๊ณ์ธต์ ์ผ๋ก ํ์ธ์ด ๊ฐ๋ฅํ๋ค. 
๋์ผํ ์ ํ์๋ ์ ๊ฑฐํ๊ณ  &๋ก ๋์ฒด ํ  ์ ์๋ค. ๊ฐ๋์ฑ์ด ์ฆ๊ฐํ๋ ํจ๊ณผ๊ฐ ์์ */
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

### โ JavaScript template literal
1. ๋ฌธ์์ด ์์์ JS ํํ์์ ์ฌ์ฉํ  ์ ์๊ฒ ํ๋ ๋ฌธ๋ฒ์ด๋ค. `string text ${expression} string text`

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

### โ Styled-components
1. `props` ์ ๋ฌด์ ๋ฐ๋ฅธ  `styled-components` ์์ฑ ๋ฐฉ๋ฒ

```javascript
// props๊ฐ ์๋ ๊ฒฝ์ฐ
const Button = styled.button`
  font-size: 32px;
	margin: 1em;
	padding: 0.25em 1em;
`

function App(){
	return <Button>Hello!</Button>
}

// props๊ฐ ์๋ ๊ฒฝ์ฐ
const Button = styled.button`
  font-size: 32px;
	margin: 1em;
	padding: 0.25em 1em;
	background: ${(props) => props.primary ? "pink" : "black"}
	color: ${(props) => props.primary ? "white" : "green"}
`

function App(){
	return <Button primary>Hello!</Button>  // primary = true์ ๊ฐ์
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

// SCSS: ์ค๋ณต๋ ์ ํ์ ์ ๊ฑฐ ๊ฐ๋ฅ
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

	+ .name {  /* ์ธ์ ์์ ์ฐ์ฐ์ */
		color: purple;
	}
}

// SCSS in styled components
const SCSSStyledDiv = styled.div`
	background-color: orange;
	color: white;

	div{   // SCSSStyledDiv ๋ด๋ถ์ divํ๊ทธ์ bg color
		background-color: red;
	}

	.purple{  // SCSSStyledDiv ๋ด๋ถ์ purple ํด๋์ค์ bg color
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

3. style-components ๋ก CSS ์์ ํ๊ธฐ

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
    
    & + & {  // ๋์ค์ ํ๋ ์ฌ์ฉํ๋ฉด ๋จ
        margin-left: 16px;
    }
    
    + button {  // ๋์ค์ ํ๋ ์ฌ์ฉํ๋ฉด ๋จ
        margin-left: 16px;
    }
    
    &:hover {
        box-shadow: 8px 4px 4px gray;
    }
`
```

### โ Figma
1. `shift + scroll` :ํก์ผ๋ก `scroll`
2. ์ข์ธก Search: ์ปดํฌ๋ํธ ๊ตฌ์กฐ ํ์ธ ๊ฐ๋ฅ
3. ๋ง์ฐ์ค ์ปค์๋ก ์ปดํฌ๋ํธ ์ฌ์ด์ ๊ฑฐ๋ฆฌ ํ์ธ ๊ฐ๋ฅ(`px`)

---
## ๐ 65์ผ์ฐจ 1.22.ํ . ์จ๋ผ์ธ ๊ฐ์
์ค๋์ ์ง์  `React`์ `Styled-components`๋ฅผ ์ด์ฉํด์ ํธ๋์นด๋, ํญ, ๊ฒ์์ฐฝ์ ์ด๊ธฐ `UI`๋ก ๊ตฌํํ๊ณ  ์ดํ์๋ ์ค์  `API`๋ฅผ ์ฐ๋ํ๋ฉด์ ๊ฒ์์ฐฝ์์ ๊ฒ์ ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ ธ์ค๋ ๋ฐฉ๋ฒ๊น์ง ์์ฉํ๋ ๋ฒ์ ๋ฐฐ์ ๋ค. ๊ทธ๋ฆฌ๊ณ  ๋ง์ง๋ง์๋ `JS`์์ `TS`๋ก ๋ง์ด๊ทธ๋ ์ด์ ์ค์  ๋ฐฉ๋ฒ์ ๋ํด์ ๋ฐฐ์ ๋ค. `CSS`๋ฅผ ๋ฐฐ์ธ ๋ `position`๊ณผ ๊ฐ์ ๋ด์ฉ์ ์ง์  ์ ์ฉํ๋ ค๊ณ  ํ  ๋ ์ด๋ ค์์ด ๋ง์๋๋ฐ ์ด๋ฒ ์ค์ต์ ๋ณด๋ฉด์ `position: absolute`์ ์ฌ์ฉ์๊ธฐ๋ฅผ ์ ๋ฐฐ์ธ ์ ์์๊ณ , ์๋ฌด ์กฐ๊ฑด์์ ์ ์ฉ๋๋๊ฒ์ด ์๋๋ผ ๋ถ๋ชจ๊ฐ `relative`์ผ ๋ ์ ์ฉ๋๋ค๋ ์ ๋ ๋ฐฐ์ ๋ค. ์ธ์๊น์๋ ๋ถ๋ถ์ `::before`์ฐ์ฐ์๋ก `background-color`๋ฅผ ๋ง๋๋ ๋ฐฉ๋ฒ์ธ๋ฐ, ํ์์ ์ ์ ์ฉํ์ง ์๋ ๋ฐฉ๋ฒ์ด์ด์ ๋์ค์ ์จ๋จน์ ์ ์๋๋ก ๋ฐ๋ก ๊ธฐ๋ก์ ํด๋์๋ค. ๊ทธ๋ฆฌ๊ณ  ๊ฒ์์ฐฝ ๊ตฌํ์ `debounce`๋ฅผ ์ ์ฉํ์ฌ ๋งค ์๋ ฅ๋ง๋ค ์๋ฒ๋ก ์์ฒญํ์ง ์๊ณ  ํน์  ์๊ฐ ์ดํ์ ์๋ฒ๋ก ์๋ ฅ๊ฐ์ ์์ฒญํ์ฌ, ์๋ฒ์์ฅ์์ ๋ถํ๋ฅผ ์ด๋์ ๋ ์ค์ฌ์ค ์ ์๋ ๋ฐฉ๋ฒ์ธ๋ฐ, ํ์์์ ๋ง์ด ์ฌ์ฉํ๋ ๋ฐฉ๋ฒ์ด๋ผ์ ๊น๋จน์ง ์์์ผ๊ฒ ๋ค๊ณ  ์๊ฐํ๋ค.

### Styled-components
1. `styled-components` ๋ฅผ ์ฌ์ฉ ํ  ๋ ๋ค์๊ณผ ๊ฐ์ด ์ปดํฌ๋ํธ ํ๋๋ง๋ค `import` ํด์ผ ํ  ์ํฉ์ด ๋ง์ผ๋ฉด `* as Card` ์ฒ๋ผ ์ ์ฒด ํ์ด์ง๋ฅผ ๋ก๋ํ๊ณ  `component` ์์ `Card` ๋ฅผ ๋ถ์ฌ  `after` ๊ณผ ๊ฐ์ด ์ฌ์ฉํ๋ฉด ๊ฐ์ ๊ฒฐ๊ณผ๋ฅผ ๋ฐํํด๋ ์ฝ๋๊ฐ ์ค์ด๋ค์ด ๊ฐ๋์ฑ์ด ์ฌ๋ผ๊ฐ๋ค.

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
        <Tags>{tags.join("๏น")}</Tags>
        <Title>{title}</Title>
        <Description>{description}</Description>
        <TextsWrapper>
            <TextWrapper>
                <Chart />
                <Text>๋์ด๋ : {level}</Text>
            </TextWrapper>
            <TextWrapper>
                <Computer />
                <Text>์์ : {classFormat}</Text>
            </TextWrapper>
            <TextWrapper>
                <Calendar />
                <Text>๊ธฐ๊ฐ : {duration}</Text>
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
            <CostFree>๋ฌด๋ฃ</CostFree>
        ) : (
            <CostWrapper>
                <CurrentCost>
                    {currentCost.toLocaleString()}์
                </CurrentCost>
                <OriginalCost>
                    {originalCost.toLocaleString()}์
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
      <Card.Tags>{tags.join("๏น")}</Card.Tags>
      <Card.Title>{title}</Card.Title>
      <Card.Description>{description}</Card.Description>
      <Card.TextsWrapper>
        <Card.TextWrapper>
          <Chart />
          <Card.Text>๋์ด๋ : {level}</Card.Text>
        </Card.TextWrapper>
        <Card.TextWrapper>
          <Computer />
          <Card.Text>์์ : {classFormat}</Card.Text>
        </Card.TextWrapper>
        <Card.TextWrapper>
          <Calendar />
          <Card.Text>๊ธฐ๊ฐ : {duration}</Card.Text>
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
        <Card.CostFree>๋ฌด๋ฃ</Card.CostFree>
      ) : (
        <Card.CostWrapper>
          <Card.CurrentCost>{currentCost.toLocaleString()}์</Card.CurrentCost>
          <Card.OriginalCost>{originalCost.toLocaleString()}์</Card.OriginalCost>
          <Card.DiscountPercentile>{discountPercentile}%</Card.DiscountPercentile>
        </Card.CostWrapper>
      )}
    </Card.Container>
  );
```

2. props ์ ๋ง๊ฒ ํด๋น ์ปดํฌ๋ํธ์ css ๋ฅผ ์ถ๊ฐํ๊ฑฐ๋ ๋ณ๊ฒฝํ๊ณ  ์ถ๋ค๋ฉด ๋ค์์ฒ๋ผ ์ฌ์ฉํ์

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

3. `absolute` ์ํ์์ `left: 0, right: 0`์ผ๋ก ์ค์ ํ๋ฉด `width: 100%` ์ ๋ง์ฐฌ๊ฐ์ง๋ก ์ข์ฐ๋ก ์ญ ํด์ง๋ค. `left: 0, right: 0, top: 0, bottom: 0`์ผ๋ก ์ค์ ํ๋ฉด ์ํ์ข์ฐ๋ก ์ญ ํด์ง ์ํ๊ฐ ๋๋ค.
4. `navBar` ์์ ์ํ๋ ๋ฉ๋ด๋ฅผ ํด๋ฆญํ์ ๋ `active` ์ํค๋ ๋ฐฉ๋ฒ์ `useState` ๋ฅผ ์ด์ฉํด์ ํด๋น ํ๊ทธ๋ฅผ ๋๋ฅด๋ฉด `active`๋๊ฒ ๋ ์ค์ ํ๋ฉด ๋๋ค.

```javascript
// App.jsx
import { useState } from "react";
import Tab from "./Tab.jsx";

export default function App() {
  const [currTab, setCurrTab] = useState("ํธ๋");
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

const tabs = ["ํธ๋", "๊ณผ๋ชฉ"];

Tab.defaultProps = {
  currTab: "ํธ๋",
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

5. ๊ฒ์ ์ฐฝ ๋ง๋ค๊ธฐ: `container` ์์ `input` ์ ๋ฃ๋๋ค. ๋๋ณด๊ธฐ ๋ชจ์์ `container` ์์์ `svg` ํ๊ทธ๋ฅผ ๋ฐ๋ก ์ค์ ํด์ค๋ค.

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
        placeholder="๋ฐฐ์ฐ๊ณ  ์ถ์ ์ธ์ด, ๊ธฐ์ ์ ๊ฒ์ํด ๋ณด์ธ์."
        value={value}
        onChange={(e) => onChange(e.target.value)}
      />
    </Container>
  );
}
```

### React์์ TS๋ก ๋ง์ด๊ทธ๋ ์ด์ ํ๊ธฐ
1. ํ์์คํฌ๋ฆฝํธ ๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ค์น

```javascript
* ์๋ก CRA๋ฅผ ์์ฑํ๋ ๊ฒฝ์ฐ: npx create-react-app <project name> -template typescript๋ง ์์ฑ
* ๊ธฐ์กด JS ํ์ผ์ TS๋ก ๋ง์ด๊ทธ๋ ์ด์ ํ๋ ๊ฒฝ์ฐ ํ๋จ ๊ณผ์  ์์

npm i -D typescript esbuild-loader @types/react @types/react-dom
yarn add -D typescript esbuild-loader @types/react @types/react-dom

- typescript: tsc ์ปดํ์ผ๋ฌ, ts ๋ฌธ๋ฒ ์ง์์ ์ํด ํ์ํ ๋ผ์ด๋ธ๋ฌ๋ฆฌ
- @types/react: react ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ฅผ ์ํ ํ์ ํจํค์ง
- @types/react-dom: react์์ dom element์ ๊ด๋ จ๋ ํ์๋ค์ ๋ชจ์๋๋ ํจํค์ง
  * @types/๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ด๋ฆ: ํ์์คํฌ๋ฆฝํธ์์ ๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ค์นํ  ๋ ์ฌ์ฉํ๋ ๋ช๋ น์ด(Definitely Typed ์ฐธ๊ณ )
- esbuild/loader: ํ์์คํฌ๋ฆฝํธ ํธ๋์คํ์ผ๋ง์ ์ํ ํจํค์ง(์๋๊ฐ ๋งค์ฐ ๋น ๋ฅด๋ค)
  * ๋ณธ๋๋ babel-loader๋ฅผ ์ฌ์ฉํ์ผ๋, ์ต๊ทผ ๋ค์ด webpack์ ๋น๋๋ฅผ ๋นจ๋ฆฌํ๊ธฐ ์ํด esbuild๋ฅผ ๋ง์ด ์ฌ์ฉํ๋ ์ถ์ธ๋ค
```

2. tsconfig.json ์ค์ 

```javascript
1. tsconfig.json ํ์ผ ์์ฑ 
  * tsc --init ํน์ npx tsc --init ์๋ ฅ ์ tsconfig.json์ ๊ธฐ๋ณธ์ ์ธ ์ปดํ์ผ๋ฌ ์ต์์ ์ค์ ํด์ค๋ค.

{
  "compilerOptions": {
    "target": "es5",  // ํธ๋์คํ์ผ๋ง์ ํ  ๊ฒฝ์ฐ ์ด๋ค ๋ฒ์ ์ผ๋ก ๋ณํ ํ  ๊ฒ์ธ์ง(IE ์ง์์ es5๋ก ์ค์ )
		"outDir": "./dist/",  // ์ปดํ์ผ ํ ์ด๋ค ๊ฒฝ๋ก๋ก ์ ์ฅํ ์ง?
		"sourceMap": true,  // ๋๋ฒ๊น์ ์ํ ์์ค๋งต์ด ํ์ํ ๊ฒฝ์ฐ์ ์ค์ 
    "module": "esnext",  // ๋ชจ๋ ์ฝ๋๋ฅผ ESM(ECMAScript Module: import, export), CJS(Common JS: require, exports.module) ๋ชจ๋๋ก ์ค์ ํ ๊ฒ์ธ๊ฐ?
    "jsx": "react-jsx"  // jsxํ์ผ์ jsํ์ผ๋ก ๋ณํํ๋๋ก ํ๋ ์ค์ , react ์ค์ ์ jsxํ์ผ์ด js๋ก ๋ณํ๋๋ค.
  }
}

jsx ์ต์์ preserve, react, react-native 3๊ฐ์ง ์ต์์ ์ค์ ํ  ์ ์์ต๋๋ค.
1. preserve: ๋ฐ๋ฒจ์ด๋ swc ๊ฐ์ ๋ค๋ฅธ ํธ๋์คํ์ผ๋ฌ๊ฐ ๋ณํํ  ์ ์๋๋ก jsx ๋ฌธ๋ฒ์ ํธ๋์คํ์ผ๋งํ์ง ์๊ณ  ๊ทธ๋๋ก ๋ก๋๋ค. ๋ฐ๋ผ์ ํธ๋์คํ์ผ๋ง ๊ฒฐ๊ณผ๋ .tsx์์ .jsx ํ์ผ์ด ๋ฉ๋๋ค.

2. react: jsx ๋ฌธ๋ฒ์ js๋ก ๋ณํ์ํต๋๋ค. ํธ๋์คํ์ผ๋ง ๊ฒฐ๊ณผ๋ .js ํ์ฅ์ ํ์ผ์๋๋ค.

3. react-native: preserve ๋ชจ๋์ฒ๋ผ jsx ๋ฌธ๋ฒ์ ๊ทธ๋๋ก ๋์ง๋ง ํธ๋์คํ์ผ๋ง ๊ฒฐ๊ณผ๋ .js ํ์ฅ์ ํ์ผ์ด ๋ฉ๋๋ค.
```

3. ์ฌ์ฉํ๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ค ์ค @types ํจํค์ง ์ถ๊ฐ(ํ์ ์ ํ)

```javascript
1. npm i -D @types/<library name>: DefinitelyTyped ์คํ์์ค์ ๋ฑ๋ก๋ ํ์ ์ ์ธ ํ์ผ ์ค์น
2. git repo์ index.d.ts์ ์๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ฉด ์ค์น ์ํด๋ ๋จ. 
3. npm์์ @types/ํจํค์ง๋ช ๊ฒ์ํด๋ณด๊ณ  ์์ผ๋ฉด @types/ํจํค์ง ์ค์นํ๊ณ  @types/ํจํค์ง๊ฐ ์๋ค๋ฉด ์ง์  ๋ชจ๋์ ๋ํ ํ์์ ์ ์ธํด์ผ ํ๋ค.
4. ๋ชจ๋์ ํ์์ ์ง์  ์ ์ธํ๋ค๋ฉด ๋ค๋ฅธ ๊ฐ๋ฐ์๋ ์ฌ์ฉํ  ์ ์๊ฒ ๋ผ์ด๋ธ๋ฌ๋ฆฌ์ DefinitelyTyped์ PR์ ๋ ๋ ค๋ณด์
```

4. `webpack` ์ค์  ๋ณ๊ฒฝ

```javascript
module.exports = {
  entry: {  // ์ฑ์ ์์ํ  ํ์ผ
    main: "./src/index.js",
  },
  output: {  // ์นํฉ ๋ฒ๋ค๋ง ๊ฒฐ๊ณผ์ ๋ํ ์ต์, ๊ธฐ๋ณธ ๊ฒฝ๋ก๋ dist
    path: path.resolve(__dirname, "dist"),
    filename: "[name].js",
  },
  resolve: {  // ๋ฒ๋ค๋งํ  ํ์ฅ์ ์ค์ 
    extensions: [".js", ".jsx", ".ts", ".tsx"],
  },
  module: {  // ๋ฒ๋ค๋ง ํ  ๋ ํ๋ฌ๊ทธ์ธ ์ค์  ๊ฐ๋ฅ
    rules: [
      {
        test: /\.(t|j)sx?$/,
        loader: "esbuild-loader",  // ํ์์คํฌ๋ฆฝํธ ๋ณํ์ ์ํ ๋ก๋
        options: {
          loader: "tsx", // Or 'ts' if you don't need tsx
          target: "es2015",
        },
      },
      {
        test: /\.css$/,  
        use: ["style-loader", "css-loader"],  // style-loader: style ํ๊ทธ๋ฅผ ์ฝ์ํด dom์ css ์ถ๊ฐ, css-loader: css ํ์ฅ์์ cssํ์ผ์ ์ฝ๊ธฐ ์ํ ๋ก๋, css ํ์ฅ์๋ฅผ ๊ฐ์ ธ์์ style ํ๊ทธ๋ฅผ ์ฝ์ํด DOM์ css๋ฅผ ์ถ๊ฐํ๋ค.
      },
    ],
  },
  externals: {  // ๋ฒ๋ค๋ง ๊ฒฐ๊ณผ์์ ์ ์ธํ  ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ค
    react: "React",
    "react-dom": "ReactDOM",
  },
};
```

5. `jsx` โ `.tsx` ๋ก ํ์ฅ์ ๋ณํ

```javascript
- jsx ํ์ผ์์ tsxํ์ผ๋ก ํ์ฅ์ ๋ณ๊ฒฝ์ ํ๊ณ  ์ด ๊ณผ์ฅ์์ ์๊ธฐ๋ ํ์ ์ค๋ฅ๋ค์ ํด๊ฒฐํด์ผ ๋ง์ด๊ทธ๋ ์ด์์ด ๋๋๋ค.
```

---
## ๐ [์ ํ๊ฐ์] React์์์ ํ์์คํฌ๋ฆฝํธ
์ด๋ฒ ๊ธ์ ํ์๋ก ๋ค์ด์ผํ๋ ๊ฐ์๋ฅผ ๊ธฐ๋กํ๊ธฐ ์ํด ์ ๋ ๊ธ์ ์๋๊ณ  ์ ํ์ ์ผ๋ก ๋ฃ๋ ๊ฐ์ ์ค `React์์์ ํ์์คํฌ๋ฆฝํธ` ๊ฐ์๋ฅผ ๊ธฐ๋ก์ผ๋ก ๋จ๊ฒจ ๋์๊นํ๋ค. ๊ทธ ์ด์ ๋ ์ด์ ๋ถํฐ ์ฌ์ฉํด์์ง๋ง ์์ผ๋ก๋ ์ฌ์ฉํ  ์ธ์ด์ธ ํ์์คํฌ๋ฆฝํธ์ ํ๋ ์์ํฌ์ธ React๊ธฐ ๋๋ฌธ์ด๋ค. ๊ทธ๋ฆฌ๊ณ  ์ง๊ธ๊น์ง ๋ด๊ฐ ์์ฑํ ์ฝ๋๋ฅผ ์ด๋ป๊ฒ ๋ ํจ์จ์ ์ด๊ฒ ์์ฑํ  ์ ์์์ง์ ๋ํ ๋ช๊ฐ์ง์ ์ํ์ ๋ฐฐ์ธ ์ ์๊ธฐ ๋๋ฌธ์ด๋ค. ํ๊ฐ์ง ์๋ก ๋๋ <a href='https://ywtechit.tistory.com/404?category=950465'>์ด๊ฑฐ ๋จน์ด๋ด?</a> ํ๋ก์ ํธ์ ํ์์กฐ์น๋ก `webpack`๊ณผ `babel`๋ฅผ ์ง์  ์ค์ ํ๋ ๊ฐ๋จํ ์์(<a href='https://github.com/YWTechIT/image-drag-and-drop'>image-drag-and-drop</a>)๋ฅผ ๋ง๋ค์์ผ๋, `babel`์ ์ค์ ํ๊ธฐ ์ํด ์๊ฐ๋ณด๋ค ๋ง์ ํ๋ฌ๊ทธ์ธ(`npm i -D @babel/core @babel/preset-env @babel/preset-react @babel/polyfill babel-loader`)์ด ํ์ํ๊ณ , ์ด๋ ๊ณง ๋น๋ ์๊ฐ์ ๋์ด๋๊ฒ ํ๋ ์ฃผ๋ฒ์ด์๋ค. ํ์ง๋ง, `esbuild-loader`๋ฅผ ์ฌ์ฉํ๋ฉด ๋น๋ ์๊ฐ์ ๋ํญ ๋จ์ถ์ํฌ ์ ์๋๋ฐ(<a href='https://github.com/privatenumber/esbuild-loader/discussions/138'>๋งํฌ</a>) ์ด๋ ๋์๊ฒ ์๋ก์ด ์๊ฐ์ ์ฃผ์๋ค. ๋ด์ผ๋ถํฐ 2์ฐจ ํ ํ๋ก์ ํธ๋ฅผ ํ๊ฒ ๋๋๋ฐ ์ด๋ `babel-loader` ๋์  `esbuild-loader`์ ์ฌ์ฉํ๋ ค๊ณ  ํ๋ค. ๋ง์ง๋ง์ผ๋ก ์ํ๊ด๋ฆฌ ๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ค ํ๋์ธ `Jotai`์ ๋ํด์๋ ๋ฐฐ์ ๋ค. 2021๋ 11์ 28์ผ ๊ธฐ์ค์ผ๋ก ๊นํ์ ์คํ ์๋ `redux`๋ 57.1k, `recoil`์ 14.9k, `jotai`๋ 6.2k์ธ๋ฐ, ์คํ ์๋ก๋ง ๋ดค์ ๋ `jotai`๊ฐ ํ์ ํ ๋ฎ์๋ฐ ์ ๋ฐฐ์ฐ๋์ง ์ฒ์์๋ ๊ถ๊ธํ์ง๋ง, ๋จ์ํ ๋ง์ ์ฌ๋๋ค์ด ์ฌ์ฉํ๊ธฐ ๋๋ฌธ์ ์ฌ์ฉํด์ผ ํ๋ค๋ ์๊ฐ๋ณด๋ค๋ ๊ฐ ์คํ์์ค ํ๋ก์ ํธ๊ฐ ์ด๋ป๊ฒ ๊ด๋ฆฌ๋๊ณ  ์๋์ง, ์ฝ์ด ๊ฐ๋ฐ์๋ ์ด๋ค ์ฌ๋์ธ์ง, ๊ฐ ๋ผ์ด๋ธ๋ฌ๋ฆฌ์ ์ฅ๋จ์ ์ ์ดํด์ ์ ํํด์ผํ๋ค๋ ๊ฐ์ ๋ด์ฉ์ ๋ณด๊ณ  ๊ผญ ์คํ์๊ฐ ๋ง์ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ง ์ฌ์ฉํด์ผํ๋ค๋ ํธ๊ฒฌ์ ๊ฐ๊ณ ์๋ ๋์ ์ค๋งํจ์ ๋ฐ๋ก ์ก์ ์ ์์๋ค. 


### React์์ TS๋ก ๋ง์ด๊ทธ๋ ์ด์ ํ๊ธฐ
1. ํ์์คํฌ๋ฆฝํธ ๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ค์น

```javascript
* ์๋ก CRA๋ฅผ ์์ฑํ๋ ๊ฒฝ์ฐ: npx create-react-app <project name> -template typescript๋ง ์์ฑ
* ๊ธฐ์กด JS ํ์ผ์ TS๋ก ๋ง์ด๊ทธ๋ ์ด์ ํ๋ ๊ฒฝ์ฐ ํ๋จ ๊ณผ์  ์์

npm i -D typescript esbuild-loader @types/react @types/react-dom
yarn add -D typescript esbuild-loader @types/react @types/react-dom

- typescript: tsc ์ปดํ์ผ๋ฌ, ts ๋ฌธ๋ฒ ์ง์์ ์ํด ํ์ํ ๋ผ์ด๋ธ๋ฌ๋ฆฌ
- @types/react: react ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ฅผ ์ํ ํ์ ํจํค์ง
- @types/react-dom: react์์ dom element์ ๊ด๋ จ๋ ํ์๋ค์ ๋ชจ์๋๋ ํจํค์ง
  * @types/๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ด๋ฆ: ํ์์คํฌ๋ฆฝํธ์์ ๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ค์นํ  ๋ ์ฌ์ฉํ๋ ๋ช๋ น์ด(Definitely Typed ์ฐธ๊ณ )
- esbuild/loader: ํ์์คํฌ๋ฆฝํธ ํธ๋์คํ์ผ๋ง์ ์ํ ํจํค์ง(์๋๊ฐ ๋งค์ฐ ๋น ๋ฅด๋ค)
  * ๋ณธ๋๋ babel-loader๋ฅผ ์ฌ์ฉํ์ผ๋, ์ต๊ทผ ๋ค์ด webpack์ ๋น๋๋ฅผ ๋นจ๋ฆฌํ๊ธฐ ์ํด esbuild๋ฅผ ๋ง์ด ์ฌ์ฉํ๋ ์ถ์ธ๋ค
```

2. tsconfig.json ์ค์ 

```javascript
1. tsconfig.json ํ์ผ ์์ฑ 
  * tsc --init ํน์ npx tsc --init ์๋ ฅ ์ tsconfig.json์ ๊ธฐ๋ณธ์ ์ธ ์ปดํ์ผ๋ฌ ์ต์์ ์ค์ ํด์ค๋ค.

{
  "compilerOptions": {
    "target": "es5",  // ํธ๋์คํ์ผ๋ง์ ํ  ๊ฒฝ์ฐ ์ด๋ค ๋ฒ์ ์ผ๋ก ๋ณํ ํ  ๊ฒ์ธ์ง(IE ์ง์์ es5๋ก ์ค์ )
		"outDir": "./dist/",  // ์ปดํ์ผ ํ ์ด๋ค ๊ฒฝ๋ก๋ก ์ ์ฅํ ์ง?
		"sourceMap": true,  // ๋๋ฒ๊น์ ์ํ ์์ค๋งต์ด ํ์ํ ๊ฒฝ์ฐ์ ์ค์ 
    "module": "esnext",  // ๋ชจ๋ ์ฝ๋๋ฅผ ESM(ECMAScript Module: import, export), CJS(Common JS: require, exports.module) ๋ชจ๋๋ก ์ค์ ํ ๊ฒ์ธ๊ฐ?
    "jsx": "react-jsx"  // jsxํ์ผ์ jsํ์ผ๋ก ๋ณํํ๋๋ก ํ๋ ์ค์ , react ์ค์ ์ jsxํ์ผ์ด js๋ก ๋ณํ๋๋ค.
  }
}

jsx ์ต์์ preserve, react, react-native 3๊ฐ์ง ์ต์์ ์ค์ ํ  ์ ์์ต๋๋ค.
1. preserve: ๋ฐ๋ฒจ์ด๋ swc ๊ฐ์ ๋ค๋ฅธ ํธ๋์คํ์ผ๋ฌ๊ฐ ๋ณํํ  ์ ์๋๋ก jsx ๋ฌธ๋ฒ์ ํธ๋์คํ์ผ๋งํ์ง ์๊ณ  ๊ทธ๋๋ก ๋ก๋๋ค. ๋ฐ๋ผ์ ํธ๋์คํ์ผ๋ง ๊ฒฐ๊ณผ๋ .tsx์์ .jsx ํ์ผ์ด ๋ฉ๋๋ค.

2. react: jsx ๋ฌธ๋ฒ์ js๋ก ๋ณํ์ํต๋๋ค. ํธ๋์คํ์ผ๋ง ๊ฒฐ๊ณผ๋ .js ํ์ฅ์ ํ์ผ์๋๋ค.

3. react-native: preserve ๋ชจ๋์ฒ๋ผ jsx ๋ฌธ๋ฒ์ ๊ทธ๋๋ก ๋์ง๋ง ํธ๋์คํ์ผ๋ง ๊ฒฐ๊ณผ๋ .js ํ์ฅ์ ํ์ผ์ด ๋ฉ๋๋ค.
```

3. ์ฌ์ฉํ๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ค ์ค @types ํจํค์ง ์ถ๊ฐ(ํ์ ์ ํ)

```javascript
1. npm i -D @types/<library name>: DefinitelyTyped ์คํ์์ค์ ๋ฑ๋ก๋ ํ์ ์ ์ธ ํ์ผ ์ค์น
2. git repo์ index.d.ts์ ์๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ฉด ์ค์น ์ํด๋ ๋จ. 
3. npm์์ @types/ํจํค์ง๋ช ๊ฒ์ํด๋ณด๊ณ  ์์ผ๋ฉด @types/ํจํค์ง ์ค์นํ๊ณ  @types/ํจํค์ง๊ฐ ์๋ค๋ฉด ์ง์  ๋ชจ๋์ ๋ํ ํ์์ ์ ์ธํด์ผ ํ๋ค.
4. ๋ชจ๋์ ํ์์ ์ง์  ์ ์ธํ๋ค๋ฉด ๋ค๋ฅธ ๊ฐ๋ฐ์๋ ์ฌ์ฉํ  ์ ์๊ฒ ๋ผ์ด๋ธ๋ฌ๋ฆฌ์ DefinitelyTyped์ PR์ ๋ ๋ ค๋ณด์
```

4. `webpack` ์ค์  ๋ณ๊ฒฝ

```javascript
module.exports = {
  entry: {  // ์ฑ์ ์์ํ  ํ์ผ
    main: "./src/index.js",
  },
  output: {  // ์นํฉ ๋ฒ๋ค๋ง ๊ฒฐ๊ณผ์ ๋ํ ์ต์, ๊ธฐ๋ณธ ๊ฒฝ๋ก๋ dist
    path: path.resolve(__dirname, "dist"),
    filename: "[name].js",
  },
  resolve: {  // ๋ฒ๋ค๋งํ  ํ์ฅ์ ์ค์ 
    extensions: [".js", ".jsx", ".ts", ".tsx"],
  },
  module: {  // ๋ฒ๋ค๋ง ํ  ๋ ํ๋ฌ๊ทธ์ธ ์ค์  ๊ฐ๋ฅ
    rules: [
      {
        test: /\.(t|j)sx?$/,
        loader: "esbuild-loader",  // ํ์์คํฌ๋ฆฝํธ ๋ณํ์ ์ํ ๋ก๋
        options: {
          loader: "tsx", // Or 'ts' if you don't need tsx
          target: "es2015",
        },
      },
      {
        test: /\.css$/,  
        use: ["style-loader", "css-loader"],  // style-loader: style ํ๊ทธ๋ฅผ ์ฝ์ํด dom์ css ์ถ๊ฐ, css-loader: css ํ์ฅ์์ cssํ์ผ์ ์ฝ๊ธฐ ์ํ ๋ก๋, css ํ์ฅ์๋ฅผ ๊ฐ์ ธ์์ style ํ๊ทธ๋ฅผ ์ฝ์ํด DOM์ css๋ฅผ ์ถ๊ฐํ๋ค.
      },
    ],
  },
  externals: {  // ๋ฒ๋ค๋ง ๊ฒฐ๊ณผ์์ ์ ์ธํ  ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ค
    react: "React",
    "react-dom": "ReactDOM",
  },
};
```

5. `jsx` โ `.tsx` ๋ก ํ์ฅ์ ๋ณํ

```javascript
- jsx ํ์ผ์์ tsxํ์ผ๋ก ํ์ฅ์ ๋ณ๊ฒฝ์ ํ๊ณ  ์ด ๊ณผ์ฅ์์ ์๊ธฐ๋ ํ์ ์ค๋ฅ๋ค์ ํด๊ฒฐํด์ผ ๋ง์ด๊ทธ๋ ์ด์์ด ๋๋๋ค.
```
### โ ํจ์ํ ์ปดํฌ๋ํธ์ `props` ํ์ ์ค์ ํ๊ธฐ
1. component props์ ํ์ ์ค์ 

```tsx
// {...props}`: ์คํ๋ ๋ ์ฐ์ฐ์๋ก props๋ฅผ button์ props์ ๋ชจ๋ ์ ๋ฌ
// `React.PropsWithChildren`: ์ฌ์ฉ์๊ฐ ๋๊ธด props ํ์(P)์ props.children์ ์ธํฐ์น์
// type PropsWithChildren<P> = P & { children?: ReactNode | undefined };
// `props.children`: react์์ ๊ธฐ๋ณธ์ ์ผ๋ก ์ ๋ฌํด์ฃผ๋ children props. ์์ ๋ธ๋๋ค์ด ์ ๋ฌ๋จ

export const Button = (props: React.PropsWithChildren<ButtonProps>) => {
	return <button {...props} }>{props.children}}</button> // {...props}๋ก children์ ํ๊บผ๋ฒ์ ์ ๋ฌ ํ  ์ ์์ผ๋ type์ด ๋ง์์ผ ํจ
};
```

2. `React.FC` ์ฌ์ฉํด ๋ ๊ฐ๋จํ ํํ

```tsx
// React.FC: ๋ด๋ถ์ ์ผ๋ก PropsWithChildren์ ์ฌ์ฉ
// React.FC ํ์์ ์ฌ์ฉํ๋ฉด ๋ด๋ถ์ ์ผ๋ก PropsWithChildren์ ์ฌ์ฉํ์ฌ ์ ๋ค๋ฆญ์ Props ํ์๊ณผ children ํ์์ ์ธํฐ์น์.
// props์ React.PropsWithChildren์ ์ ์ธํ๋ ๊ฒ๊ณผ ๊ฐ์ ํจ๊ณผ

export const Button: React.FC<ButtonProps> = (props) => {
	return <button style={props.buttonStyle>{props.children}</button>;
}

type FC<P = {}> = FunctionComponent<P>;

interface FunctionComponent<P = {}> {
	(props: PropsWithChildren<P>, context?: any): ReactElement<any, any> | null;
}
```

### โ style props์ ํ์ ์ ์ฉํ๊ธฐ
1. ๊ธฐ์กด ๋ฐฉ๋ฒ

```css
/* 
1. ๋ชจ๋  button์ ์ ์ฉ ๋จ
2. class๋ก ๋ง๋ค์ด๋ `background-color`, `font-size`, `font-weight` ๋ฑ ์์ฃผ ๋ณ๊ฒฝ๋๋ ๊ฒ๋ค์ ์ํด ์ฌ๋ฌ ๊ฐ์ `class` ๋ฅผ ์กฐํฉํด์ผ ํจ(ex, `className = button bg-black size-16 weight-700`)
3. `props` ๋ก ์ ๋ฌํ๋ฉด ์ด๋จ๊น? 
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
1. button ํ๊ทธ์ style props ํ์
2. createButtonStyle: ๋ฐํ ํ์์ React CSSProperties๋ก ํ๋ style ๊ฐ์ฒด ํฉํ ๋ฆฌ ํจ์ ์์ฑ
3. '...styles'๋ก ๋ค๋ฅธ style ์์ฑ๋ ๋ฐ์ ์ ์๊ฒ ์ถ๊ฐ
*/

const createButtonStyle = (
	styles?: React.CSSProperties): React.CSSProperties => ({
	padding: 50,
	borderRadius: 4,
	border: "none",
	...styles,  // ๊ธฐ์กด ์์ฑ์ override ํ  ์ ์์
});

interface ButtonProps {
	styles?: React.CSSProperties;
}

export const Button: React.FC<ButtonProps> = (props) => {
  const buttonStyles = createButtonStyle(props.styles);
	return <button style={buttonStyles>{props.children}</button>;
}
```

### โ event props์ ํ์ ์ ์ฉํ๊ธฐ
1. button์ ํด๋ฆญํ์ ๋ handleClick์ผ๋ก ์ ๋ฌํ๊ณ  ์ถ์
2. `React.MouseEvent<Element, Event>`: `<button onClick={e => console.log(e)} />` ์ํ์์ `e` ์ ๋ง์ฐ์ค ํธ๋ฒ
3. `e` ์ ํ์์ ๋ณต์ฌํด์ `ButtonProps` ์ธํฐํ์ด์ค์ `handleClick event` ํ์์ผ๋ก ๋ถ์ฌ๋ฃ๊ฑฐ๋, `form` ์ฒ๋ผ `e`๊ฐ ๋ณด์ด์ง ์์ ๋๋ `BaseSyntheticEvent` ๋ฅผ ์ฌ์ฉํ๋ค.

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

4. ๊ฒฐ๊ณผ์ฝ๋

```tsx
// MainScreen.tsx
import { Button } from "../components/Button";
import { useNavigate } from "react-router-dom";

export const MainScreen = () => {
  const navigate = useNavigate();
  return (
    <>
      <h1>ํ์์คํฌ๋ฆฝํธ ๋ฅ๋ ฅ ๊ณ ์ฌ</h1>
      <p>๋์ ํ์์คํฌ๋ฆฝํธ ์ค๋ ฅ์ ์ด๋ ์ ๋์ผ๊น?</p>
      <a
        className="App-link"
        href="https://www.typescriptlang.org/ko/docs/handbook/react.html"
        target="_blank"
        rel="noopener noreferrer"
      >
        Learn Typescript + React
      </a>
      <Button styles={{ marginTop: 50 }} handleClick={() => console.log('button click')}>
        ํ์คํธ ์์ํ๊ธฐ
      </Button>
    </>
  );
};

// Button.tsx
import React from "react";

// 3. styles๋ฅผ ๋งค๊ฐ๋ณ์๋ก ๋ฐ์ styles ๊ฐ์ฒด๋ฅผ ๋ฐํํ๋ style ํฉํ ๋ฆฌ ํจ์๋ฅผ ์ ์ํด์ฃผ์ธ์
// createButtonSylte์ ๋งค๊ฐ๋ณ์์ ๋ฐํ ํ์์ ์ ์ด์ฃผ์ธ์
// styles๋ React์์ ์ ๊ณตํ๋ style ํ์์๋๋ค. 
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

// 1. component์ props ์ ์ฉ์ ํ๊ธฐ ์ํด ButtonProps ์ธํฐํ์ด์ค๋ฅผ ์ ์ธํด์ฃผ์ธ์
interface ButtonProps {
  // React์์ ์ ๊ณตํ๋ styles ํ์์ ์ ์ด์ฃผ์ธ์
  styles?: React.CSSProperties;
  // event๋ฅผ ๋งค๊ฐ๋ณ์๋ก ๋ฐ๊ณ , void๋ฅผ ๋ฐํํ๋ ํจ์ ํ์์ ์ ์ด์ฃผ์ธ์
  // event ํ์์ onClick={e => props.handleClick(e)}์์ e์ ๋ง์ฐ์ค๋ฅผ ์ฌ๋ฆฌ๋ฉด ํ์ธํ  ์ ์์ต๋๋ค
  handleClick: (event: React.MouseEvent) => void;
}

// 2. props๊ฐ ButtonProps์ children ์์ฑ์ ํจ๊ป ๊ฐ์ง ์ ์๋๋ก ํ์์ ์ ์ธํด์ฃผ์ธ์
export const Button: React.FC<ButtonProps> = (props) => {
  // 4. createButtonStyle ํจ์๋ฅผ ํธ์ถํ์ฌ buttonStyles ๊ฐ์ฒด๋ฅผ ์์ฑํ๊ณ  style props์ ์ ๋ฌํด์ฃผ์ธ์
  // 5. props์ handleClick์ onClick props์ ์ ๋ฌํด์ฃผ์ธ์
  const buttonStyles = createButtonStyle(props.styles);
  return (
    <button style={buttonStyles} onClick={props.handleClick}>
      {props.children}
    </button>
  );
};
```

### โ Hook์ ํ์ ์ ์ฉํ๊ธฐ
1. `useState` ์ ํ์ ์ ์ฉํ๊ธฐ

```tsx
function useState<S>(initialState: S | (() => S)) : [S, Dispatch<SetStateAction<S>>];
function useState<S = undefined>(): [S | undefined, Dispatch<SetStateAction<S | undefined>>];

const [name, setName] = useState(null)  // ์ด๊ธฐ๊ฐ์ผ๋ก state ํ์์ ๊ฒฐ์ 
const [name, setName] = useState()  // ์ด๊ธฐ๊ฐ์ด ์๋ค๋ฉด undefined๋ก ์ค์ 

// ์ด๊ธฐ๊ฐ ์ค์  ์ ์ด๊น๊ฐ์ ํ์์ ์ถ๋ก ํด์ state์ setState์ ํ์์ ๊ฒฐ์ 
// ์ด๊น๊ฐ๊ณผ ๋ค๋ฅธ ํ์์ ๋ฐ์ดํฐ๋ฅผ setState์ ์ธ์๋ก ๋๊ธธ ๊ฒฝ์ฐ ์๋ฌ
// ์ด๋ฐ ๊ฒฝ์ฐ useState์ ์ ๋ค๋ฆญ ํ์ ์ค์ : useState<string | null>(null)

import React, { useState } from "react";

export const TestScreen = () => {
	const [ name, setName ] = useState(null);

	const handleChange = (e: React.ChangeEvent<HTMLInputElement>) => {
		setName(e.target.value);  // ํ์ ์๋ฌ
	}

	return(
		<div>
			<input onChange={handleChange} />
		</div>
	)
}
```

2. `useReducer` ์ ํ์ ์ ์ฉํ๊ธฐ

```tsx
// ๋ฌธ์ ์ 
// ์๋ํ ํ์๊ณผ ๋ค๋ฅธ ํ์์ ๋ฐ์ดํฐ๋ฅผ case๋ก ์ถ๊ฐํด๋ ์๋ฌ๊ฐ ๋์ง ์์(ex case "CHANGEVALUE":)
// state๊ฐ ์ด๋ค ํ์์ธ์ง ์ ์ ์์
// action์ ์ด๋ค ํ๋กํผํฐ๊ฐ ์๋์ง ์ ์ ์์
// reducer์ ์ ๋ค๋ฆญ ํ์์ Reducer<any, any>๋ฅผ ํ์ฅํ๋ฏ๋ก ํ์์ ์ง์ ํ์ง ์์ผ๋ฉด state์ dispatch๋ any ํ์์ด ๋จ

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

// ํ์ ์ ์ฉํ๊ธฐ
// 1. state์ action type ์ ์ธ
// 2. Action type์ action์ ๊ตฌ๋ถํ  type์ธ์๋ ์์ ๋กญ๊ฒ ๊ตฌ์ฑ
// 3. score, dispatch๊ฐ ๊ฐ๊ฐ ScoreState, React Dispatch<ScoreAction>๋ก type ๊ฒฐ์ 
// ๋ฌธ์ ์ : action.type์์ increment, decrement ์ธ์ ๋ค๋ฅธ action.type์ด ์ค์ง ๋ชปํ๊ฒ ํด์ผ ํจ

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

// strict type ์ ์ฉํ๊ธฐ
// 1. ScoreAction์ type์ string union type์ผ๋ก ์ ์ธ
// 2. reducer์์๋ literal type guard๋ก ํ์๋ง๋ค ๋ค๋ฅธ ๋ก์ง ์คํ
// ๋ฌธ์ ์ : RESET ์ก์์ ๊ฒฝ์ฐ score๋ฅผ ๋ฐ๋ก ๋ฐ์ง ์์๋ ๋จ, ๊ทธ๋ฌ๋ Action ํ์์ ์ํด ์ ์๋ฅผ ๋ฃ์ด์ค์ผ ํจ

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

// ํด๊ฒฐ
// 1. ScoreAction์ score๋ฅผ optional๋ก ๋ฐ๊พธ๋ฉด RESET ์ก์์ ๊ฒฝ์ฐ score๋ฅผ ๋ฐ๋ก ๋ฐ์ง ์์๋ ๋๋ค.
// 2. ํ์ง๋ง, reducer์ case๋ฌธ์์ action.score๋ฅผ ์ฌ์ฉํ๋ ์ชฝ์์ ๊ฒฝ๊ณ ๋ฅผ ๋ฟ๋๋ค
// 3. ๋ฐ๋ผ์, ๊ตฌ๋ณ๋ ์ ๋์จ์ ์ผ์ฉํ์ฌ type์ ๋จ์๋ก score ํ๋๊ฐ ๋ค์ด๊ฐ์ง ์ ๋ค์ด๊ฐ์ง swtich๋ฌธ์์ type guard ํ๋๋ก ๋ง๋ ๋ค.

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
        ์ ๋ต
      </Button>
      <Button handleClick={() => dispatch({ type: "DECREMENT", score: 10 })}>
        ์ค๋ต
      </Button>
      <Button handleClick={() => dispatch({ type: "RESET" })}>์ด๊ธฐํ</Button>
    </div>
  );
};
```

### โ Context API์ ํ์ ์ ์ฉํ๊ธฐ
1. ํ์ ์ ์ฉ ์ 

```tsx
// ScoreContext.ts
import React from "react";

export const ScoreContext = React.createContext({
	score: 0,
	dispatch: () => {}  // ์๋ฌ ์ ๋ฐ
})

// App.tsx
...
const [ counter, dispatch ] = React.useReducer(reducer, { score: 0 });
<ScoreContext.Provider value={{ score: counter.score, dispatch }}  // ํ์ ์๋ฌ(๊ตฌ์ฒด์ ์ธ ์ก์์ด ์ฌ์ฉ๋์ด์ผ ํจ)
```

2. ํ์ ์ ์ฉ ํ

```tsx
// 1. createContext๋ ์ด๊น๊ฐ์ ๋ํ ํ์์ ์ ๋ค๋ฆญ์ผ๋ก ๋ฐ๋๋ค
// 2. Context์ value์ ๋ํ ํ์์ ์ ์ธํ ๋ค ์ ๋ค๋ฆญ์ ํ์ ํ๋ผ๋ฏธํฐ์ ๋ฃ์ด์ฃผ๋ฉด ๋๋ค.

import React from "react";
import { ScoreAction } from "../reducers/ScoreCounterReducer";

interface ScoreContextValue {
	score: number;
	dispatch: Dispatch<ScoreAction>;
}

export const ScoreContext = React.createContext<ScoreContextValue>({
	score: 0,
	dispatch: () => {}  // ์๋ฌ ์ ๋ฐ
})
```

### โ ํ์์คํฌ๋ฆฝํธ์ ๋ฆฌ์กํธ ์ํ ๊ด๋ฆฌ: Redux
1. `npm i redux @reduxjs/toolkit react-redux @types/react-redux`

```tsx
1. react, typescript์ ํจ๊ป ์ฐ๊ธฐ ์ํ redux ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ค์ ์ค์น
2. @reduxjs/toolkit์ RootState์ Dispatch ํ์์ ์ถ์ถํ๋๋ฐ ์ฌ์ฉ
3. react-redux์ ๊ฒฝ์ฐ ํ์ ์ ์ธ ํ์ผ์ด ์์ด @types ํจํค์ง๋ฅผ ๋ฐ๋ก ์ค์น ํด์ผ ํจ
```

2. `redux toolkit`

```tsx
// configureStore: redux์ createStore๋ฅผ ์ฌ์ฉ์ฑ ๋๊ฒ ํ ๋ฒ ๋ ์ถ์ํํ ๊ฒ
// redux์ combineReducers๋ฅผ ์ฐ๋ ๊ฒ๋ณด๋ค RootState, AppDispatch, AppThunk ๋ฑ ํ์ ์ถ๋ก ์ด ๋ ์ฌ์์ง

// Reducers/store.ts
import { configureStore, ThunkAction, Action } from "@reduxjs/toolkit";

export const store = configureStore({
	reducer: { scoreCount },
})

export type AppDispatch = typeof store.dispatch;
export type RootState = ReturnType<typeof store.getState>;  // RootState๋ผ๊ณ  ํ๋ ์ด์ ๋ configureStore์์ ๋ชจ๋  ๋ฆฌ๋์๋ฅผ ํ๊ณณ์์ ๊ด๋ฆฌํ๊ธฐ ๋๋ฌธ์ rootState๋ผ๊ณ  ํํํ๋ค.
export type AppThunk<ReturnType = void> = ThunkAction<
	ReturnType,
	RootState,
	unknown,
	Action<string>,
>;

// selector: reducer์ state ์ถ์ถ(rootState์์ ์ํ๋ state๋ฅผ ์ถ์ถ)
// dispatch: reducer์ dispatch ์ถ์ถ
// useAppDispatch, useAppSelector: app์ ๋ชจ๋  dispatch, selector ๊ฐ์ ์ฌ์ฉํ  ์ ์๊ฒ ํ๋ hook
// TypedUseSelectorHook: ํน์  State์ ๋ํ ํ์ดํ์ด ๋ useSelector๋ฅผ ์์ฑํ  ์ ์์
import { TypedUseSelectorHook, useDispatch, useSelector } from "react-redux";
import type { RootState, AppDispatch } from "./store";

export const useAppDispatch = () => useDispatch<AppDispatch>();
export const useAppSelector: TypedUseSelectorHook<RootState> = useSelector;

// redux store ์ ์ฉ์ ์ํ provider ์ฌ์ฉ
import { Provider } from "react-redux";
import { store } from "./reducers/store";

ReactDOM.render(
	<React.StrictMode>
		<Provider store={store}>
			<App />
		</Provider>
	</React.StrictMode>
)

// useAppSelector: TypedUseSelectorHook๋๋ถ์ RootState์์ ์๋ ์์ฑ์ ํตํด ํน์  reducer์ ๋ํ state ์ถ์ถ ๊ฐ๋ฅ
// useAppDispatch: ์ ์ญ์์ ๊ด๋ฆฌ๋๋ dispatch ์ฌ์ฉ
// dispatch({ type: "scoreCounter/RESET" }): ๋ค๋ฅธ reducer์ ํจ๊ป ์ฐ์ด๊ธฐ ๋๋ฌธ์ reducer์ ์ด๋ฆ์ ์์ ๋ถ์ฌ์ ๊ตฌ๋ถํด์ฃผ๋ ๊ฒ์ด ๊ด์ต.

import { useNavigate } from "react-router-dom";
import { Button} from "../../componennts/Button";
import { useAppSelector, useAppDispatch } from "../../reducers";

export const ResultScreen = () => {
	const score = useAppSelector((state) => state.scoreCounter.score);
	const dispatch = useAppDispatch();
	const navigate = useNavigate();
	const handleReset = () => {
		dispatch({ type: "scoreCounter/RESET" })  // ๋ค๋ฅธ reducer์ ์ฌ์ฉํ์ ๋ type์ด ๊ฒน์ณ action์ด ํผ์ฉ๋๋ ๊ฒ์ ๋ฐฉ์งํ๊ธฐ ์ํด prefix๋ฅผ ๋ถ์๋๋ค. ํ์์ ๊ฐ์ ํ๋ ๊ฒ์ ์๋. RESET์ด๋ผ๊ณ ๋ง ์จ๋ ํ์ ์๋ฌ๋ ๋์ง ์์ต๋๋ค.
		navigate("/");
	};

	return(
		<div>
			...
		</div>
	)
}
```

### โ ํ์์คํฌ๋ฆฝํธ์ ๋ฆฌ์กํธ ์ํ ๊ด๋ฆฌ: Jotai
1. `redux`: ์๋ฐ์คํฌ๋ฆฝํธ ์ฑ์์ ์ฌ์ฉ ๊ฐ๋ฅํ๊ณ , ๋ฆฌ์กํธ ์ํ๊ณ์์ ๊ฐ์ฅ ๋ง์ด ์ฐ์ด๋ ์ํ ๊ด๋ฆฌ ๋ผ์ด๋ธ๋ฌ๋ฆฌ
2. `recoil`: ๋ฆฌ์กํธ ํ์์ ๋ง๋  ์ํ ๊ด๋ฆฌ ๋ผ์ด๋ธ๋ฌ๋ฆฌ
3. `Jotai`: `recoil` ์ `atomic model` ๊ธฐ๋ฐ์ ์ํฅ์ ์ ๊ทผ์ ์๊ฐ์ ๋ฐ์ ๋ง๋  ์ํ ๊ด๋ฆฌ ๋ผ์ด๋ธ๋ฌ๋ฆฌ

![](https://images.velog.io/images/abcd8637/post/b42b3cbe-6090-454a-a966-4308afcb818e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-01-24%2013.48.40.png)

### โ Jotai์ ์ฌ์ฉ๋๋ ๊ฐ๋
1. `Atom`: ์ํ๋ฅผ ๋ํ๋ด๋ ๋จ์, `recoil` ๊ณผ ๋ฌ๋ฆฌ `atom` ์ ์์ฑํ  ๋ ์ฌ์ฉ๋๋ ๋ฌธ์์ด `key` ๊ฐ ํ์ ์๋ค.
2. `config`: `atom`์ ์์ฑํ  ๋ ๋ฃ์ด์ฃผ๋ ์ด๊น๊ฐ
3. `Provider`: `Atom` ์ด ์ฐ์ด๋ ๋ฒ์(scope)๋ฅผ ๋๋ ๋ ์ฌ์ฉ
4. atom, hook ์์ฑ

```tsx
import { atom } from "jotai";

export const scoreAtom = atom(0);  // scoreAtom์ state์ฒ๋ผ ์ฌ์ฉ๋จ
```

5. `useAtom` ์ ์ฌ์ฉํ `custom hook`

```tsx
// useAtom์ ์ฌ์ฉํด useState์ฒ๋ผ ์ฌ์ฉ ๊ฐ๋ฅ
// setScore๋ฅผ consumer(state๋ฅผ ๊ฐ์ ธ๋ค ์ฐ๋ ์ชฝ)์์ ํ์์ ๋ฐ๋ผ setScore๋ก ๋งค๋ฒ ๊ฐ์ ์ฝ๋๋ฅผ ๋ฐ๋ณตํด์ผ ํจ
// ๋ฐ๋ผ์, custom hook์ ๋ง๋ค์ด์ dispatcher์ฒ๋ผ ์ฌ์ฉ
// custom hook์์ use<hook์ด๋ฆ>์ hook ๋ค์ด๋ฐ ์ปจ๋ฒค์์ด๋ฏ๋ก ๋ฐ๋ผ์ผ ํจ

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

6. `useScoreHook` ์ฌ์ฉ

```tsx
// screens/ResultScreen 
// ์์ฑํ custom hook์ importํด์ ์ฌ์ฉ

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
## ๐ 66์ผ์ฐจ 1.25.ํ.(14์ฃผ์ฐจ 2์ฐจ ํ ํ๋ก์ ํธ)
์ค๋๋ถํฐ ์๋ฆฌ์ค ๊ต์ก์ด ๋๋๋ 2์ 20์ผ๊น์ง๋ 2์ฐจ ํ ํ๋ก์ ํธ ๊ธฐ๊ฐ์ด๋ค. ์๋ ํฌ๋ฆฌ์ค๋ง์ค์ 1์ฐจ ํ ํ๋ก์ ํธ๋ฅผ ๋๋๋๋ฐ, ๋ฒ์จ 2์ฐจ ํ๋ก์ ํธ๋ผ๋.. ์๊ฐ์ด ์ฐธ ๋น ๋ฅธ๊ฒ ๊ฐ๋ค. ์๋ง๋ ๋์ ๊ธฐ์ต๋ ฅ์ด ์ข๋ค๋ฉด ์ง๊ธ๊น์ง ๋ฐฐ์ด๋ด์ฉ๋ค์ ๊ธฐ์ตํ๊ฒ ์ง๋ง, ๊ทธ๋ ์ง ๋ชปํ๊ธฐ์ ์ง๊ธ๊น์ง ๋จ๊ฒจ๋์ ์ฝ 66๊ฐ์ ๊ธฐ๋ก๋ค์ ๋ณด๋ฉฐ ๋ ์ฌ๋ ค์ผ๊ฒ ๋ค. ์ด๋ฒ์ ํ์์ด ์๋๋ผ ํ์ฅ์ผ๋ก์ ํ๋ก์ ํธ๋ฅผ ์งํํ๋๋ฐ, ๋ง์๊ฐ์ง์ ๋ค๋ฅด๊ฒ ๊ฐ์ ธ์ผ๊ฒ ๋ค๊ณ  ์๊ฐํ๋ค. ๋ํ ์ ๋ฒ ํ๋ก์ ํธ์ ํ์์กฐ์น๋ก `webpack`์ ๊ณต๋ถํ๋๋ฐ, `React`๋ฅผ ์ด์ฉํด ๊ฐ๋ฐํ  ๋ `CRA`๊ฐ ์๋ ์ง์  `webpack`์ ์ด์ฉํด์ ํ๋ก์ ํธ๋ฅผ ๊ตฌํํด์ผ๊ฒ ๋ค๊ณ  ๋ง์๋จน์๋ค. ๊ทธ๋ฆฌ๊ณ  ๋ ํ๊ฐ์ง ๋ณ์๊ฐ ์๊ฒผ๋๋ฐ, ๋ฐ๋ก ๋ฐฑ์๋๋ฅผ ๋งก๊ฒ ๋์๋ค. ์ฒ์๋ถํฐ ๋ฐฑ์๋๋ฅผ ๋งก๊ฒ ๋ค๊ณ  ํ๊ฒ์ ์๋์๊ณ , ์๋๋ ํ๋ก ํธ๋ก ์ญํ ์ ๋ฐฐ์ ๋ฐ์์ง๋ง, ํ ๋ฏธํ ๋ ํ์ ๋ชจ๋ ๋ฐฑ์๋๋ฅผ ์์ฃผ ๋ค๋ค๋ณด์ ๋ถ์ด ์๋ค๊ณ  ํ์์ ๋ด๊ฐ ๋ฐฑ์๋๋ฅผ ๋ค๋ฃจ๊ฒ ๋ค๊ณ  ์๊ธฐํ๋ค. ์ง๊ธ๊น์ง ํญ์ ํ๋ก ํธ๋ง ๋ค๋ค์์ ๋ฐฑ์๋๋ ํ  ์ค ๋ชจ๋ฅด๋ ๋ด๊ฐ ์ ํ  ์ ์์์ง๋ ๋์กฐ์ฐจ๋ ์๋ฌธ์ด๋ค. ๋๊ตฐ๊ฐ๋ ๋ญํ๋ฌ ์๋ฌด๋ ์ ํ์ํ๋ ํฌ์ง์์ ํ๋ ค๊ณ  ๋น์๊ฒ ์ง๋ง, ๋ด๊ฐ ์ํ๋ฉด ๋๊ตฐ๊ฐ๋ ํด์ผ๋๋ ๋ถ์ผ๊ณ  ํ๊ธฐ ์ซ์ ์ฌ๋์ด ์ต์ง๋ก ํ๋๊ฒ๋ณด๋ค๋ ์ฐจ๋ผ๋ฆฌ ํ๊ณ  ์ถ์ ์ฌ๋์ด ํ๋๊ฒ ๋ซ๋ค๋ ์๊ฐ์ด ๋ค์๋ค. ํญ์ ๊ฐ์ธ ํ๋ก์ ํธ๋ฅผ ํ๋ฉฐ ๋ฐฑ์ ๋ค๋ฃจ๊ธฐ ์ซ์ด ๋ผ์ด๋ธ๋ฌ๋ฆฌ์ ์์งํ๋ค๋ฉด ์ด๋ฒ์ ์ง์  ๋ถ๋ชํ๋ณด๊ณ ์ถ๋ค๋ ์๊ฐ๋ ๋ค์๋ค. ์ ๊ทธ๋ฌ๋์ง ๋ค์ ์๊ฐํ๋ฉด ํ์์๋ง ๋์ค์ง๋ง ์ด๋ฏธ ์์ง๋ฌ์ง ๋ฌผ์ด๊ธฐ์.. ํ๋ฒ ๋์ ํด๋ณผ๊น ํ๋ค. ์ฌ์ฉ ์คํ์ `express + MondoDB`์ธ๋ฐ, ์ด์ ์ ๋ค์๋ ์๋ฆฌ์ค ๊ฐ์์์ ์ถ๊ฐ๋ก ์์์ผ๊ฒ ๋ค๊ณ  ๋ง์๋จน๊ณ  ์๋ผ๋์์ <a href='https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=269942241'>๊ด๋ จ ์์ (ํ ๊ถ์ผ๋ก ๋๋ด๋ Node & Express)</a>์ ๊ตฌ๋งคํ๋ค. (์๊ฐ๋ณด๋ค `express` ๊ด๋ จํ ์์ ์ด ์์๋ค.) ์ด์  ๋ฌด๋ชจํ ๋์ ๊ฒฐ์ ์ 3์ฃผ๋์ ๊ธฐ๋กํด๋๊ฐ๋ณด์..

### โ ๊ฐ๋ฐ์์ ์ญ๋
1. `์ํต์ญ๋`: ๋ค๋ฅธ ๊ฐ๋ฐ์์ ์๊ฒฌ์ ๊ฒฝ์ฒญํ๊ณ , ์๊ฒฌ์ ์๋์ ํต์ฌ์ ์ดํดํ ํ, ์์ ์ ๊ด์ ์ ๋ชํํ๊ณ  ๋ผ๋ฆฌ ์ ์ฐํ๊ฒ ์ค๋ชํ๋ ๊ฒ์๋๋ค. ์์ ๊ณผ๋ ๋ค๋ฅธ ์๊ฒฌ, ์๋ก์ด ๊ด์ ์ ํ์ํ๊ณ  ๋ ๋์ ๋ฐฉํฅ์ผ ๊ฒฝ์ฐ ๊ฒธํํ๊ฒ ๋ฐ์๋ค์๋๋ค. (๋ง๋ณด๋ค๋ ์ฝ๋๋ก ์ํตํ๋ผ)
2. `์๊ฐ, ํ์คํฌ ๊ด๋ฆฌ ๋ฅ๋ ฅ`: ํน์  ํ์คํฌ๋ฅผ ์ํด ์์๋  ์๊ฐ์ ์ ํํ๊ฒ ํ์ํ  ์ ์๊ณ , ์ด๋ฅผ ๋ฐํ์ผ๋ก ๋ค๋ฅธ ๊ฐ๋ฐ์์ ์ํตํ์ฌ ์ผ์  ๊ด๋ฆฌ๋ฅผ ํฉ๋๋ค. ์ฌ์ ์ ์ ํ ์ผ์ ์ ๋ฐ๋์ ์งํค๋ฉฐ, ์งํค๊ธฐ ์ด๋ ค์ด ๊ฒฝ์ฐ ๋ฏธ๋ฆฌ ์ํตํ์ฌ ์ํ๋ผ์ด์ฆ๋ฅผ ์ค์๋๋ค. (ํน์  ๋ถ๋ถ์ ๋ถ๊ฐ์ํค๊ณ  ๋ค๋ฅธ ๋ถ๋ถ์ ํฌ๊ธฐํ๋ค๋ ์ง..)
3. `๋ผ๋ฆฌ๋ ฅ`: ์ฌ์ฉํ๋ ๊ธฐ์  ์คํ๊ณผ ์ฝ๋์ ์์ฑ ๋ฐฉ์์๋ ๋ผ๋ฆฌ๊ฐ ํ์ํ๋ค. (์ฃผ์ด์ง ๋ชฉํ๋ฅผ ๋ ํจ๊ณผ์ ์ผ๋ก ๋ฌ์ฑํ๊ธฐ ์ํ ๊ฐ๋ฐ ๋ฐฉํฅ์ด์ด์ผ ํ๋ค.), ์ ์ด ๊ธฐ์  ์คํ์ ์ ํํ๋์ง? ์ ์ด๋ฐ ์ฝ๋๋ฅผ ๊ตฌ์ฑํ๋์ง๋ฅผ ๋ผ๋ฆฌ์ ์ผ๋ก ์ค๋ชํ  ์ ์์ด์ผ ํ๋ค.
4. `ํ์ต๋ฅ๋ ฅ`: ํน์  ์ธ์ด, ํน์  ํ๋ ์์ํฌ์์ ๋ฒ์ด๋๋๋ผ๋ ๊ฐ๋ฐํ  ์ ์๋ ๋ฅ๋ ฅ์ ๊ฐ์ถ์ด์ผํฉ๋๋ค. ๊ธฐ๋ณธ๊ธฐ์ ๋ฌธ์  ํด๊ฒฐ ๋ฅ๋ ฅ์ ๊ฐ์ถ๋ฉด, ์ธ์ด์ ํ๋ ์์ํฌ๊ฐ ๋ฐ๋๋๋ผ๋ ๋ฐ๋ก ๋์ํ  ์ ์์ต๋๋ค. ๊ฐ๋ฐ ๊ณผ์ ์์ ์ถ๊ฐ์ ์ผ๋ก ๊ธฐ์  ์คํ, ์ธ์ด๊ฐ ์๊ธด ๊ฒฝ์ฐ, ์งง์ ์๊ฐ ๋ด์ ์ค์ค๋ก ๋ฐฐ์ธ ์ ์์ด์ผ ํฉ๋๋ค.

### โ ์ข์ ์ฝ๋๋?
1. ๊ฐ๋์ฑ: ์ฝ๋๋ฅผ ์ฝ์ผ๋ฉด์ ์ฝ๊ฒ ์ดํดํ  ์ ์๊ณ , ์๋๋ฅผ ์ดํดํ๊ธฐ ์ํด ๊ณ ๋ฏผํ์ง ์์๋ ๋๋ ์ฝ๋
2. ์ผ๊ด์ฑ: ์ฌ์ ์ ์ ํ ์ผ๊ด๋ ๊ท์น์ ๋ฐ๋ผ์ผ ํฉ๋๋ค.

### โ GitLab ํ์ฉ๋ฒ(Git Flow)
1. `README.md`: ํ๋ก์ ํธ๋ฅผ ๊ด๋ฆฌํ๋ ๋ชฉ์ , ํ์ํ ์ ๋ณด๋ค๋ง ์์ฑํ๊ธฐ
2. `Issue`: ํ๋ก์ ํธ ์งํ ์, ์ด๋ ํ ์ํฉ, ๋ฌธ์  ๋๋ ๊ณํ์ ๊ฐ๋ฐ ํ  ์์ ์ด๋ผ๋ ๊ฒ์ ์๋ ค์ฃผ๋ ์ด์ ํ ํด์ผ ํ  ์ผ์ ์ด์๋ก ์ ๋ฆฌํ์
3. `MR`

```
- Matser Branch(Main branch): ์๋น์ค๋ก ์ถ์๋  ์ ์๋ ๋ธ๋์น, ๋ฐฐํฌ ๊ฐ๋ฅํ ์ํ์ ์ฝ๋๋ฅผ ๊ด๋ฆฌ
- Sprint Branch: ๋ชจ๋  ๊ธฐ๋ฅ์ด ์ถ๊ฐ๋๊ณ  ๋ฒ๊ทธ๊ฐ ์์ ๋์ด ๋ฐฐํฌ ๊ฐ๋ฅํ ์ํ๋ผ๋ฉด MR
- Feature Branch: ์๋ก์ด ๊ธฐ๋ฅ ๊ฐ๋ฐ ๋ฐ ์์ ํ๋ ๋ธ๋์น, ์์์ด ๋๋ ๊ธฐ๋ฅ์ Sprint๋ก MR!
```

---
## ๐ 67์ผ์ฐจ 1.26.์ ํ๋ก์ ํธ 2์ผ์ฐจ TL;DR
์ค๋๋ถํฐ 2์ฐจ ํ๋ก์ ํธ๊ฐ ๋๋๋ ๋ ๊น์ง ๊ธ์ ๊ธธ๊ฒ ์ฐ์ง ์๊ณ  ๊ทธ๋  ๋ฐฐ์ด๋ด์ฉ์ด๋ ๋๊ผ๋ ์ ๋ค์ ๋์ดํ๊ฒ ๋ค.

1. `configuration`: `secretKey`์ ๊ฐ์ ๊ฐ๋ค์ ์์ค์ฝ๋์ ํฌํจํ์ง ์๊ณ , `local`์์ ๋ณด๊ดํ๋ค. ์ด๋, `dotenv`๋ฅผ ์ด์ฉํ๋ฉด ์ฝ๊ฒ `config` ํ์ผ์ ์์ฑํ  ์ ์๋ค.
2. `express` ์๋ฌ์ฒ๋ฆฌ: ๋๊ธฐ์ ์ผ๋ก๋ ๋ง์ง๋ง `use`๋ก ๋์ด๊ฐ์ง๋ง ๋น๋๊ธฐ์ ์ธ ์ฒ๋ฆฌ์์๋ ์ฝ๋ฐฑํจ์ ๋ด์์ ์๋ฌ์ฒ๋ฆฌ๋ฅผ ํด์ผํ๋ค.
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

6. `morgan`: ์์ฒญ์ ์ด๋ค ์์ฒญ์ ๋ฐ์๋์ง, ์ผ๋ง๋ ๊ฑธ๋ ธ๋์ง log๋ฅผ ๋จ๊ฒจ์ฃผ๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ
7. `helmet`: ๋ณด์์ ํ์ํ ํค๋๋ฅผ ์ถ๊ฐํด์ค๋ค.

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
## ๐ 68์ผ์ฐจ 1.27.๋ชฉ ํ๋ก์ ํธ 3์ผ์ฐจ TL;DR
### โ JWT ํ ํฐ ์ธ์ฆ ํ๋ฆ
<a href='https://www.youtube.com/watch?v=p09YODnkSO8&list=PLanIiKDTgXLy4cZc5Ahfi_x443ZVKXb_5&index=12'>DFSW Labs Youtube ๊ฐ์</a>

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
14. token ํ์ธ ํ : then we tried to access a protected route we first did it without the token. you saw it was authorized then we added correct token and now responding with the user data

---
## ๐ 69์ผ์ฐจ 1.28.๊ธ. ํ๋ก์ ํธ 4์ผ์ฐจ TL;DR
1. ๋ฐฑ์๋ ์ธ์ฆ ๋ก์ง: GitHub login -> GitHub ์ ๋ณด ํ๋ -> JWT ํ ํฐ ์์ฑ -> ์ฟ ํค๋ก client ์ ๋ฌ -> ๋ก๊ทธ์ธ ํ์ํ ์๋น์ค์์ JWT ๊ฒ์ฆ(๊ฒ์ฆ์ req.user์๋์ง ํ์ธ)
2. React CRA ์ค์ ์ override ํ๊ณ  ์ถ์ผ๋ฉด React-app-rewired
3. redux์ฒ๋ผ API๋ฅผ ์ค์์์ ๊ด๋ฆฌํ๊ณ  ์ถ๋ค๋ฉด react-query ์ฌ์ฉ
4. rebase์ ์ฅ. ๋จ์ : merge commit ์ด ์์ด์ ธ history ๊ฐ ๊น๋ํด์ง, ๋ฐ๋๋ก history ๊ฐ ์์ด์ ธ commit ์ด๋ ฅ์ด ๋จ์ง ์์ confilct ๊ฐ ๋๊ธฐ ์ฝ๋ค. `Git`์ ์๋ จ๋์ ๋ฐ๋ผ `rebase` ๋์ ์ฌ๋ถ๋ฅผ ๊ณ ๋ฏผํ๊ธฐ
5. browser์์ mobile device ํ์ธํ๋ ๋ฐฉ๋ฒ: device-width, user-agent
6. ๋ชจ๋ฐ์ผ์ ์ฌ์ฉ์ฑ์ ๋ง์ท๊ธฐ ๋๋ฌธ์ ๋ฐ์ํ ์น ๋์์ธ์์ ๋ชจ๋ฐ์ผ, ํ๋ธ๋ฆฟ๊น์ง๋ง ๋์ํ๊ธฐ
7. redux๋ state๋ฅผ ์ค์์์ ๊ด๋ฆฌํ  ์ ์๋ค๋ ์ฅ์ ์ด ์์ผ๋, boilerplate์ ์์ฑ์ด ์ค๋๊ฑธ๋ฆฐ๋ค. ํ๋ก์ ํธ์ ๊ธฐ๊ฐ์ด ๊ธธ์ง ์๊ธฐ ๋๋ฌธ์ ํ์ด์ง๋ณ๋ก ์ํ๋ฅผ ๊ด๋ฆฌํ๋ ๋ฐฉ๋ฒ์ ์ฌ์ฉํ์.
8. ์ ํต์ ์ธ flow๋ back์์ api๋ฅผ ๋ด๋ ค์ฃผ๋ ๋ฐฉ๋ฒ์ ์ฌ์ฉํ์ผ๋, ์ต๊ทผ์๋ back์ผ๋ก ํ์ ์ง์ง ์๊ณ  front์์๋ api๋ฅผ ํธ์ถํ์ฌ ์ฌ์ฉํ๋ค.
9. `branch`์ `feature-TODO`๋ง๋ค๊ณ , issue์๋ TODO ๋จ๊ธฐ๊ธฐ (cross-check)
10. React-query๋ฅผ ๋์ํ์ฌ API๋ฅผ ์ค์์์ ๊ด๋ฆฌํ๋ ์์ผ๋ก ๊ตฌํํ๋ฉด ๋ฐ์คํฌํ ๋ฒ์ ์์๋ ๋ฌธ์ ๊ฐ ์์ ๊ฒ์ผ๋ก ๋ณด์๋๋ค. API.js์ API๋ฅผ ๋ชจ์๋๊ณ , ํธ์ถํ๋ ๋ถ๋ถ์์ React-query๋ฅผ ์ด์ฉํ๋ฉด ์ํํ  ๊ฒ์๋๋ค.
11. ๊ฒ์ ๊ธฐ๋ฅ์ ๊ตฌํํ  ๋, ์๋ฒ์ ๋ณด๋ผ๊ฑด์ง ํ๋ก ํธ์์ ์ฒ๋ฆฌํ ๊ฑด์ง์ ๋ฐ๋ผ ๋๋ฉ๋๋ค. ๋ญํฌ ์ ๋ณด๋ ๋ฐฑ์๋์์ ์ฒ๋ฆฌํ๋ฉด ๋๊ณ , mongoDB ์ฟผ๋ฆฌ๋ฅผ ๋ ๋ฆฌ๋ ์๊ฐ์ ์์๋ฅผ sorting ํ๋ฉด ๋ฉ๋๋ค.
12. Router -> mobile์์ PCํ๋ฉด์ผ๋ก ๊ฐ ๋ ๊ณ ๋ฏผํด๋ณด์์ผ ํ  ๊ฒ ๊ฐ์ต๋๋ค. (ex: rank ํ์ด์ง์์ ํ๋ฉด์ ํ์ฅํ์ฌ PC๋ฒ์ ์ด ๋์์ ๋๋ /rank์ ์๋ฏธ๊ฐ ์์ด์ง๊ธฐ ๋๋ฌธ)
13. ์ฐจํธ -> ๋ฌผ๋ก  ์ง์  ๊ณต๋ถํ๋ฉด์ ๊ตฌํํ๋ฉด ์ข๊ฒ ์ง๋ง, ์๊ฐ์  ๋น์ฉ์ ์ค์ด๊ธฐ ์ํด ์ฐ์ ์ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ฅผ ์ด์ฉํ์ฌ ์์ฑํ๊ณ  ์ถํ์ ์๊ฐ์  ์ฌ์ ๊ฐ ์์ ๋ ์ง์  ๊ตฌํํด๋ณด๋ฉด ์ข์ ๊ฒ ๊ฐ์ต๋๋ค.

---
## ๐ 70์ผ์ฐจ 1.29.ํ . ํ๋ก์ ํธ 5์ผ์ฐจ TL;DR
1. `firebase`๋ก ๊ฐ๋จํ๊ฒ ์์ ์ฌ์ด์ฆ์ ํ๋กํ ํ์์ ๋ง๋ค ๋ ๋น ๋ฅด๊ณ  ์ฝ๊ฒ ์ฌ์ฉํ  ์ ์๋ ์ข์ ์คํ์ด์ง๋ง, ํ์์์๋ `MERN` ์คํ๋ ์ฌ์ฉํ๋ ๊ณณ์ด ๋ง๋ค. ๊ณต๋ถํ๋ ์์ฅ์์ `MERN` ์คํ์ ์ฌ์ฉํ๋ค๋ฉด ๋ฐฑ๊ณผ ํ๋ก ํธ์ ์ ๋ฐ์ ์ธ ํ๋ฆ๋ ์ ์ ์๊ณ , `web framework`๋ฅผ ์ฌ์ฉํ๊ฒ ๋  ์ํฉ๋ ๋ง๊ณ , ํ์ฅ์ฑ์ธก์์๋ `MERN` ์ฌ์ฉํ๋ ๊ฒ์ ์ถ์ฒํ๋ค.
2. ํ์ ์ธ์ฆ, ๊ถํ ๊ตฌํ ํ  ๋ `cookie`๋ฅผ ์ฌ์ฉํ๋ฉด ๋ฏธ๋ค์จ์ด์ ๋ฌด์กฐ๊ฑด `cookie-parser`๋ฅผ ์ค์นํ์.. ์ด๊ฒ๋๋ฌธ์ 2์๊ฐ ๊ณ ์ํจ..
3. ํ๋ก ํธ์์ `API`๋ฅผ ๊ฐ์ ธ๋ค ์ฌ์ฉํ  ๊ฒฝ์ฐ. ๋ง์ฝ์ `API`๊ฐ ์๋ฌ๊ฐ ๋์ ์ ์์ ์ธ `data`๋ฅผ ๊ฐ์ ธ์ค์ง ๋ชปํ  ๋๋ ์ด๋ป๊ฒ ์ฒ๋ฆฌํ  ๊ฒ์ธ๊ฐ? 404ํ์ด์ง๋ก ์ด๋ ์ํฌ์๋ ์์ง๋ง ๋ฐฑ์ ๋ฏธ๋ฆฌ ์ ์ฅ๋์ด์๋ `db`์์ ๊ฐ์ ๋ด๋ ค์ค๋ ๋๋ค.
4. `Backend`์์ `API`๋ฅผ ๊ฐ๊ณตํ ๋ค์์ ์ฒ๋ฆฌํ์. ํ๋ฉด์์ ๊ฐ๊ณตํด์ผ ํ๋ ๋ฐ์ดํฐ๋ค์ด ์ฌ์ฉํ๋ `API`๋ค๋ง์ผ๋ก ๊ฐ๋ฅํ์ง ์์ ๊ฒฝ์ฐ๊ฐ ์์ ์ ์์ด์ ํ์ํ `API` ๋ด์ฉ๋ค์ ๋ฐ์์ฃผ๊ณ , ๊ฐ๊ณตํด์ `Frontend`๋ก ๋ด๋ ค์ฃผ๋ ๊ฒ์ด ์ข์ ๊ฒ ๊ฐ๋ค.
5. API์ฒ๋ฆฌ ๋ก์ง: ํด๋ผ์ด์ธํธ -> ์๋ฒ(์ปค๋ฐ ์ ์์ฒญ) -> ์๋ฒ์์ API์์ฒญ -> ๋ฐ์์จ ์ ๋ณด๋ก DB ๊ฐฑ์  -> ํด๋ผ์ด์ธํธ์๊ฒ ์๋ต
6. ์ธ์ฆ / ๊ถํ ํ์ด์ง ๋ก์ง

```
1. ๊ถํ: `client`์ `JWT` ํ ํฐ ๊ฐ์ `cookie`์ ๋ด์ `server`๋ก ๋ณด๋. -> ํ ํฐ์ด ๋ง๋ฃ๋์๊ฑฐ๋ ์ผ์นํ์ง ์์ผ๋ฉด `status(401)`๋ฆฌํด
2. ์ธ์ฆ: `GitHub OAuth` -> `db`์์ ํด๋น `id`์ ์ผ์นํ๋ `id`๋ฅผ ์ฐพ๊ณ  ์์ผ๋ฉด ์๋ก ๋ง๋ค์ด์ ์ ์ฅ -> `cookie`๋ก `JWT`ํ ํฐ ๊ฐ `browser`๋ก ์ ์ก
```

7. ์๋ฒ๋ ํ๋ก ํธ์์ ์์ฒญํ ๊ฒฐ๊ณผ๊ฐ ์ฌ๋ฐ๋ฅธ์ง ์๋์ง๋ฅผ ๊ฒฐ๊ณผ๊ฐ์ผ๋ก๋ง ๋ด๋ ค์ค๋ค. ๊ทธ๋ฆฌ๊ณ  ํ๋ก ํธ์์ ๊ฒฐ๊ณผ๊ฐ์ ํ ๋๋ก ๋ค์ ๋ก์ง์ ๊ตฌ์ฑํ๋ค.
8. ํ๋ก ํธ์ `json`ํํ๋ก ๊ฐ์ ๋ด๋ ค์ค๊ฑฐ๋ฉด `res.send` ๋์  `res.status(200).json({ isOk: true, postId });`์ ๊ฐ์ ํํ๋ก ๋ด๋ ค์ฃผ์. `res.status(200).json`์ `json` ํํ๋ก ๋ด๋ ค์ค๋ค๋ ์๋ฏธ๊ฐ ํฌํจ๋์ด์์ผ๋, `res.send`๋ ์๋ฏธ๊ฐ ๋ถ๋ชํํ๋ค. ๋ํ, `res.send`๋ก ์ ์กํ๊ฒ๋๋ฉด ๋ถํ์ํ ํจ์๋ฅผ ํ๋ฒ ๋ ํธ์ถํ๊ฒ ๋๋ค. ์ฐธ๊ณ (<a href='https://haeguri.github.io/2018/12/30/compare-response-json-send-func/'>harguri.github.io</a>)

---
## ๐ ๋ฐฉํ 2. 3. ๋ชฉ
1. ๋ฐฑ์๋์ ํด๋ ๊ตฌ์กฐ๋ ๋ณดํต ์ด๋ค์์ผ๋ก ๊ตฌ์ฑํ๋์ง ์ ํฌ๋ธ์`MERN` ์คํ์ ์ฌ์ฉํ ์์์ ๋ง์ด ์ฐพ์๋ณด๊ณ  ๋๋ฆ์ ํด๋ ๊ตฌ์กฐ๋ฅผ ๋ง๋ค์๋ค. ์ง๋๋ฒ ํ๋ก์ ํธ์์ ๋ฐฑ์๋๋ฅผ ๋ด๋นํ์  ์ธ์๋๊ป์ ์์ฑํ์  ํด๋๊ตฌ์กฐ๊ฐ ๋ง์ ๋์์ด ๋์๋ค.(๊ฐ์ฌํฉ๋๋ค.)

```
โโโ config
โ   โโโ db.js
โ   โโโ keys.js
โโโ middleware
โ   โโโ error-handler.js
โโโ model
โ   โโโ index.js
โ   โโโ schema
โ       โโโ User.js
โโโ package-lock.json
โโโ package.json
โโโ passport
โ   โโโ index.js
โ   โโโ strategy
โ       โโโ GitHub.js
โโโ routes
โ   โโโ api
โ   โ   โโโ auth.js
โ   โโโ index.js
โโโ server.js
โโโ utils
    โโโ cookie-extractor.js
    โโโ create-token.js
```

---
## ๐ 71์ผ์ฐจ 2.8.ํ. ํ๋ก์ ํธ 6์ผ์ฐจ TL;DR
1. mongoDB connect ์ฃผ์๋ localhost ๋์  MongoDB Compass URI ์ฌ์ฉํ๊ธฐ (mongodb+srv://<account>:<password>@<URI>.mongodb.net/<dbName>)
2. Database Accessํญ์์ ์ ๊ทผ ๊ณ์ ์ ์์ฑํ  ์ ์๋ค.
3. dotenv ํ์ผ์์ key=value์์ value์ ""๋ฅผ ๋ถ์ด์ง ์์๋ ๋๋ค.
4. Promise.all ์ฌ์ฉ์ ์ค๊ฐ์ reject๊ฐ ๋๊ฒ๋๋ฉด ์คํ์ ์ค์งํ๋ค. ๊ทธ๋ฌ๋, Promise.allSettled๋ฅผ ์ฌ์ฉํ๋ฉด ์ค๊ฐ์ reject๊ฐ ๋๋ ๋ฉ์ถ์ง ์๋๋ค. settled๋ fulfilled, rejected ์ํ๋ฅผ ์๋ฏธํจ.
5. GitHub API rest๋ก total commit์ ๊ตฌํ  ๋ get์์ฒญ ๋น per_page๊ฐ 100๊ฐ๊ฐ limit์ด๋ฏ๋ก 100๊ฐ๊ฐ ๋์ ๋๋ `@octokit/plugin-paginate-rest`์ paginateRest๋ฅผ ์ฌ์ฉํ์.
6. ์ธ๋ถ API๋ฅผ ์ฌ์ฉํ๋ ๋ก์ง์ lib/api ํด๋ ์์ ๋ฃ์ด๋์
7. passport.authenticate('jwt', { session: false })์์ next()๊ฐ ๋์ง ์๊ณ  Unautorized๊ฐ ๋์ค๋ฉด jwt์ expiredIn ๊ฐ์ ์ ๋๋ก ์ ์ฉํ๋์ง ์ดํด๋ณด์ (3600 => 1h)
8. `jest` ์คํ ์ `svg` ๊ด๋ จ ์ค๋ฅ๊ฐ ๋๋ค๋ฉด `jest-svg-transformer` ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ฅผ ์ดํด๋ณด์

---
## ๐ 72์ผ์ฐจ 2.9.์. ํ๋ก์ ํธ 7์ผ์ฐจ TL;DR
1. React์์ webpack๊ณผ ํจ๊ป ์ฌ์ฉ์ svg๋ฅผ ์ฌ์ฉํ  ๋ ["@svgr/webpack"]๋ฅผ ์ฌ์ฉํ๋ค๋ฉด file-loader์๋ svg๋ฅผ ์ ๊ฑฐํด์ฃผ์ 
2. webpack alias๋ก jest test๊ฐ ์ ์์ ์ผ๋ก ์๋ํ์ง ์์ผ๋ฉด "@/(.*)": "<rootDir>/src/$1"๋ฅผ ์ถ๊ฐํ์
3. mongoDB์ timestamps๋ฅผ ์นด๋ฉ์ผ์ด์ค๋ก ์์ฑํ๋ฉด ์๋ํ์ง ์๋๋ค.(timeStamps(x)) ์ฃผ์ํ์
4. mongoDB์์ _v(์ด ํค ๊ฐ์๋ ๋ฌธ์์ ๋ด๋ถ ๊ฐ์ ์ด ํฌํจ๋ฉ๋๋ค)๋ฅผ ์์ ๋ ค๋ฉด versionKey: false๋ก ์ค์ ํ์.
6. DB์ accessToken๊ฐ์ ๊ทธ๋๋ก ์ ์ฅํ๊ธฐ๋ณด๋ค๋ ์ํธํ์์ ํน์ yml, aws-secret-manager๋ก ๊ด๋ฆฌํ์
7. API๊ฐ ์ค๋ณต๋๋๋ผ๋ Restํ๊ณ  ๊ทธ ์์ด ์ ๋ค๋ฉด ์ค๋ณต์ผ๋ก ๋ณด์ง ์์๋ ๋๋ค.
8. commit/today์์ ํ๊บผ๋ฒ์ ๋ชจ์ผ์ง ๋ง๊ณ  ๊ณ์ธตํ์ํค์. commit/today/detail, commit/today/repo-name, commit/today/list์ฒ๋ผ
9. issue๋ commit์ผ๋ก ํฌํจ์ํค๋๊ฐ? ๋๋ฉ์ธ๊ฐ์ ํฌํจ๊ด๊ณ๋ฅผ ๋ฐ์ ธ restํ๊ฒ ์์ฑํ์.
10. ํ์ํ ๋ฐ์ดํฐ๋ง ์ถ๋ ค์ db์ ๋ฃ๊ณ  ๊ฐ๊ณตํ์
11. ์ฐ๋ฆฌ ์๋ฒ์์ ์ ์กํ๋ api๊ฐ ์๋๊ณ  ์  3์ api๋ฅผ ์ด์ฉํ๋ค๋ฉด external-api์ ๊ฐ์ ์๋ช์ ์๊ฐํ์
12. service๋ api๋ฅผ ํธ์ถํด์ ๋์จ ๊ฒฐ๊ณผ๋ฅผ ๊ฐ๊ณตํด์ ๋์จ ๊ฒฐ๊ณผ๋ฅผ db์ ์ ์ฅํ๋ ์ฉ๋, contoller๋ client๋ก ๋ด๋ ค์ฃผ๋ ์ฉ๋(ex. res.json)
13. router๊ฐ controller์ ๊ธฐ๋ฅ์ ๊ฐ์ ธ๊ฐ ์๋ ์๋ค.
14. router๋ API path๋ฅผ ๋ง๋ค์ด์ค๋ค.
15. /api์ ์กด์ฌ์ฌ๋ถ๊ฐ restful์ ์ฐจ์ด๋ฅผ ๋ง๋ค๊ธฐ๋ณด๋ค๋ ๋ณดํต์ ์ฐ๋ฆฌ ์๋น์ค์ api๋ฅผ ํธ์ถํ  ๋ ์ฌ์ฉํ๋ค.

---
## ๐ 73์ผ์ฐจ 2.10.๋ชฉ. ํ๋ก์ ํธ 8์ผ์ฐจ TL;DR
1. populate๋ mongoDB์์ _id๋ฅผ ํตํด ๋ค๋ฅธ ์ปฌ๋ ์์ ์๋ ๋ฐ์ดํฐ๋ฅผ ์ฐธ์กฐํ  ์ ์๋ค.
2. new User({}).save()์ User.create({})๋ ๋์ผํ๋ค.
3. findById(id)๋ findOne({_id: id})์ ๊ฐ๋ค.
4. query ์์ฒญ์ ์ค์ด๊ธฐ ์ํด find() -> ์์  -> save()๋ณด๋ค where()๋ฅผ ํ์ฉํ์.
5. upsert(): ์กด์ฌํ์ง ์๋ ๋ฌธ์์ ๊ฒฝ์ฐ ์๋ก ์์ฑํ์ฌ ์ ์ฅํ๋ค.
6. mongoDB์์ dataBase๋ ์ฌ๋ฌ collection์ ๋ด๋ ํ๋์ ์ ์ฅ์, collection: ์ฌ๋ฌ๊ฐ์ document๋ฅผ ๋ด๋ ๊ณต๊ฐ, document: ์ฌ๋ฌ๊ฐ์ key-value๋ก ์ด๋ฃจ์ด์ง ํ๋์ ํ์ด์ง, key-value: ์ด๋ฆ - ๊ฐ

---
## ๐ 74์ผ์ฐจ 2.11.๊ธ. ํ๋ก์ ํธ 9์ผ์ฐจ TL;DR
1. ํจ์ ํ๋ผ๋ฏธํฐ๋ก ์๋ก์ด ๊ฐ์ฒด key๋ฅผ ์ค์ ํ  ๋๋ ๋ค์๊ณผ ๊ฐ์ด ์์ฑํ์.

```javascript
const FindByKey = (key) => {
  const config = {};
  config[key] = value;
}
```

2. webpack์์ favicon ๊ด๋ จ ์ค์ ์ `HtmlWebpackPlugin`์ option์ผ๋ก ์ค์ ํ  ์ ์์ง๋ง manifest๋ฅผ ๊ณ ๋ คํ๋ค๋ฉด `FaviconsWebpackPlugin`์ผ๋ก ์ค์ ํด์ฃผ์.
3. GitLab์๋ Default branch๋ฅผ ์ค์ ํ์ฌ MR์์ฒญ์ ๋ณด๋ผ ๋ target์ค์ ์ ํ์ง ์์ผ๋ฉด default branch๋ก ๊ฒฝ๋ก๋ฅผ ์ค์ ํ  ์ ์๋ค.
4. GitLab์๋ Protected branches ์ค์ ์ด์์ด ํจ๋ถ๋ก ํด๋น branch์ ๋ฐ๋ก commitํ์ง ๋ชปํ๊ฒ ์ค์ ํ  ์๋ ์๋ค.(force๋ ์ฌ์ฉ๋ถ๊ฐ, MR๋ก๋ง merge ๊ฐ๋ฅ)
5. eslint ์ค์ ์ `eslint-plugin-prettier` ํจํค์ง์ `eslint-config-prettier` ํจํค์ง๊ฐ ์ ์์ ์ผ๋ก ์ค์น๋์๋์ง ํ์ธํ์.
6. eslint ์ค์ ์ `test` ํ์ผ์ `eslint-plugin-jest` ํจํค์ง๋ก ๋ฌธ๋ฒ ๊ฒ์ฌํ์.
7. DB์ ์ ์ฅํ๋ timestamp๋ฅผ KST๋ก ๋ง์ถ์ง๋ง๊ณ  UTC๋ก ํต์ผํ์. ๋์ค์ ๋ง์ด๊ทธ๋ ์ด์ ํน์ ์๋น์ค ๋ณต์ ์ ๋ถ ํ์ํ ํ์๋ฅผ ๋ฐฉ์งํ๋ค.
8. GitHub API์์ ์๋ต์๊ฐ์ ๊ณ ๋ คํด์ ์๋ต์๊ฐ์ ์ด๊ณผํ๋ฉด DB์ ์๋ ๊ฐ์ ๋ด๋ ค์ฃผ๊ธฐ
9. ๋งค ์์ฒญ๋ง๋ค API๋ฅผ ์ฃผ์ง๋ง๊ณ  ์ผ์ ์๊ฐ ์ด๋ด ๋์ผํ ์์ฒญ์ด์ค๋ฉด DB์ ์๋ ๊ฐ์ ๋ด๋ ค์ฃผ์ด ๋ถ ํ์ํ API ์์ฒญ์ ๋ง๋๋ค.
10. ๊ฐ๊ด์ ์ธ ๊ธฐ์ค์ด ์๋๋ผ ์ฃผ๊ด์ ์ธ ๊ธฐ์ค์ ์ํํด๋ณด๊ณ  ์ถ๋ค๋ฉด ํ๋ฒ ์๋ํด๋ณด๊ณ  ์ฅ๋จ์ ์ ๋น๊ตํด์ ๋๋ง์ ๊ธฐ์ค์ ์ธ์๋์.
11. ํ์ฌ ํ์ ์ํฉ์ ๊ณ ๋ คํด์ ๋ธ๋์น ์ ๋ต์ ์ด๋ป๊ฒ ๊ตฌ์ฑํ ์ง ์๊ฐํด๋ณด์ 
12. ์ปค๋ฐ ๋จ์๋ ํ์๋ค๋ผ๋ฆฌ ๊ณ ๋ คํด์ ์ ์ฉํ์.
13. GitHub API GET ์์ฒญ์ time์ UTC๋ก ๋ณ๊ฒฝํด์ ์์ฒญํ๋์ง๋ doc๋ฅผ ์ฐธ๊ณ ํ์
14. GitHub API์์๋ timestamps ๊ธฐ๋ฅ์ ์์ฒญํ  ๋๋ง ์ฌ์ฉํ  ์ ์๊ณ , ๊ฐ์ ๋๋ ค๋ฐ๋ ์์ฒญ์์๋ ์ฌ์ฉํ  ์ ์๋ค. (Note that these rules apply only to data passed to the API, not to data returned by the API. As mentioned in "Schema," timestamps returned by the API are in UTC time, ISO 8601 format.) <a href='https://docs.github.com/en/enterprise-server@3.0/rest/overview/resources-in-the-rest-api'>GitHub DOC</a>
15. mongoDB์์ UTC๋ฅผ KST๋ก ๋ณ๊ฒฝํ๋ ๋ฐฉ๋ฒ
16. UTC์์ KST๋ก ๋ฐ๊ฟ ๋ Date.prototype.toLocaleTimeString()๋ฅผ ์ฌ์ฉํ๋ฉด ๊ฐํธํ๊ฒ ๋ฐ๊ฟ ์ ์๋ค.
17. JS ๊ธฐ๋ณธ Date๋ UTC๋ก ๋ณํ๋๊ธฐ ๋๋ฌธ์ UTC๋ก ์์ฒญ์ ๋ฐ๋ GitHub API๋ ์ถ๊ฐ์ ์ผ๋ก ์๊ฐ์ ๋ณํํด์ค ํ์๊ฐ ์๋ค.

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
## ๐ 75์ผ์ฐจ 2.12.ํ . ํ๋ก์ ํธ 10์ผ์ฐจ TL;DR
1. MR์ confilct๊ฐ ๋๋ค๋ฉด ์๋ก์ด branch๋ฅผ ํ๋ ํ์ ๋ด๊ฐ ์ฌ๋ฆฌ๋ ค๋ branch๋ฅผ git pull origin <๋ด ๋ธ๋์น>ํ๊ณ  ๋ค์ MR์์ฒญํ์.
2. MR์ ํ์ฅ๋ง ๋ณด๋๊ฒ์ด ์๋๋ผ ํด๋น ํ์๋ค๊ณผ ๊ฐ์ด ๋ณด๋ฉด์ ๊ฐ์ ํ๊ณ  ์ถ์์ , ๋๋์ ๋ฑ์ ๊ฐ๋จํ๊ฒ ์ฝ๋ฉํธ๋ก ๋จ๊ฒจ์ฃผ๊ณ  mergeํ๋ ๋ฐฉ๋ฒ๋ ์๋ค.
3. postman์์ POST์์ฒญ์ ๋ณด๋ผ ๋ cookie๋ฅผ ์ฌ์ฉํ๋ค๋ฉด cookie ํญ์ ๊ฐ์ ์ถ๊ฐํ์. ์ด๋ ๋๋ฉ์ธ์ host๋ค์๋ง ์์ฑํด๋ ๋๋ค.
4. ์บ๋ฆฐ๋ํ์์ data์์ ๊ฐ๊ฐ ์ผ์๋ฅผ ๋ํ๋ ๋ก์ง

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
๐๐ฝ [ [ 0, 0, 2, 10 ], [ 4, 14, 2, 8 ] ]
```

5. ํ์ฌ ๋ฌ์ ๊ธฐ์ค์ผ๋ก ๋ฉฐ์น ๊น์ง ์๋์ง ๋ฆฌํดํ๋ ํจ์์์ฑ(์ค๋ํฌํจ)

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
๐๐ฝ [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0 ]
```
---
## ๐ 2.14.์. TL;DR
1. Suspense๋ ์์ ์ปดํฌ๋ํธ์ ๋น๋๊ธฐ ์์์ด ์ฒ๋ฆฌ๋๊ธฐ ์ ์ fallback props๊ฐ ๋ ๋๋ง ๋๋ค. ์ฆ, ๋น๋๊ธฐ ์์์ด ๋๋  ๋๊น์ง loading ์ปดํฌ๋ํธ๋ฅผ ๋ณด์ฌ์ฃผ๋ ์ฝ๋๋ฅผ ๋ฃ์ ์ ์๋ค.
2. bcrypt์์ sync๋ณด๋ค async๋ฅผ ๊ถ์ฅํ๋ ์ด์ : ๊ฐ๋จํ script์์๋ sync๋ชจ๋๋ฅผ ์ฌ์ฉํ๋๊ฒ์ด ์ข์ผ๋, ์๋ฒ์์ bcrypt๋ฅผ ์ฌ์ฉํ๋ ๊ฒฝ์ฐ ๋น๋๊ธฐ๋ชจ๋๋ฅผ ์ฌ์ฉํ๋๊ฒ์ด ์ข๋ค. bcrypt์ ์ํด ์ํ๋ ํด์ฑ์ CPU๋ฅผ ๋ง์ด ์ฌ์ฉํ๋ฏ๋ก ๋๊ธฐํ๋ ์ด๋ฒคํธ ๋ฃจํ๋ฅผ ์ฐจ๋จํ๊ธฐ๋๋ฌธ์ ๋ค๋ฅธ ์ด๋ฒคํธ๋ฅผ ์ฒ๋ฆฌํ์ง ๋ชปํ๋ค. ๋น๋๊ธฐ๋ ๋ฉ์ธ ์ด๋ฒคํธ ๋ฃจํ๋ฅผ ์ฐจ๋จํ์ง ์๋ ์ค๋ ๋ ํ์ ์ฌ์ฉํ๋ค.
3. GitHub๋ก ๋ก๊ทธ์ธํ๋ฉด Backend์์ cookie์ ๋ด์์ Frontend๋ก ๋ณด๋ธ๋ค.
4. Frontend์์ JWTํ ํฐ์ Header์ ๋ฃ์ด์ req์์ฒญ์ ๋ณด๋ด๋ฉด Backend์์ ํด๋น jwt๋ฅผ ํด์ํ๋ค. ํน์ cookie์ ๋ด์์ ๋ณด๋ธ๋ค.
5. jest test์ `expect(...).toBeA is not a function` ์ค๋ฅ๊ฐ ๋๋ค๋ฉด expect์ ๊ดํธ๊ฐ ์ ๋๋ก ์์ฑ๋์ด์๋์ง ์ดํด๋ณด์.
// correct expect(getApi()).toBe(answer);
// Incorrect expect(getApi().toBe(answer));
6. jest test์ `regeneratorRuntime is not defined`๊ฐ ๋ฌ๋ค๋ฉด `npm i -D regenerator-runtime`๋ฅผ ์ค์นํ๊ณ  `import 'regenerator-runtime'`๋ก ๋ถ๋ฌ์ค์.

---
## ๐ 76์ผ์ฐจ 2.15.ํ. ํ๋ก์ ํธ 11์ผ์ฐจ TL;DR
1. branch ์ ๋ต

```javascript
  - Git-Flow: ๋จ์ํ๋ค, CI/CD๊ฐ ์์ฐ์ค๋ฝ๋ค, master(์ต์ข), ์ฒด๊ณ์ ์ธ ๋ถ๋ฅ ์์ด master์ ์์กดํ๋ค.
  - GitHub-flow: ์์ธํ ๋ฆฌ๋ทฐ์ ํ ์, master(์ต์ข), develop(๊ฐ๋ฐ), release(QA ๋ฐ ๋ฒ ํ ํ์คํธ), hotfix(master์์ ๋ฒ๊ทธ์์ )
```

2. ์ฐ๋ฆฌํ์ GitHubFlow๋ฅผ ๊ธฐ๋ฐ์ผ๋ก ํ๋ GitFlow์ ๋ฐฉ๋ฒ์ ์กฐ๊ธ ์์๋ค. commit convention์ ์ ํ๊ณ , MR์ฌ๋ฆฌ๋ฉด ํด๋น ๋ถ์ผ ํ์๋ค์ด ์ฝ๋๋ฆฌ๋ทฐ ํ ์๊ฒฌ์ ๋จ๊ธด๋ค. emoji๋ฅผ ๋ชจ๋ ๋จ๊ฒผ์ผ๋ฉด ํ์ฅ์ด ์ต์ข์ ์ผ๋ก mergeํ๋ค. merge๊ฐ ์๋ฃ๋ branch๋ ์ญ์ ํ๋ค. commit์ ๊ฐ์๋ฅผ ๋ชจ๋ ๋จ๊ธฐ๋๊ฒ๋ณด๋ค squash ์ ๋ต์ผ๋ก ์ฌ๋ฌ๊ฐ์ ์ปค๋ฐ์ ํ๋๋ก ๋ญ์น๋ค. (์ด์ ๋น์ทํ rebase ์ ๋ต์ ์ ์ผ ๋ง์ง๋ง commit๋ง ์ฌ์ฉํ๋ค. log๊ฐ ๊น๋ํด์ง๋ ์ฅ์ ์ด ์์ง๋ง ๋ฐ๋ฉด์ ๊ธฐ๋ก์ด ๋จ์ง ์์ผ๋ฏ๋ก git ์๋ จ๋๊ฐ ๋ฎ์ผ๋ฉด ์ถ์ฒํ์ง ์๋๋ค.) ๊ธํ๊ฒ ์์ ํ๋ ์ฌํญ์ hotfix ๋ธ๋์น๋ฅผ ์ฌ์ฉํ๊ณ , Back๊ณผ Front ์ฐ๊ฒฐ์ release 0.0.x ๋ฒ์ ์ ๋ธ๋์น๋ฅผ ๋ง๋ค์ด์ QAํ์คํธ๋ฅผ ์งํํ๋ค. 
3. react์์ proxy๋ฅผ ์ฌ์ฉํ  ๋ CRA ๋์  webpack์ ์ฌ์ฉํ๋ค๋ฉด webpack.config.js์์ devServer์์ ๋ค์๊ณผ ๊ฐ์ ์ฝ๋๋ฅผ ์ถ๊ฐํ๋ค. ์ด๋ ๊ฒ ์์ฑํ๋ฉด ํ๋ก ํธ์์ ๋ฐฑ์ผ๋ก API์์ฒญ์ ํ  ๋ host + port๋ฅผ ์๋ตํด๋ target์ผ๋ก ์์ฒญ์ด ๋์ด๊ฐ๋ค.

```javascript
proxy: {
      "/api": {
        target: "http://localhost:8888",
	},
}
```

4. ์ด์ ์๋ฒ ๋ฐฐํฌํด๋ณด๋ ๊น์ `Azure`, `Nginx`, `CI/CD` ๋ ๊ณต๋ถํด๋ณด์.
5. ์๋ฒ์์ `GET,`, `POST` ์ ๊ฐ์ ์์ฒญ์ ํ์คํธํ๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ `supertest`๋ฅผ ์ด์ฉํ๋ค. ์ ๋ ํ์คํธ๋ `jest`
6. `jest coverage` ๋ ํ์คํธ ํํฉ์ ํ๋ก ํ ๋์ ๋ณผ ์ ์๋ค.

---
## ๐ 77์ผ์ฐจ 2.16.์. ํ๋ก์ ํธ 12์ผ์ฐจ TL;DR
์ค๋์ ๋ด ์์ผ์ด๋ค. ์ด๋ฆด๋์ ์์ผ์ ํน๋ณํ ๋ ๋ก ์๊ฐํ์ง๋ง ์์ฆ์ ํน๋ณํ ๋ ์ด ์๋๋ผ๋ ์๊ฐ์ด ๋ ๋ค. ํ๋ก์ ํธ ๋ง๊ฐ์ด 4์ผ์ด ์ฑ ๋จ์ง ์์๊ธฐ ๋๋ฌธ์ ์ ๊ฒฝ์ฐ์ง์๊ณ  ์์์ค์ด๋ค.

1. ๋์ ์๋ฅผ ๊ณ ๋ คํ ์์ ๋งค๊ธฐ๊ธฐ

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

2. develop์ ์ต์  ์ฝ๋๋ฅผ ๋ค๋ฅธ ๋ธ๋์น๋ก ๋ด๋ ค๋ฐ์ ๋๋ git checkout develop ํ git merge <target-branch>๋ฅผ ํด์ฃผ๋ฉด ๋๋ค.
3. routes์์ ๋์ผํ URI๋ก GET, POST์์ฒญ์ ๋ณด๋ด๋ ์ฝ๋๋ ๋ค์์ฒ๋ผ ํ ์ค๋ก ์ค์ผ ์ ์๋ค.

```javascript
// before
router.get("/today/goal", getGoalController);
rotuer.post("/today/goal", postGoalController);

// after
router.route("/today/goal").get(getGoalController).post(postGoalController);
```

4. `nvm(node version manager)`: curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.36.0/install.sh | bash
5. `source ~/.bashrc` ํ์ผ๋ก ์ด๋ 
6. `nvm install 14.18.1`: ์ํ๋ ๋ธ๋ ๋ฒ์  ์ค์น 
7. `nvm ls`: ์ค์นํ ๋ธ๋ ๋ชฉ๋ก ๋ณด๊ธฐ
8. `node -v` : ํ์ฌ ๋ธ๋๋ฒ์  ๋ณด๊ธฐ
9. ํฐ๋ฏธ๋ ์ฌ๋ถํ ํ์๋ ๋ธ๋ ๋ฒ์ ์ด ์ ๋๋ก ์ ์ฉ๋์ด์๋์ง ์ดํด๋ณด๊ธฐ
10. ๋ฐฑ์๋ ๊ฐ์ ํ  ์ : ์จ๋ํํฐ API๋ฅผ ์ด์ฉํ๋ ๋ก์ง์ ์ฒ์์ ๋ชจ๋ ๊ธ์ด์จ๋ค์ DB์ ์ ์ฅํ๊ณ , ์ผ์  ์๊ฐ๋ง๋ค ๊ฐฑ์ ํ์ผ๋ฉด ๋ ์ข์ ๊ฒ ๊ฐ๋ค.
11. `Nginx` ์ด์ฉ์ `proxy_pass` ๊ฐ ์ค์ ํ๊ธฐ `๋๋ฉ์ธ` -> `nginx` -> `server.js`
12. `release` ๋ธ๋์น๋ ์์ ํ์ง ์๊ณ  `develop` ๋ธ๋์น์ ์์ ์ฌํญ์ ๊ฐ์ ธ์ค๊ธฐ๋ง ํ๋ค. ๋ง์ฝ, `release` ๋ธ๋์น์ `history`๋ฅผ ๊ด๋ฆฌํ๊ณ  ์ถ๋ค๋ฉด `tag`๋ฅผ ๋จ๊ธฐ๊ฑฐ๋ ์ญ์ ํ์ง ์๊ฑฐ๋..
13. ๋ฌด๊ฒ์ง ์์ ๋ก์ง์ ํ์คํธ์ฝ๋๋ก ๋จ๊ฒจ๋๊ธฐ

---
## ๐ 78์ผ์ฐจ 2.17.๋ชฉ. ํ๋ก์ ํธ 13์ผ์ฐจ TL;DR
1. cors credentials: HTTP Cookie์ HTTP Authentication ์ ๋ณด๋ฅผ ์ธ์ํ  ์ ์๊ฒ ํด์ฃผ๋ ์์ฒญ์ด๋ค. ํด๋ผ์ด์ธํธ์์ ์๋ฒ๋ก ์์ฒญ์ ๋ณด๋ธ๋ค๋ฉด `axios.defaults.withCredentials = true;`๋ฅผ ๊ผญ!!!@#!@#!@#!@ ์ค์ ํด์ฃผ์.

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

2. /bin/www ํ์ผ์ ์ต์คํ๋ ์ค์ ์ค์  ํ์ผ์ ๊ฐ์ ธ์ http์ ์ฐ๊ฒฐํ๋ ์์ (nginx๋ฅผ ๋ถ์ธ๋ค๋ฉด ์ด ํ์ผ๊ณผ ์ฐ๊ฒฐํ๋ฉด ๋๋ค.)

---
## ๐ 79์ผ์ฐจ 2.18.๊ธ. ํ๋ก์ ํธ 14์ผ์ฐจ TL;DR
1. webpack ์ฌ์ฉ์ public์ ์ ๊ทผํ๋ ค๋ฉด devServer.static์๋ ๋ค์๊ณผ ๊ฐ์ด ์์ฑํ๋ฉด `localhost:port/assets/public`๋ก ์ ์์ด ๊ฐ๋ฅํ๋ค.

```javascript
static: {
      directory: path.resolve(__dirname, "public"),
      publicPath: "/assets", /
}
```

2. public์์ manifest.json์ ๊ฒฝ๋ก๋ ๋ค์๊ณผ ๊ฐ์ด ์์ฑํ๋ค. `<link rel="manifest" crossorigin="use-credentials" href="/assets/manifest.json">`
3. GitLab์์ tag๋ ๋ธ๋์น๊ฐ ์๋๋ผ commit์ ๊ด๋ฆฌํ๋ค.
4. ์๋ต์ JSON Parse๋ฅผ ์ฌ์ฉํ  ๋๋ ์์ฒญ๋ String์ผ๋ก ๋ณํํ๊ณ  ๋ณด๋ด์ผ ํ๋ค.(๋ฐ์ดํฐ ํ์์ด ๋ฐฐ์ด์ด๋ฉด `[${badges}]` ์ฒ๋ผ ๋ณด๋ด๊ธฐ)
5. nginx๋ฅผ ์ฌ์ฉํ๋ฉด ํด๋ผ์ด์ธํธ์์ ์๋ฒ URI์ ์์์ ๋ณผ ์ ์๋ค.(์ ํด์งAPI๋ก ์์ฒญํ๋ฉด ๋ฆฌ๋ฒ์ค ํ๋ก์ฑ์ ํตํด ์๋ฒ๊ฐ ์๋ตํ๋ ์ฃผ์๋ก ๋ฐ๊ฟ์ฃผ๊ธฐ ๋๋ฌธ)

---
## ๐ 80์ผ์ฐจ 2.20.ํ . ํ๋ก์ ํธ 15์ผ์ฐจ TL;DR
1. ํด๋ผ์ด์ธํธ์์ ์์ฒญํ ๋๋ ๊ฐ๋์๋ฒ(localhost)๋ก ์์ฒญํ๋๊ฒ์ด ์๋๋ผ ๋ฐฐํฌํ๋ ๋๋ฉ์ธ์ผ๋ก ์์ฒญํด์ผํ๋ค.(์ดํ์ nginx์์ reverse proxy ์ฒ๋ฆฌํจ)
2. env์ callback URI๋ ๋๋ฉ์ธ๊น์ง ํฌํจํด์ ์์ฑํ์.
3. Git clone ๋ฒํผ์ผ๋ก ๋๋ฌ์ ๋ฐ๋๊ฒ์ ์ต์ ์ ๋ธ๋์น๋ฅผ ๋ฐ๋๊ฒ์ด๋ค. ํน์  ๋ธ๋์น๋ฅผ ๋ฐ๊ณ  ์ถ์ผ๋ฉด ๋ค์ ์ฃผ์๋ฅผ ์๋ ฅํ์ `git clone -b <branchName> --single-branch <git clone URL>`