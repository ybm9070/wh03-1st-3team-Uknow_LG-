## 내 마음 LG 서비스 

 고객 상담 이력 자동분석 서비스 기획 및 설계


프로젝트 3팀 : 유병민, 장성권, 김수민, 최동욱





1. 서비스 목적

	상담 이력 자동분석을 이용한 키오스크 판매 시스템 구현






2. 서비스 배경

	문제의식  

 ![123](https://github.com/user-attachments/assets/496e46ec-ac83-4b3a-908c-211f51e86412)


	디즈니는 직원 수가 계속 증가했지만, 고객 만족도는 점차 감소하는 경향을 보였습니다. 
	이는 비효율적 직원 관리가 고객 경험에 부정적인 영향을 미쳤을 가능성을 시사합니다.


	비용적 손실 , 시간적 손실 , 기회적 손실, 기타 손실 발생



3. 서비스 목표 설정

상담 이력 자동화
실시간 데이터 업데이트 시스템 구축으로 효율성 향상
개인화 추천 및 불만족 사례 탐지
데이터 분석과 고객 세분화로 마케팅 최적화
자동화로 운영 비용 절감 및 고부가가치 업무 집중 유도.





키오스크 사용 절차

![image02](https://github.com/user-attachments/assets/246746ec-13dd-41f3-af12-2f24c351843e)

![image03](https://github.com/user-attachments/assets/09f18aea-42e9-4a31-a784-aad854877d16)

프로젝트 일정

기간 2025년 1월~ 2025년 5월



## 데이터 설계




기술 스택:

프로그래밍 언어: Python

데이터베이스: MySQL, Redis

서버: AWS EC2, Nginx

API: Flask (RESTful API)

LLM : LangChain

검색: Elasticsearch

API: FastAPI



# work flow

![image04](https://github.com/user-attachments/assets/c5324af7-aaa0-4628-9477-3d73ca8f847c)





# 주요 데이터 속성

• OrderHistory:

• order_id : id

• user_id : (FK)

• product_id : 제품번호

• order_date : 주문날짜

• quantity : 수량

• total_price : 총 가격

• order_type : 현금 , 신용카드

• Counsellinfo:

• counsel_id : 상담번호

• user_id : FK=id

• curious_product : 관심품목

• visit_purpose: 관람 ,상담, 구매

• is_purchases : 구매 여부



• User:

• id : PK

• Name : 고객명

• Age : 나이

• Gender : 성별

• Job : 직업

• Address : 거주지

• VisitLogs:

• user_ id : (FK)

• visit date : 방문 날짜

• visit location : 방문지점



  
	ERD
![image05](https://github.com/user-attachments/assets/2edd0932-e267-4f1a-b747-6cf359c45159)



## 리스크 관리


1. 기술적 위험

(1) 기기 오작동

(2) AI 상담 실시간 정보 부족, 모델의 한계로 인한 정확도 하락



2. 사용자 경험 위험

(1) 사용자 인터페이스(UI)의 복잡성

(2) 고객 신뢰 부족



## 기대 효과

1. 운영 효율성 강화


2. 고객 만족도 향상


3. 데이터 기반 의사결정


4. 기업 경쟁력 향상


5. 환경적, 사회적 가치


