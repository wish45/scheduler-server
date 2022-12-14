### 스킬셋
Java, Spring Boot, Jpa, MySQL, Java 11, JUnit, mokito


### 로그파일 저장 경로
C:\Users\newhyodong\pjt\log

### 결제정보파일 읽어들이는 경로
C:\Users\newhyodong\pjt

![image](https://user-images.githubusercontent.com/23456264/198540700-9d30097d-f1e5-49f6-a69b-3ee81c1ffc29.png)


# 작업내용

### 1. 스케쥴러를 통한 결제정보 저장 api 구현

### 2. 결제정보 등록, 수정, 삭제, 조회 api 구현
<ol>application.yml에 설정된 ip에 한에서 접근가능</ol>
<ol>aop를 통한 메서드 전후에 실행시간 로그기록</ol>

### 3. api호출시 JWT + spring security를 통한 인증 및 인가 작업 구현


### 4. api 테스트 코드 작성
<ol>test code (진행중)</ol>


# 구동 방법

### 1. data.sql에 쿼리문으로 h2디비에 데이터 생성

### 2. http://localhost:8080/api/authenticate  를 호출하여 token 생성
![image](https://user-images.githubusercontent.com/23456264/192147197-8407aa4b-fc49-48cc-aa9d-efa537b0a64b.png)


### 3. api 호출
<ol>get- http://localhost:8080/payment</ol>
<ol>post- http://localhost:8080/payment</ol>
<ol>del - http://localhost:8080/payment/deletePayment</ol>
<ol>patch - http://localhost:8080/payment/updatePayment</ol>

### 4. 스케쥴러는 매 12시정각에 C:\Users\newhyodong\pjt 위치에서 데이터를 읽어서 디비에 저장.

### 5. jmeter 를 활용한 부하테스트 진행

### 6. 분산락을 이용한 동시성 이슈 해결(redis)

### 7. 향후 계획
<ol> DDD 중심으로 리팩토링하기 </ol>

