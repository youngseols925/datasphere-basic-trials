# 28. Linked Analysis 및 Input Controls

**소요 시간:** 약 10분

## 학습 목표

특정 위젯에만 필터를 적용하는 **Input Control**을 생성하고 **Linked Analysis**로 연결합니다.

## 주요 내용

**Input Control**은 차원 멤버를 동적으로 변경하여 위젯을 필터링합니다. 기본적으로 동일한 데이터 소스를 사용하는 모든 위젯에 필터가 적용되며, **Linked Analysis**로 특정 위젯에만 제한할 수 있습니다.

### 단계별 실습

**플레이스홀더 정리**
- 템플릿에 4개의 Input Control 플레이스홀더 중 2개만 필요 → 2개 삭제

**날짜 Input Control 생성 (연도 필터)**
1. 템플릿 Filter Lane의 `+` **Create an Input Control** 플레이스홀더 선택
2. **Dimensions** → **OrderCreationDate** → **Filter by Member** 선택
3. 연도 목록 확장 후 **2021, 2022, 2023** 선택 → **OK**
4. 위젯 크기 조절로 모든 연도 표시

**판매 조직 Input Control 생성 (SALESORG 필터)**
- 두 번째 플레이스홀더에서 **SALESORG** 차원으로 Input Control 생성

**Linked Analysis 설정**
- Input Control을 특정 위젯에만 연결
- 차트, 지도, 테이블 중 원하는 위젯만 선택하여 필터 적용 범위 제한

**Input Control 탐색**
- 연도 및 판매 조직 필터를 변경하면 연결된 위젯이 동적으로 업데이트

> 💡 SAP Help Portal의 **Input Controls** 문서를 참조하세요.
