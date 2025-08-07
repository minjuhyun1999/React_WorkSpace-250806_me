# 프로젝트 개발 가이드

이 문서는 `React_WorkSpace-250806` 프로젝트의 विभिन्न सब-प्रोजेक्ट्स को चलाने और प्रबंधित करने के लिए आवश्यक CLI (Command Line Interface) 명령어를 안내합니다.

## 사전 준비

개발을 시작하기 전에 다음 소프트웨어가 시스템에 설치되어 있어야 합니다.

- [Node.js](https://nodejs.org/) (LTS 버전 권장)
- [Yarn](https://yarnpkg.com/) (npm 대신 yarn 사용)
- [Git](https://git-scm.com/)

## 프로젝트 구조

이 워크스페이스는 여러 개의 독립적인 리액트 프로젝트를 포함하고 있습니다.

- `hello-react`: Create React App (CRA) 기반의 기본 프로젝트
- `ch03-vite-test`: Vite 기반의 테스트 프로젝트
- `hello-react2`: Vite 기반의 또 다른 리액트 프로젝트
- `memo`: 개발 관련 메모를 저장하는 폴더

## 설치

각 프로젝트를 시작하기 전에 해당 프로젝트 폴더로 이동하여 의존성을 설치해야 합니다.

```bash
# 예시: hello-react 프로젝트 설치
cd hello-react
yarn install

# 예시: ch03-vite-test 프로젝트 설치
cd ../ch03-vite-test
yarn install
```

## 주요 명령어

각 프로젝트의 타입(CRA 또는 Vite)에 따라 사용하는 명령어가 다릅니다.

### Create React App (`hello-react`)

`hello-react` 폴더 내에서 다음 명령어를 사용할 수 있습니다.

- **`yarn start`**: 개발 모드로 앱을 실행합니다.
- **`yarn build`**: 프로덕션용으로 앱을 빌드합니다.
- **`yarn test`**: 테스트를 실행합니다.

### Vite (`ch03-vite-test`, `hello-react2`)

`ch03-vite-test`, `hello-react2` 폴더 내에서 다음 명령어를 사용할 수 있습니다.

- **`yarn dev`**: 개발 서버를 시작합니다. (HMR 지원)
- **`yarn build`**: 프로덕션용으로 앱을 빌드합니다.
- **`yarn preview`**: 빌드된 프로덕션 앱을 로컬에서 미리 봅니다.
- **`yarn lint`**: ESLint를 사용하여 코드 스타일을 검사합니다.
