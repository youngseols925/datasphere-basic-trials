# Product Dimension 정의

> **원본 레슨**: dsp-overview-product-dimension | **소요시간**: 10분

## 학습 목표
Dimension 시맨틱 유형의 그래픽 뷰를 생성하고, 제품 관련 데이터를 결합·필터링하여 Product Dimension을 완성합니다.

## 주요 내용

### 개요
이 레슨에서는 **Product Dimension** 뷰를 생성합니다. 이전 단원의 제품 정보와 감성 데이터를 조인하고, SQL 표현식으로 필터링하며, 불필요한 컬럼을 제외하는 Projection을 추가합니다. 마지막으로 뷰 데이터를 SAP Datasphere에 영속화합니다.

### 1단계: Product Dimension 뷰 생성
1. **Data Builder**를 선택하고 스페이스를 선택합니다.
2. **New Graphical View** 타일을 클릭하여 뷰 편집기를 엽니다.
3. 왼쪽 소스 트리 패널의 **Repository** 탭에서 `Products` 원격 테이블을 캔버스로 드래그합니다.
   - 이전 단원에서 생성하지 않은 경우 공유 오브젝트 `4OV_Products`를 사용합니다.

### 2단계: Product Text 조인
1. 소스 트리에서 `ProductTexts` 테이블을 캔버스로 드래그합니다.
2. **Products** 노드와 **ProductTexts** 노드를 **Join** 노드로 연결합니다.
3. 조인 조건: `Products.ProductID = ProductTexts.ProductID`
4. 언어 필터를 추가하여 특정 언어 텍스트만 표시합니다.

### 3단계: Sentiment 데이터 조인
1. `ProductSentiments` 테이블을 캔버스로 드래그합니다.
2. 기존 조인 결과와 **Left Outer Join**으로 연결합니다.
3. 조인 조건: `ProductID` 컬럼 기준

### 4단계: 필터 추가
1. **Filter** 노드를 추가합니다.
2. SQL 표현식으로 조건을 정의합니다 (예: 특정 카테고리 필터링).

### 5단계: Projection 추가
1. **Projection** 노드를 추가합니다.
2. 분석에 불필요한 컬럼을 제외합니다.

### 6단계: 속성 시맨틱 설정
1. 출력 노드를 선택하고 **Semantic Usage**를 **Dimension**으로 설정합니다.
2. 키 속성(**Key Attribute**)을 지정합니다: `ProductID`
3. 각 컬럼의 시맨틱 유형(Label, Text 등)을 설정합니다.

### 7단계: 데이터 미리보기
- **Data Preview** 기능으로 Dimension 데이터를 확인합니다.

### 8단계: 저장, 배포 및 영속화
1. 뷰를 **저장(Save)**하고 **배포(Deploy)**합니다.
2. 배포 후 **Enable Data Persistence**를 활성화하여 뷰 데이터를 물리적으로 저장합니다.
3. 영속화 실행 후 데이터 새로고침 스케줄을 설정할 수 있습니다.

## 핵심 포인트
- **Graphical View**로 코드 없이 직관적인 데이터 모델 구성 가능
- **Join** 노드로 여러 테이블의 데이터 결합 가능
- **Dimension** 시맨틱 설정 후 SAC에서 분석 차원으로 활용
- **Data Persistence**로 성능 최적화 및 오프라인 분석 지원

![스크린샷](../screenshots/12_dsp-overview-product-dimension.png)
