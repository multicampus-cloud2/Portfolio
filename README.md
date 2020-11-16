# TEAM 얼죽아

### CACAO : Cafe Caffeine Open

카카오는 같은 음료라도 카페마다 다른 영양 정보를 조회하고 각자 다른 선호도에 맞게 음료를 골라 먹을 수 있도록 비교할 수 있는 서비스입니다.

카카오 서비스를 계획하게 된 이유는

<img align="left" width="500px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/Ingredient%20table.PNG" alt="성분표" />

</br></br></br></br></br></br></br>

- 심박 증가, 불면증 등 카페인에 대해 민감한 분들에게 영양 정보를 제공하여 소비자 성향에 맞는 커피를 고를 수 있게 하기 위함이며,
- 카페마다 구석에 배치한 영양 정보표로 접근성과 가독성이 떨어지는 것을 방지하는 동시에,
- 우리가 자주 이용하는 커피에 대해 더 똑똑하고 현명한 소비자가 될 수 있도록 커피 프렌차이즈 별로 쉽게 비교하고 가까운 위치까지 조회해 볼 수 있도록 제작하였습니다.

## TEAM 맴버

### <img align="left" width="60px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/teamwork.png" alt="teamwork"/> 김윤영 안예진 이재환 주성우

---

## 애플리케이션 워크 플로우 및 도식화

![service-workflow](https://github.com/multicampus-cloud2/Portfolio/blob/master/img/service-workflow.PNG)

## 화면 스케치 & 배포

링크 주소 참고 : https://www.caca0.shop/ (AWS 서비스를 이용한 배포)

## 프로젝트 목표

* **React.js, AWS Serverless**를 이용한 성분 비교 **SPA (Single Page Application)** 사이트 제작
* AWS 클라우드 서비스와 자동화(CI / CD) 인프라 구축

## 프로젝트 기획 및 세부 일정

<img align="left" width="700px" src="C:\Users\Nick_주성우\OneDrive\바탕 화면\지우기\프로젝트 기획안.PNG" alt="프로젝트 기획안"  />

#### 프로젝트 세부 일정 및 간트표

![WBS간트차트](C:\Users\Nick_주성우\OneDrive\바탕 화면\지우기\WBS간트차트.PNG)

## 화면 설계

kakao oven - https://ovenapp.io/view/nhaTPgzdKBGwJzxT9SXvnfEDKGDHBZPf/sZGR1 <img align="right" width="100px" src="C:\Users\Nick_주성우\OneDrive\바탕 화면\지우기\oven6.PNG" alt="oven6"/>



#### 화면 설계 프로토타입

<img width="500px" src="C:\Users\Nick_주성우\OneDrive\바탕 화면\지우기\oven1.PNG" alt="oven1"/>

<img width="600px" src="C:\Users\Nick_주성우\OneDrive\바탕 화면\지우기\oven2.PNG" alt="oven2"  />

<img width="500px" src="C:\Users\Nick_주성우\OneDrive\바탕 화면\지우기\oven3.PNG" alt="oven3" />

<img width="500px" src="C:\Users\Nick_주성우\OneDrive\바탕 화면\지우기\oven4.PNG" alt="oven4" />

<img width="500px" src="C:\Users\Nick_주성우\OneDrive\바탕 화면\지우기\oven5.PNG" alt="oven5" />



## 프로젝트 주요 기능

* 회원가입 및 로그인
  * 타사 자격증명 플랫폼을 이용한 Auth0 구현 및 사용자 선호 브랜드 지정 후 `AWS-SNS`알림 서비스
* 신제품 SNS 알림 발송
  * 사용자가 회원가입할 때 등록한 선호 브랜드를 지정하고 해당 브랜드에서 신제품이 출시될 시 `AWS-SNS` 기능을 통해 사용자가 등록한 핸드폰으로 신제품 알림 문자 발송
* 제품 상세 조회 및 비교
  * 각 브랜드 제품들의 영양 정보를 웹 스크래핑으로 취합해서 상품 전체 조회 및 개별 조회 가능
  * 최소 2개 ~ 최대 3개의 제품을 비교 창에 담아 비슷한 제품들을 시각화 해 정교하게 비교 가능
* 제품 필터링 기능
  * 제품의 상세 영양 정보뿐 아니라, 사용자가 원하는 기준을 토대로 순서대로 정렬(오름차순, 내림차순)
* 비교함에 담은 제품의 브랜드 위치 확인
  * 브랜드 위치 정보를 `Kakao API`를 이용해, 현재 위치에서 가장 가까운 매장을 알려줌

## 사용 기술

#### 웹 스크래핑

* WEB-Scraping (스타벅스, 할리스, 탐앤탐스, 이디야, 커피빈, 투썸플레이스, 엔제리너스, 빽다방)
  * 2019년 11월 기준 상위 10개 브랜드를 대상으로 스크래핑

#### 로그인 서비스 및 API

* Auth0(Google, Kakao)
* KaKao Location API (현재 위치에서 가까운 매장 찾기)

#### AWS Service

* IAM

* CloudFront
* Certificate manager
* Route53
* S3-bucket
* API-Gateway
* Lambda
* RDS(MySQL)
* CloudWatch
* SNS
* CodePipeLine (Github, Code-commit, 관리자 수동 승인, Code-deploy)

#### UI 화면 구성

* React (FrontEnd)

#### 버전 및 형상 관리

* Git, Github
* Slack (참조 링크, 코드업로드, 문서 관리 등)
* WBS (Work Breakdown Structure)

