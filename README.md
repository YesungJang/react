# Why React?

- 44% usage top 10k company
- React JS came Facebook
- Huge Community

# 1. The basics of React

## 1.1 Introduction

interactive 한 사이트를 만드는 것을 위한 도구
js로만 할 때에 필요한 것들을 쉽게 준비되어 있다

## 1.2 Before React

number count

- install React
  두개의 js를 import해야 함 react, react-dom

```
https://unpkg.com/react@17.0.2/umd/react.production.min.js
https://unpkg.com/react-dom@17.0.2/umd/react-dom.production.min.js
```

## 1.3 First React Element

오직 script만 써서 body를 생성
생성은 react-dom이 생성해줌
인터렉티브한 UI를 생성해줌
render -> 사용자한테 보여준다

바닐라에서는 html를 쓰고 js를 썼지만
리액트에서는 모든 것을 js로 시작하고 html
-> 리액트는 html를 제어할 수 있다 -> 원하는 것을 보여줄 수 있다

## 1.4 Event in React

버튼(property)에 eventlistener를 넣는게 가능
리액트는 인터렉티브를 위해 만들어 졌다

## 1.5 Recap 복습

react component에 3가지 argument

1. element
2. property
3. content

property에 eventlistener를 넣을 수 있다

## 1.6 JSX

Javascript를 확장한 문법
브라우저가 jsx를 이해할 수 있도록 설치가 필요-> 바벨이 필요
바벨 : 코드의 변환
jsx로 적은 코드를 브라우저가 이해할 수 있도록 변환

```
https://babeljs.io/repl
```

바벨 트란스폼 스크립트를 import

```
https://unpkg.com/@babel/standalone/babel.min.js
```

사용하는 script에 `type="text/babel"`을 추가
