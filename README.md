# React JS란?!

## 바닐라 JS와 리액트 JS의 차이점을 알고 어떤 장단점이 있는지 확인해 본다. /n Convert 게시물의 파일은 React 17버전을 기준으로 작성되었음. 현재 React 18버전과 차이가 있으니 유의하기.

# Vanilla JS의 경우 `HTML → JS 순서`

📍 Html 작성
📍 html 요소를 JS로 가져온다.
📍 event를 감지하고 데이터를 업데이트 한다.
📍 Html에도 데이터 업데이트를 반영한다.

# React JS는 이와 반대로 `JS에서 HTML 요소`를 컨트롤 한다

📍 JS 작성 | React 환경 설정
📍 React를 이용, HTML요소 생성 및 삽입
📍 event를 감지하고 데이터를 업데이트 한다.
📍 Html에도 데이터 업데이트를 반영한다.

# React를 단순하게 사용하자! JSX(실용)

- This funny syntax is neither a string nor HTML.
  It is called JSX, and it is a syntax ectension to JavaScript. (JSX = JS를 확장한 문법!)
- But, JSX는 브라우저가 인식하지 못하므로 ‘Babel’을 설치하여 읽을 수 있는 문법으로 변환 시켜줘야함!
- `id=”root”`로 모든 JSX컴포넌트들을 품는 최상위 컴포넌트가 필요.
  1. JSX 요소들을 함수화 한다. ⇒ **컴포넌트 ,** 이때 함수명은 대문자로 시작!!! `const Title=… // const Btn=… // const Container=…`
  2. 함수를 root 태그 안에 넣는다. ⇒ 이때 (함수형)컴포넌트는 `Btn()`이 아닌 `<Btn />` 으로 작성해야한다!
     React JSX 방식

```jsx
const element = <h1 class="greeting">Hello, world</h1>;
```

React JSX with Babel 방식

```jsx
const element = React.createElement(
  "h1",
  { className: "greeting" },
  "Hello, world"
);
```
