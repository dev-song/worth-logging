# Snowpack: a newly adopted front-end build tool for a new project, Aicel Market Intelligence

### Intro

에이셀테크놀로지스의 새로운 프로젝트인 Aicel Market Intelligence에서는 Snowpack을 프론트엔드 빌드 도구로 채택하였습니다.

이 글에서는 Snowpack이 프론트엔드 빌드 도구로 채택되었다는 것이 어떤 의미인지, 기존의 빌드 도구를 대체한 이유는 무엇이며, Snowpack의 특징은 어떤 것이 있는지 간략하게 알아보려고 합니다.

### Snowpack?

웹 프론트엔드 기술에 대해 접해보신 분이라면, 트랜스파일, 모듈 번들링, 빌드, Babel, Webpack 등의 이름을 들어보신 적이 있으시라 생각합니다.

[Snowpack 페이지](https://www.snowpack.dev/)에선 스스로를 **webpack이나 Parcel 같은 무겁고 복잡한 번들러를 대체할 수 있는 `번개처럼 빠른` 빌드 도구**라고 소개하고 있습니다.

※ 트랜스파일링 `Transpiling` : 한 언어로 작성된 소스코드를 **비슷한 추상화 수준을 가진 다른 언어**로 변환하는 것 (JS ES6 -> JS ES5 등)

※ 모듈 번들링 `Bundling` : 소스 코드에 포함된 복잡한 모듈 의존 관계를 정리하여 배포할 수 있는 파일로 합치는 것

※ 빌드 `Build` : 소프트웨어의 소스 코드를 실행 가능한 형태로 변환하는 것 - 트랜스파일, 모듈 번들링 등을 모두 포함하는 개념

### 기존 빌드 도구과의 비교

에이셀테크놀로지스의 기존 프로젝트들은 [create react app](https://github.com/facebook/create-react-app)을 베이스로 제작되었고, 자연히 create react app에 포함된 webpack을 빌드 도구로 사용했습니다.

- webpack과의 차이점

### Snowpack의 특징

- webpack과의 차이점 외 실행 방법에서의 주의점, 사용상의 특별한 편의성 등
