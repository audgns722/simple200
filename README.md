# 프로젝트 개요

이 프로젝트는 React, Node.js, MongoDB, AWS S3, Firebase 등을 사용하여 블로그를 구현한 것입니다.

## 개발 환경

React v18.1.0
Node.js v18.0.0
MongoDB v5.0.6
AWS S3
Firebase

## 설치
서버(SERVER)
```bash
npm init -y
npm install express
npm install nodemon --save
npm install path --save
npm install mongoose --save
npm install multer --save
npm install --s aws-sdk@2.348.0
npm install multer-s3 --save "multer-s3": "^2.10.0",
```
클라이언트(CLIENT)
```bash
npx create-react-app .
npm install react-bootstrap bootstrap
npm install react-router-dom
npm install axios
npm install http-proxy-middleware
npm install @emotion/css
npm install @emotion/react
npm install @emotion/styled
npm install sass
npm install firebase
npm install react-redux
npm install @reduxjs/toolkit

npm run build
```

## 프로젝트 구성

client
├── App.js
├── components
│   ├── Header.js
│   ├── Post.js
│   └── Footer.js
├── index.css
└── index.html

server
├── index.js
└── model
    ├── Post.js
    └── Counter.js

## 프로젝트 제작 과정

초기 설정
React 애플리케이션을 생성하고 필수 패키지를 설치합니다.
README.md 파일을 생성합니다.
서버 제작
Express 프레임워크를 사용하여 서버를 생성합니다.
MongoDB를 연결합니다.
CORS를 설정합니다.
body-parser를 사용하여 요청 데이터를 처리합니다.
MongoDB에 게시물을 저장합니다.
클라이언트 제작
React Router를 사용하여 라우팅을 구현합니다.
Axios를 사용하여 서버와 통신합니다.
emotion 라이브러리를 사용하여 CSS 스타일을 적용합니다.
react-redux를 사용하여 상태 관리를 구현합니다.
트러블슈팅
클라이언트에서 text를 보내려는데 undefind 메시지 출력: body-parser 미들웨어를 사용하지 않아서 발생한 문제입니다. body-parser 미들웨어를 사용하면 요청 데이터를 처리하여 JavaScript 객체로 변환할 수 있습니다.
프로젝트 결과

이 프로젝트를 통해 React, Node.js, MongoDB, AWS S3, Firebase 등을 사용하여 블로그를 구현하는 방법을 배울 수 있습니다.

향후 계획

사용자 인증 및 권한 관리 기능을 추가합니다.
댓글 기능을 추가합니다.
검색 기능을 추가합니다.
기타

이 프로젝트는 개인적인 학습 목적으로 만들어졌습니다.
이 프로젝트의 코드는 MIT 라이선스로 공개되어 있습니다.
server config .env

MONGODB_URI=mongodb://localhost:27017/reactblog
FIREBASE_API_KEY=
FIREBASE_AUTH_DOMAIN=
FIREBASE_DATABASE_URL=
FIREBASE_PROJECT_ID=
FIREBASE_STORAGE_BUCKET=
추가 정리

트러블슈팅 부분에 git rm --cached . -rf 명령어를 추가했습니다. 이 명령어는 .gitignore 파일에 지정된 파일을 제외하고 .git 캐시를 삭제합니다.
서버 제작 과정 부분에 body-parser 미들웨어 사용 항목을 추가했습니다. 이 항목에서는 body-parser 미들웨어를 사용하여 요청 데이터를 처리하는 방법을 설명합니다.