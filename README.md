⭐️Portfolio - Almeal
======================

📝개요
=======
* 프로젝트 명 : Almeal
* 일정 : 2022.05 ~ 2022.06
* 인력 구성 : BE 5명 / FE 1명
* 프로젝트 목적 : 팀 프로젝트로서 Spring과 MyBatis 활용능력을 기르기 위한 프로젝트
* 나의 역할 : 회원 관리, 마이페이지, 비밀번호 찾기 이메일 인증 구현
* 개발 환경
  + Server : Apache-tomcat-8.5
  + Java EE IDE : Eclipse 
  + Database : MySQL
  + Programming Language : JAVA, CSS, JavaScript, SQL
  + Framework/Flatform : Spring, MyBatis, jQery 3.5.1, Bootstrap v5
  + API : Kakao Login, Naver Login, CoolSMS
  + Version management : (https://github.com/wurstel/ITWill_team_Spring.git)
* * *

📝내용
=======
* 개발 환경
  + 회원가입 및 로그인
  + 마이페이지 구현
  + 공지사항 게시판
  + 상품 리스트 및 결제
  + 구독 정기결제
  + 관리자 페이지 구현
 
📝ERD
=======
## 상품과 회원을 기준으로 DB 설계
![ERD2](https://user-images.githubusercontent.com/104838354/177591389-3e6eb6e4-ed27-4a01-a8c2-156aa6d98329.png)

📝구현 기능
=======
## 회원가입 및 로그인

### 1. 회원가입 
#### 일반 회원가입
![회원가입](https://user-images.githubusercontent.com/104838354/177592260-2cdfce4a-647d-4365-ace2-ed1c7f0d4f7c.gif)

#### 회원가입 성공 후 메일 인증 
![회원가입메일인증](https://user-images.githubusercontent.com/104838354/177592427-db0d1eda-5cd9-4369-8916-c63499bc7407.gif)

#### 메일 인증 후 로그인
![회원가입후로그인](https://user-images.githubusercontent.com/104838354/177592462-5da17504-a636-4f61-9b19-c987f8fecb3d.gif)

* 구현 기능 설명
  + 아이디 중복 체크
  + 비밀번호 정규표현식, 일치 여부 판별
  + 다음 우편번호 API
  + 비밀번호 암호화
  + 회원가입 완료 후 메일 인증 필수
  
  
### 2. 로그인
#### 네이버 로그인
![네이버로그인](https://user-images.githubusercontent.com/104838354/177592645-c6302d58-4412-45d2-9729-2278acc0d906.gif)

#### 카카오 로그인
![로그인](https://user-images.githubusercontent.com/104838354/177592682-fcf1665e-ef49-40b4-bf44-00d66188c34f.gif)

### 3. 아이디, 비밀번호 찾기
#### 아이디 찾기
![아이디찾기](https://user-images.githubusercontent.com/104838354/177594714-ddabc6a3-0c1b-44f3-a26d-bd5f2455fed3.gif)

![아이디찾기완료](https://user-images.githubusercontent.com/104838354/177594770-19b5affe-248b-43a8-8132-c46294dc2ad2.gif)

#### 비밀번호 찾기
![비밀번호찾기](https://user-images.githubusercontent.com/104838354/177594860-174e4150-2509-4d32-8d7f-6479b3cfdb15.gif)

![비밀번호찾기메일인증](https://user-images.githubusercontent.com/104838354/177594906-ce2e9588-0990-429a-9990-7a009de4dc9d.gif)

#### 비밀번호 변경
![비밀번호변경](https://user-images.githubusercontent.com/104838354/177595010-ef754d10-2593-46fc-a289-3b59829f4607.gif)

![비밀번호변경후로그인](https://user-images.githubusercontent.com/104838354/177595063-5835a9b7-c00b-40d3-aadd-16bacd426ccb.gif)

* 구현 기능 설명
  + 일반 로그인
  + 카카오 로그인
  + 네이버 로그인
  + 아이디 찾기를 위한 SMS 인증
  + 비밀번호 찾기를 위한 SMS, 이메일 

---------------------------------------
