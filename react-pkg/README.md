## React Package

1. react.development.js
2. react.production.min.js
3. react-dom.development.js
4. react-dom.production.min.js

|번호|설명|
|-|-
|1,3| React 개발(development) 환경에서 사용되는 파일
|2,4| 배포(production)환경에서 사용되는 파일
|1,2| 리액트의 핵심 기능이 담긴 파일. react-native 에서도 사용된다.
|3,4| 가상돔 자료구조 정보가 담긴 파일. 웹에서만 사용된다.

### 가상돔이란?
> React에서 이전 UI 상태를 메모리에 유지하고 데이터가 변경됐을 떄 UI 변경사항을 빨리 찾기 위한 자료구조이다.

### 리액트 네이티브?
> 리액트 네이티브는 리액트로 작성된 소스코드로 안드로이드와 iOS의 네이티브 앱을 만들기 위한 라이브러리이다.
> 상단에 서술된 react 패키지가 react-native에서도 사용되며 react-dom의 경우 react-native를 위한 코드가 별도로 존재한다.

### 리액트 네이티브는 어떻게 모바일 환경에서 자바스크립트를 실행하는가?
> react-native는 JavascriptCore(웹킷에 내장된 자바스크립트 엔진)을 이용해 모바일에서 자바스크립트를 실행한다. 
> 이때 JavascriptCore는 C++로 작성되어 있는데 모바일 운영체제는 대부분 C++ 코드를 실행할 수단을 제공한다.
> 그러므로 앱 빌드 시 JavascriptCore를 포함 시키는 것으로 자바스크립트 실행환경을 갖출 수 있다.

### min이 붙은 파일과 아닌 파일의 차이
> min은 minify의 약자로 min이 붙은 파일은 minify가 적용된 파일이라는 뜻이다.
> minify는 코드를 경량화 하기위한 방법 중 하나이다.