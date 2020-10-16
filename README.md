# TEAM 얼죽아

### CACAO : Cafe Caffeine Open

카카오는 같은 음료라도 카페마다 다른 영양 정보를 조회하고 각자 다른 선호도에 맞게 음료를 골라 먹을 수 있도록 비교할 수 있는 서비스입니다.

카카오 서비스를 계획하게 된 이유는

<img align="left" width="600px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/Ingredient%20table.PNG" alt="성분표" />

</br></br></br></br></br></br></br></br>

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

<img width="700px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EA%B8%B0%ED%9A%8D%EC%95%88.PNG"  />

</br></br>

#### 프로젝트 세부 일정 및 간트표

![WBS간트차트](https://github.com/multicampus-cloud2/Portfolio/blob/master/img/WBS%EA%B0%84%ED%8A%B8%EC%B0%A8%ED%8A%B8.PNG)

## 화면 설계

kakao oven - https://ovenapp.io/view/nhaTPgzdKBGwJzxT9SXvnfEDKGDHBZPf/sZGR1 <img align="right" width="100px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/oven6.PNG" alt="oven6"/>



#### 화면 설계 프로토타입

<img width="500px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/oven1.PNG" alt="oven1"/>

> 네비게이션 바 - 버튼 클릭시 동적으로 One 페이지에서 변경
>
> 광고 배너 - S3 버킷에 있는 광고 이미지 불러오기
>
> 광고 배너 변경 버튼 - 버튼 클릭 시 광고 이미지 변경

<img width="600px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/oven2.PNG" alt="oven2"  />

> 카페 / 음료 / 콤보박스 선택 시 화면 동적으로 변경

<img width="500px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/oven3.PNG" alt="oven3" />

> 음료 이미지 클릭 시, 상세정보와 담기 버튼이 보임
>
> 담기 버트 클릭 시, 성분 비교 박스에 들어가서 타 제품과 비교 가능

<img width="500px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/oven4.PNG" alt="oven4" />

> 음료 비교 창 - 모달창으로 구현
>
> 음료 2 ~ 3잔을 화면에 출력
>
> 브랜드별 현재 위치에서 가장 가까운 위치 확인 가능

<img width="500px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/oven5.PNG" alt="oven5" />

> 서비스 소개 작성
>
> 개발자 소개 - 이미지 위에 마우스 hover 시, 이름 / instagram / github 주소 확인 가능

## 웹 스크래핑을 이용한 음료 제품 정보 데이터 가져오기

#### 써드파티 모듈 사용 목록

* requests, Selenium, BeautifulSoup, sqlalchemy, pandas, numpy, pymysql

※ 총 8개의 브랜드 웹 스크래핑 중 2개만 표시

#### 엔젤리너스

![WEB-angelinus](https://github.com/multicampus-cloud2/Portfolio/blob/master/img/WEB-angelinus.PNG)

#### 탐앤탐스

![WEB-tomntoms](https://github.com/multicampus-cloud2/Portfolio/blob/master/img/WEB-tomntoms.PNG)

#### 스크래핑한 결과를 DB에 Import

![WEB-DB임포트](https://github.com/multicampus-cloud2/Portfolio/blob/master/img/WEB-DB%EC%9E%84%ED%8F%AC%ED%8A%B8.PNG)

## AWS-IAM를 이용한 그룹 권한 관리

* 하나의 루트 사용자로 IAM 사용자를 여럿으로 나누어 하나의 애플리케이션을 관리
  * 팀원 모두 프로젝트를 통해 AWS 서비스를 이용해보고 배우기위해 권한은 동등하게 배분

<img  width="400" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/AWS-IAM(group).PNG" alt="AWS-IAM(group)" />

<img width="400px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/AWS-IAM(%EA%B4%80%EB%A6%AC%ED%98%95%EC%A0%95%EC%B1%85).PNG" alt="AWS-IAM(관리형정책)" />

<img width="400px" src="https://github.com/multicampus-cloud2/Portfolio/blob/master/img/AWS-IAM(%EC%9D%B8%EB%9D%BC%EC%9D%B8%EC%A0%95%EC%B1%85).PNG" alt="AWS-IAM(인라인정책)" />

## AWS를 이용한 CI / CD

#### 자동화된 지속적 통합 및 지속적 전달 릴리스 워크플로

![20_11_12. codepipeline구조](https://github.com/multicampus-cloud2/Portfolio/blob/master/img/20_11_12.%20codepipeline%EA%B5%AC%EC%A1%B0.PNG)

* CodePipeLine에 등록한 Github - master 브랜치에 변경 사항이 생기면 소스코드를 가져옵니다.
* 수동 승인을 통해 코드를 검토하고 승인 또는 철회합니다.
* 승인된 코드는 정적 웹 호스팅 S3 버킷(운영서버)에 자동으로 배포 및 업데이트 해 줍니다.

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

* IAM : 각 IAM 사용자 그룹 권한 관리

* CloudFront : CDN 기능과 Auth0에서의 `Http`주소의 통신 문제(`HTTPS`만 사용 가능), S3 버킷에서의 특정 폴더에 대한 `URL redirection`을 설정
* Certificate manager : 도메인을 승인 받기 위한 자격 증명 이용
* Route53 : DNS 이용
* S3-bucket : 웹 호스팅(Static Web-hosting) 실제 운영 서버로 이용
* API-Gateway : 웹사이트의 운영 서버와 DB 연동을 위한 게이트웨이 설정
* Lambda : RDS 서비스와 연동하여 DB 데이터를 조회
* RDS(MySQL) : 카페 제품 정보와 사용자 정보 관리
* CloudWatch : 각 브랜드마다 최신 제품 정보를 업데이트(웹 스크래핑) 하기 위한 주기 설정
* SNS : 신제품이 출시할 시 해당하는 브랜드 S3 버킷에 사진을 업로드할 시  사용자에게 Notify 발생
* CodePipeLine (Github, Code-commit, 관리자 수동 승인, Code-deploy) : 운영 서버 코드 배포 자동화

#### UI 화면 구성

* React (FrontEnd)

#### 버전 및 형상 관리

* Git, Github
* Slack (참조 링크, 코드업로드, 문서 관리 등)
* WBS (Work Breakdown Structure)

## 문제 해결 과정

* 원하는 시점에 Rendering 불가능 (FrontEnd)
  * 왜? Class형 컴포넌트에 필요한 함수가 없었기 때문해결! Function 형 컴포넌트 (React Hook)을 이용해 컴포넌트가 mount / unmount 될 때 동적으로 state를 갱신하여 해결
* Auth0 인증 및 카카오맵 API 호출되지 않는 문제 (Auth0 로그인)
  * 왜? 보안을 위해 HTTPS 프로토콜에서만 동작하기 때문해결! AWS CloudFront를 이용해 기존의 HTTP url을HTTPS로 리다이렉팅하여 해결
* 컴포넌트 객체가 모두 같이 동작하는 문제
  * 왜? 부모 컴포넌트의 state로 동작하도록 구현했기 때문해결! 자식 컴포넌트에서 state를 선언해 객체마다 따로동작할 수 있도록 하여 해결
* CodePipeline 자동배포 문제
  * 리액트 앱으로 개발을 마친 상태에서 npm run build를 통해 Static Web hosting S3 서비스를 이용하려고 하였지만, S3 서비스의 호스팅 서비스 특성상 root 폴더 경로에 있는 파일밖에 인식을 하지 못해 자동화 구현에 애를 먹었었지만 CloundFront와 error 페이지 경로를 우회해서 들어가는 방법을 터득하여 문제를 해결할 수 있었다.
    이번에 처음 써보는 AWS 기능을 시행착오를 겪어가며 알아본 경험은 앞으로의 문제 해결 능력에 자신감을 붙여준거 같아 좋았다.

## 개선 방향

* 지역상권을 살릴 수 있는 방안 - 사용자가 직접 입력하여 데이터 추가 및 확장
  * 개인 카페 포함, 여러 카페 데이터 통합 및 신뢰성 있는 데이터를 제공해 사용자와 업주 모두에게 만족할 만한 서비스를 구현 및 보완
* 광고 배너 삽입 자동화
  * 웹 스크래핑 코드와 AWS 서비스 개선을 통해 광고 배너 이미지를 주기적 수집 및 업데이트
* 신제품 알림 수신거부 기능
  * 사용자가 처음 해당 서비스에 가입하였을 때 등록하였던 선호 브랜드에 대한 광고 SMS 수신거부 기능 추가 / 개인 정보 보호 가능
* 커스텀 메뉴 공유
  * 사용자 간 레시피 공유 기능 추가 / 커뮤니티 활성화 기대
* 모바일 앱 UI 개선
  * 반응형 웹 구현 /  멀티 디바이스에 대해서도 대응이 가능하도록 해상도에 따라 UI 자동 조정