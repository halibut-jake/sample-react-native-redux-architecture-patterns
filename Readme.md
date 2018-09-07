# React Native Redux Sample Project

## 소개
`React Native`로 간단한 덧셈이 되는 `Redux` 아키텍쳐 패턴을 적용한 셈플입니다.<br />

## 결과 이미지 (GIF)

<img width="268" height="480" src="/Image/result_image00.gif"></img>

## 주요 구조

```
- ios
- android
- scr
	- actions
		- index.js
		- calculatorAction.js
		- types.js
	- components
		- Calculator.js
	- containers
		- Main
		- Root
	- store
		- index.js
- App.js

```



## 설명
### Redux란?
시작이 되는 근원은 리엑티브 라고 할 수 있습니다.
리엑티브는 같은 말로 알엑스(Rx) 라고 부릅니다.
리엑티브 페러다임은 마이크로소프트가 창안한 개념으로 데이터의 흐름에 따른 변화를 만드는 비동기적인 프로그래밍 패러다임입니다
기본 실행 모델이 데이터의 흐름을 통해 자동으로 전파하는 것입니다.

RX 패러다임은 다양한 개발언어로 확장 되었는 데, 
페이스북에서 만든 Flux 패턴의 구현체 중 하나입니다.

- [Redux 설명 링크](https://medium.com/@jang.wangsu/rn-react-native-redux-%EB%9E%80-reactive-%EB%B6%80%ED%84%B0-c089d4549edb)

### Redux 간략 설명

Redux는 앱의 상태 모두를 하나의 store안에 트리 구조로 저장합니다. 
그 스토어를 변경시키는 것은 action (들) 뿐입니다.
action이 어떻게 (How) 변경시켜야 하는 지는 reducer(들)가 정의합니다.
화면(View)들은 중요하진 않겠지만 component들을 담는 것을 Container(들) 이라 지칭하겠습니다.
Container(들)은 Store의 상태값이 변화되는 지 구독하고(subscribe, subscript) 있는 데, redux에서는 props에 담아 넘겨줍니다. Props에 selector(들) 하고 있습니다.
Container 의 화면에서는 사용하기 위해 props를 state에 map 하는 과정이 진행됩니다.
그리고 화면의 메인스레드 런루프에서 클릭등 이벤트가 발생해서 변경요청을 하면, 
 
Container에서 action을 보내는 데, 그것을 dispatch action이라 합니다.
action을 dispatch하는 거죠....
추가적으로 state를 변경하기 위해 비동기 처리를 하는 경우가 있는 데 보통 대표적인 것이 네트워크 처리 이죠? 물론 그게 아니더라도 보통 비동기 처리를 하는 것이 대부분 일 것 같기도 합니다. 
이렇게 비동기 처리를 위해 action과 reducer 사이에 middleware를 둡니다.
그 때 미들웨어에 thunk(들)과 saga (들).. 등 이(가) 있습니다.



### 진행 사항 간 특징
- 쉘 명령어 react-native로 구현하였습니다.
	- [react-native 를 이해하기 위한 링크](https://medium.com/@jang.wangsu/rn-react-native-%EC%8B%9C%EC%9E%91-3aab881f574f) : 여기를 참고해서 기본 환경 설정을 해주세요. 
- middleware는 적용하지 않았습니다.
- 동작 시키기 위한 React Native 외의 라이브러리는 없습니다.
- 동작의 흐름을 보기위한 간단한 덧셈이 되는 셈플입니다.

### 상세 설명

#### Store
작성중

#### Action(s)
작성중

#### Reducer(s)
작성중

#### View (components, containers)
작성중
