# <img src="https://private-user-images.githubusercontent.com/190439817/431173194-b0117f89-0016-43b7-abca-fd93144802ac.svg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDQwNzczMTAsIm5iZiI6MTc0NDA3NzAxMCwicGF0aCI6Ii8xOTA0Mzk4MTcvNDMxMTczMTk0LWIwMTE3Zjg5LTAwMTYtNDNiNy1hYmNhLWZkOTMxNDQ4MDJhYy5zdmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwOFQwMTUwMTBaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1hZjRkYzdkYWRlM2ZhNDhjNDBmYjM4MzM1ZTQyNWVkYmE1ZGQwMWQyZGFkNDZkNDBhNTNhOWI5MDZmYTI0N2U2JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.YdwtF5zFNknIBFLp_wc7aJMHYGmVRe_X-Fv7fU-zfW0">

> 반려견 산책 메이트를 찾고, 정보를 공유하며, 사용자 간 소통이 이루어지는 **반려견 커뮤니티 플랫폼**입니다.

---

## 프로젝트 개요

- **프로젝트명**: 댕근 (DaengGeun)
- **목표**: 반려견 산책 메이트 매칭, 실시간 채팅, 커뮤니티, 마켓 기능을 통해 반려견 보호자 간의 활발한 교류를 지원하는 플랫폼 구축

---

## 주요 기능

- 회원가입 / 로그인 (S3 이미지 업로드, 지역 자동추출, 암호화)
- 마이페이지 (프로필 및 반려견 정보 수정)
- 커뮤니티 게시판 (글/댓글 CRUD, 카테고리 필터링, 조회수)
- 산책 메이트 매칭 (랜덤, 좋아요 기반)
- 실시간 채팅 (WebSocket + STOMP 기반)
- 인기 강아지 랭킹
- 박람회 정보 제공
- 중고 상품 거래 마켓

---

## 기술 스택

### 💻 Front-End

<p align="left">
  <img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=white">
  <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white">
  <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/css3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/nginx-009639?style=for-the-badge&logo=nginx&logoColor=white">
  <img src="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
  <img src="https://img.shields.io/badge/amazonec2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white">
  
</p>

### 🖥 Back-End

<p align="left">
  <img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
  <img src="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
  <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">
  <img src="https://img.shields.io/badge/amazonrds-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white">
  <img src="https://img.shields.io/badge/amazons3-569A31?style=for-the-badge&logo=amazons3&logoColor=white">
  <img src="https://img.shields.io/badge/amazonec2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white">
  
</p>

---

## 아키텍처

### EC2 배포 구조
![EC2 Architecture](./댕근%20서비스%20아키텍쳐%20ec2.png)

### Local 개발 구조
![Local Architecture](./댕근%20서비스%20아키텍쳐%20로컬.png)

---

## 팀원 및 담당 기능

| 이름 | 역할 | 주요 구현 기능 |
|------|------|----------------|
| **나진수** (팀장) | 회원가입, 로그인, 메인, 매칭, 채팅, 랭킹, 박람회 | - S3 업로드, 주소 자동 추출<br> - STOMP 실시간 채팅<br> - 인기 랭킹 UI 구현 |
| **유경현** | 마이페이지, 마켓 | - 프로필/반려견 정보 수정<br> - 상품 CRUD, 댓글 관리<br> - 이미지 미리보기, 자동 로그인 |
| **이효진** | 커뮤니티 | - 게시글/댓글 CRUD<br> - 카테고리 필터, 조회수 증가<br> - 권한 기반 수정/삭제 |

---

##  구현 범위

### 필수
- 회원가입/로그인 처리 (S3 포함)
- 게시판 기본 기능
- 마이페이지 기본 수정

### 중요
- 매칭 및 좋아요 반영
- 커뮤니티 필터링 기능

### 추가
- 실시간 채팅방 생성
- 박람회 및 랭킹 기능
- 마켓 상품 정렬/댓글

---

## 프로젝트 일정

| 단계 | 기간 | 주요 작업 |
|------|------|-----------|
| 기획 | 3/5 ~ 3/7 | 아이디어 선정 및 기획안 작성 |
| 분석 | 3/10 ~ 3/12 | 요구사항, 기능 구조도, WBS 작성 |
| 설계 | 3/13 ~ 3/14 | DB 설계 및 CSS 정의 |
| 개발 | 3/17 ~ 3/28 | 프론트/백엔드 개발 |
| 테스트 | 3/31 ~ 4/1 | 기능 테스트 및 최종 수정 |

---

## 협업 도구

- GitHub (Issues, Pull Request)
- Figma
- Postman

---

## 커뮤니케이션 계획

- **주 2회 오프라인 회의**
- **GitHub Issues**를 통한 실시간 이슈 관리

---

## 프로젝트 구조 (개선 버전)

- DaengGeun/
  - README.md : 프로젝트 설명 문서
  - .gitignore : Git 무시 파일 설정
  - .github/
    - workflows/
      - fe-deploy.yml : 프론트엔드 CI/CD 설정
      - be-deploy.yml : 백엔드 CI/CD 설정
  - frontend/ (React 기반)
    - public/
    - src/
      - assets/ : 이미지, 폰트 등 정적 자산
      - components/ : 공통 UI 컴포넌트
      - hooks/ : 커스텀 React 훅
      - pages/ : 라우트별 페이지
      - apis/ : Axios API 함수 모음
      - store/ : 상태관리 (Recoil, Redux 등)
      - utils/ : 유틸 함수
      - App.tsx
    - .env : 환경변수
    - package.json : 프론트엔드 의존성 및 스크립트
  - backend/ (Spring Boot 기반)
    - src/
      - main/
        - java/com/daenggeun/
          - config/ : 보안, WebSocket 등 설정
          - controller/ : API 컨트롤러
          - dto/ : 요청/응답 데이터 전송 객체
          - entity/ : JPA 엔티티 클래스
          - repository/ : DB 접근 레이어
          - service/ : 비즈니스 로직
          - DaengGeunApplication.java : 메인 실행 파일
        - resources/
          - application.yml : 설정 파일
          - static/ : 정적 리소스
    - Dockerfile : 백엔드용 도커 파일
    - build.gradle : 빌드 설정
  - docker/
    - nginx/ : Nginx 설정
    - docker-compose.yml : 전체 서비스 묶는 도커 컴포즈
  - docs/
    - 프로젝트계획서.docx
    - 요구사항정의서.ods
    - wbs.xlsx

