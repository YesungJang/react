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

## 1.7 JSX part 2

function 으로 표현 가능
대문자여야만한다
소문자면 html태그라고 인식
arrow function도 사용 가능
<strong>독자적으로 만든 components는 반드지 대문자로 시작해야 한다!!</strong>

# 2. State

## 2.1 Understanding State

state : 데이터의 저장장소
-> 카운터를 state로 할 수 있다
렌더링과 ui업데이트는 다르다
return같은 개념 함수는 계산을 완료했는데 데이터를 표시갱신이 안되어있음
-> rerendering이 필요
리액트의 좋은 점 : 이전에 렌더링된 컴포넌트는 어떤거였는지 확인 후 렌더링될 컴포넌트를 확인 후 다른 부분만 파악

## 2.2 setState part one

리렌더링을 까먹지 않기 위해선?->reactjs에서 데이터를 보관하고 리렌더링하는 방법을 사용(함수를 불러 줄 필요 없음)
어디에 데이터를 담으면 되는 것인가? -> useState
2개의 array를 담음
first element : 시작
second element : function

어떻게 하면 array에서 꺼내서 배열할 수 있을까? ->

## 2.3 setState part two

useState를 쓰면 array를 주는데
첫번째 요소는 시작값
두번째 요소는 값을 바꿀 때 사용할 modifier 수정자
리렌더링을 하기 위해 한번 더 호출 -> react에선set을 붙이면 업데이트 후 리렌더링된다!!java같음
