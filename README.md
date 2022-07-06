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
#### SMS 인증 후 아이디 찾기 완료
![아이디찾기](https://user-images.githubusercontent.com/104838354/177594714-ddabc6a3-0c1b-44f3-a26d-bd5f2455fed3.gif)

![아이디찾기완료](https://user-images.githubusercontent.com/104838354/177594770-19b5affe-248b-43a8-8132-c46294dc2ad2.gif)

#### 비밀번호 찾기
#### SMS , 이메일 인증 후 비밀번호 변경
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
## 마이페이지 구현

### 1. 회원정보 수정
![회원정보수정](https://user-images.githubusercontent.com/104838354/177597870-9682a3e8-a562-4f07-8fa2-291329e202f2.gif)

* 구현 기능 설명
  + 이메일, 전화번호, 주소 정보 변경

### 2. 회원 탈퇴
* 구현 기능 설명
  + 비밀번호 확인 후 회원 탈퇴

### 3. 장바구니
#### 장바구니 수량 변경
![장바구니수량](https://user-images.githubusercontent.com/104838354/177597693-69438545-3bae-4e8f-be89-ef64372f2e06.gif)

#### 장바구니 삭제
![장바구니삭제](https://user-images.githubusercontent.com/104838354/177597676-b4fd72ae-8a0d-447f-adaf-01b78617acfd.gif)

* 구현 기능 설명
  + 수량 변경 및 삭제 시 alert창으로 한번 더 확인
  
### 4. 장바구니
#### 리뷰 쓰기
---------------------------------------
## 공지사항 게시판

### 1. 공지사항 조회

* 구현 기능 설명
  + 공지사항 게시판 글 목록 조회
  + 페이징 처리를 통해 게시글 목록 조회
  + 게시판 글 작성
  + 게시글 상세 조회
  + 목록으로 이동
 
### 2. 공지사항 조회

* 구현 기능 설명
  + 게시글 수정 시, 원래 등록된 게시글 제목, 내용 불러옴
  + 수정 버튼 클릭 시 수정된 게시글 상세조회 가능

### 3. 공지사항 삭제

* 구현 기능 설명
  + 삭제 버튼 클릭 시 게시물 삭제

---------------------------------------
## 상품 리스트 및 결제
### 1. 상품 메인 페이지
![상품리스트](https://user-images.githubusercontent.com/104838354/177602791-5d9473ab-7857-4274-9802-fd61266dbaad.gif)

![페이징처리](https://user-images.githubusercontent.com/104838354/177603060-c8d03931-1420-49b2-a7dc-0541454cb60c.gif)

* 구현 기능 설명
  + 상품 정렬(최신순, 평점순, 낮은 가격순, 높은 가격순)
 
### 2. 상품 상세 페이지
#### 리뷰 평점, 신상품, best 상품 아이콘
![상품상세](https://user-images.githubusercontent.com/104838354/177603778-677f28b8-6542-40f2-b930-ad47cee9cd52.png)

* 구현 기능 설명
  + 상품 등록 후 2주동안 new 아이콘 뜨기
  + 평점 4점 이상 best 아이콘 뜨기
  + 리뷰 정렬(최신순, 평점순)

#### 장바구니 담기
![장바구니담기](https://user-images.githubusercontent.com/104838354/177603234-099b23be-7917-49f6-a9bd-8ea46357ed90.gif)

* 구현 기능 설명
  + 수량 변경 후 장바구니 담기
  
### 3. 상품 결제
#### 주문하기
![주문하기이동](https://user-images.githubusercontent.com/104838354/177604673-80be8bb1-74f9-4308-9503-02dc51f5d31f.gif)

#### 주문 완료 후 마이페이지 주문 조회로 이동
![일반결제](https://user-images.githubusercontent.com/104838354/177604977-488089f5-9502-406c-8e31-80b6e9bf9cdf.gif)

* 구현 기능 설명
  + 주문 완료 후 장바구니에서 내역 삭제
  + 로그아웃 상태에서 장바구니/주문하기 버튼 누르면 로그인 페이지로 이동

### 3. 상품 검색
#### 상품 키워드로 검색
![상품검색](https://user-images.githubusercontent.com/104838354/177605192-94fe797f-8284-4aae-9225-defadf67f09c.gif)

* 구현 기능 설명
  + 상품 이름에 포함된 키워드를 입력하면 키워드를 포함한 상품이 검색됨
  + 검색된 총 상품 갯수 구현
  
---------------------------------------
## 구독 정기결제
### 1. 구독 페이지
![구독](https://user-images.githubusercontent.com/104838354/177605738-44ff3e7e-d482-40bb-805d-7c3797f0da29.gif)

* 구현 기능 설명
  + 스탠다드, 프리미엄 중 선택

#### 정기결제
![정기결제](https://user-images.githubusercontent.com/104838354/177605803-09ba2c15-a0be-4f88-ab4d-d6b0bfd017ae.gif)

* 구현 기능 설명
  + 카카오로 정기결제
---------------------------------------

## 관리자 페이지 구현

### 1. 상품 관리
#### 관리자 상품 삭제
![관리자상품삭제](https://user-images.githubusercontent.com/104838354/177606573-d7bf5928-de6f-4688-b294-bd3a3ef6fc36.gif)

* 구현 기능 설명
  + 삭제 시 한번 더 확인

### 2. 회원 관리
#### 관리자 회원 삭제
![관리자회원삭제](https://user-images.githubusercontent.com/104838354/177606598-0bead362-5baf-492b-8368-4985e2a4242a.gif)

* 구현 기능 설명
  + 삭제 시 한번 더 확인

### 3. 고객 센터
#### 고객센터 답글
![고객센터답글](https://user-images.githubusercontent.com/104838354/177606657-4b4d88b9-3a65-4fa4-a0be-867f5e38d93e.gif)

* 구현 기능 설명
  + Re: 제목에 표시

---------------------------------------

📝보완할 점
=======
* 정기 결제 후 멤버십 관리
* 관리자 대쉬보드 (매출 현황 차트 구현)
* 전체적인 오류 확인
