# Redux

`강의 소스` : https://opentutorials.org/module/4078

- 예측 가능한 애플리케이션의 상태 저장소

앱을 개발하는데 어렵게 만드는 복잡성을 낮춰줄 수 있다. 복잡성을 낮춰주는 방법은 앱에서 사용하는 모든 state를 하나의 상태(객체)로 관리하는 것이다. redux에 상태를 바꾸려고 할 때 특정 함수를 이용하게 하고 상태가 변경되면 컴포넌트에 잘 알려준다. `undo`와 `redo`를 매우 쉽게 할 수 있다.

## 리덕스 여행지도

- store

  은행. 정보가 저장되는 곳

- state

  실제 데이터가 저장되는 장소

- reducer

  함수.

- dispatch, getState, subscribe

  행원 역할을 하는 함수들

  - subscribe

    state가 바뀔때마다 렌더링을 다시 해달라고 요청할 수 있게 해줌

- render

  개발자가 직접 짤 코드, ui를 만드는 코드

- action과 dispatch

  1. reducer를 호출해서 state를 바꿈
  2. subscribe를 호출해서 render를 다시 함



## Redux가 좋은 가장 중요한 이유

1. 컴포넌트에서 다른 컴포넌트의 상태값을 바꾸어 줄 때 중앙집중적인 방식으로 구현하면 복잡성을 줄여줄 수 있다.

2. 버전관리가 가능