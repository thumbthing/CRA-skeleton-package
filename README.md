# CRA 초기 세팅 파일 

# 프로젝트 생성 날짜: 2023/09/10

> 라이브러리 버전은 이 날짜를 기준으로 최신 버전을 적용

---

## 목적

CRA로 프로젝트 생성 후 불필요한 파일 제거 및, 초기 세팅 뼈대용 프로젝트

---

## 버전

node: 18.17.0

---

### 세팅 목록

---

#### Package.json

- dependecies

```javascript
  "dependencies": {
    "@testing-library/jest-dom": "^5.17.0",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^13.5.0",
    "@types/jest": "^27.5.2",
    "@types/node": "^16.18.48",
    "@types/react": "^18.2.21",
    "@types/react-dom": "^18.2.7",
    "axios": "^1.5.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-router-dom": "^6.15.0",
    "react-scripts": "5.0.1",
    "styled-components": "^6.0.7",
    "typescript": "^4.9.5",
    "web-vitals": "^2.1.4"
  },
```

- devDependencies

```javascript

"devDependencies": {
    "@typescript-eslint/eslint-plugin": "^6.6.0",
    "@typescript-eslint/parser": "^6.6.0",
    "eslint": "^8.48.0",
    "eslint-config-airbnb": "^19.0.4",
    "eslint-config-airbnb-typescript": "^17.1.0",
    "eslint-config-prettier": "^9.0.0",
    "eslint-import-resolver-typescript": "^3.6.0",
    "eslint-plugin-import": "^2.28.1",
    "eslint-plugin-jsx-a11y": "^6.7.1",
    "eslint-plugin-prettier": "^5.0.0",
    "eslint-plugin-react": "^7.33.2",
    "eslint-plugin-react-hooks": "^4.6.0",
    "husky": "^8.0.3",
    "lint-staged": "^14.0.1",
    "prettier": "^3.0.3"
  },
  "lint-staged": {
    "*.{ts,tsx}": [
      "prettier --write",
      "eslint --fix"
    ]
  }
```

- scripts

```javascript
 "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject",
    "lint": "eslint --cache './src/**/*.{ts,tsx,js,jsx}'",
    "lint:fix": "eslint --fix './src/**/*.{ts,tsx,js,jsx}'",
    "prettier": "prettier --write --config ./.prettierrc './src/**/*.{ts,tsx}'",
    "postinstall": "husky install",
    "format": "prettier --cache --write .",
    "prepare": "husky install"
  },
```

---
#### lint, prettier

airbnb 규칙을 기반

---
#### husky

pre-commit, pre-push

> commit, push 명령어 수행시 husky 작동을 안할 경우엔 husky 스크립트의 권한 수정 필요

---
#### README 기초 템플릿

# `[패키지 이름을 작성]`

---

## 기능

---

## 실행방법

---

## 프로젝트 구조

---

## Commit Convertion

| Type 키워드 | 사용 시점                                                             |
| ----------- | --------------------------------------------------------------------- |
| Feat        | 새로운 기능 추가                                                      |
| Fix         | 버그 수정                                                             |
| Docs        | 문서 수정                                                             |
| Style       | 코드 스타일 변경 (코드 포매팅, 세미콜론 누락 등)기능 수정이 없는 경우 |
| Design      | 사용자 UI 디자인 변경 (CSS 등)                                        |
| Test        | 테스트 코드, 리팩토링 테스트 코드 추가                                |
| Refactor    | 코드 리팩토링                                                         |
| Build       | 빌드 파일 수정                                                        |
| Ci          | CI 설정 파일 수정                                                     |
| Chore       | 빌드 업무 수정, 패키지 매니저 수정 (gitignore 수정 등)                |
| Rename      | 파일 혹은 폴더명을 수정만 한 경우                                     |
| Remove      | 파일을 삭제만 한 경우                                                 |

---

### 사용 라이브러리

---



---

