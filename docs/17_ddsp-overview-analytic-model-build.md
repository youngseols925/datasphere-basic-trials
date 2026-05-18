# 17. Analytic Model 정의 (Define the Analytic Model)

**소요 시간:** 약 15분

## 학습 목표

Sales Fact 뷰와 Business Partner, Product 차원을 가져와 측정값 및 차원 속성을 정리하고, 측정값 모델링 및 입력/필터 변수를 설정합니다.

## 주요 내용

이 단원에서는 **Sales Analytic Model**을 생성하고 분석 소비를 위해 준비합니다. Sales Fact의 측정값과 차원 속성, 연결된 Business Partner 및 Product 차원을 지정합니다.

### 단계별 구성 내용

**Analytic Model 생성 (Add Fact Model)**
1. 사이드 네비게이션에서 **Data Builder** 선택
2. 필요 시 개인 스페이스 선택
3. **New Analytic Model** 선택 후 편집기 열기
4. **Repository** 섹션에서 **Sales Fact** 검색
5. **Sales Fact**를 캔버스에 드래그 앤 드롭
   - 이전 단원에서 Sales Fact를 생성하지 않은 경우 **4OV_Sales Fact** 사전 정의 오브젝트 사용
6. 팝업에서 모든 측정값, 속성, 연결 차원이 기본 선택됨 → **Select** 버튼 클릭

**측정값 및 차원 설정 (Set Measures and Dimensions)**

캔버스에서 팩트/차원 노드를 선택하면 측정값, 속성, 차원 연계를 사이드 패널에서 추가/제거할 수 있습니다.

**측정값 유형별 정의**

| 측정값 유형 | 설명 |
|---|---|
| **Calculated Measure** | 기존 측정값을 기반으로 계산식 정의 |
| **Restricted Measure** | 특정 조건으로 필터링된 측정값 |
| **Count Distinct Measure** | 고유값 개수 측정 |
| **Exception Aggregation Measure** | 예외 집계 방식 측정값 |

**변수 설정**
- **Input Variable**: 분석 시 동적으로 값 변경 가능
- **Filter Variable**: 필터 조건을 변수로 정의

**배포 (Deploy Analytic Model)**

모든 설정 완료 후 **Deploy** 버튼으로 Analytic Model을 배포합니다.

> 💡 더 자세한 내용은 SAP Help Portal의 **Creating an Analytic Model** 문서를 참조하세요.
