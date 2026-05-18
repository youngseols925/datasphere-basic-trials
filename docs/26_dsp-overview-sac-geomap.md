# 26. Geo Map 추가 (Add Geo Map)

**소요 시간:** 약 10분

## 학습 목표

**Choropleth** 레이어가 포함된 Geo Map을 Story에 추가합니다.

## 주요 내용

SAP Analytics Cloud는 추가 라이선스 없이 **ESRI** 지도 통합을 기본 제공합니다. SAP HANA Spatial 기술과 결합하여 비즈니스 데이터를 지리 정보 위에 오버레이할 수 있습니다.

> 💡 SAP Datasphere 모델에는 이미 지리 정보(Geo Enriched Data)가 포함되어 있습니다.

### 단계별 실습

**Geo Map 생성**
1. Story 편집 모드 열기
2. 템플릿 메인 레인의 `+` **Create a Geo Map** 플레이스홀더 선택
3. **Right Side Panel (Builder, Styling)** 열림

**Amount 레이어 추가**
- Choropleth 레이어: 지리적 형태(음영 표시) 또는 버블로 차원과 측정값을 시각화
1. **Builder** 탭 → **Content Layers** → `+` **Add Layer** 선택
2. **Layer Type**을 **Choropleth / Drill** 로 변경
3. **Style**을 **Bubble** 로 변경
4. **Layer Name**을 `Amount` 로 지정
5. **Available Objects** 에서 측정값 선택

**Geo Map 탐색 (Navigate the Geo Map)**
- 지도 상에서 지역별 매출 데이터를 버블 크기/색상으로 확인
- 지역 드릴다운으로 세부 데이터 탐색

> 💡 SAP Help Portal의 **Geo Maps** 문서를 참조하세요.
