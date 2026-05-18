# Sales Fact 데이터 모델 생성

> **원본 레슨**: dsp-overview-sales-fact | **소요시간**: 10분

## 학습 목표
Fact 시맨틱 유형의 그래픽 뷰를 생성하고, 차원 뷰들과 연관을 설정하여 분석용 Sales Fact 모델을 완성합니다.

## 주요 내용

### 개요
**Sales Fact** 뷰를 생성합니다. Sales Order와 Sales Order Items 테이블을 조인하여 팩트 뷰를 만들고, Product·Business Partner·Address Dimension과 연관을 설정합니다.

### 1단계: Sales Fact 뷰 생성
1. **Data Builder**에서 **New Graphical View**를 선택합니다.
2. **Repository** 탭에서 `SalesOrder` 테이블을 캔버스로 드래그합니다.
3. `SalesOrderItems` 테이블도 드래그하여 **Join** 노드로 연결합니다.
4. 조인 조건: `SalesOrderID` 기준 조인

### 2단계: 뷰 속성 설정
1. 출력 노드를 선택하고 Business Name을 `Sales Fact`로 변경합니다.
2. **Semantic Usage**를 **Fact**로 설정합니다.
3. Fact 유형으로 설정 시 측정값(Measure) 설정 탭이 활성화됩니다.

### 3단계: 측정값(Measure) 설정
1. 수치형 컬럼(금액, 수량 등)을 **Measure**로 지정합니다.
2. 집계 함수(SUM, COUNT 등)를 설정합니다.

### 4단계: 차원 Association 추가
1. **Association** 탭에서 다음 차원들과 연관을 추가합니다:
   - `Product Dimension` — ProductID 기준
   - `Business Partner Dimension` — BusinessPartnerID 기준

### 5단계: Projection 추가
- 분석에 불필요한 컬럼을 제외합니다.

### 6단계: 저장 및 배포
1. 뷰를 **저장(Save)**하고 **배포(Deploy)**합니다.

## 핵심 포인트
- **Fact** 시맨틱 설정으로 측정값과 차원 연관 구성 가능
- 여러 차원과 연관된 팩트 뷰가 Star Schema의 중심
- **Analytic Model**에서 이 팩트 뷰를 기반으로 분석 레이어 구성
- Fact 뷰는 영속화 불필요 (차원 뷰에서 영속화)

![스크린샷](../screenshots/15_dsp-overview-sales-fact.png)
