# 19. [Optional] Analytic Model 템플릿 사용

**소요 시간:** 약 5분

## 학습 목표

모델 직접 생성 대신 Analytic Model 템플릿을 가져와서 미리보기를 실행하고, SAP Analytics Cloud 시각화 단원으로 이어갈 수 있습니다.

## 주요 내용

이전 단원(**Define the Analytic Model**)에서 Sales Analytic Model을 직접 생성하지 않은 경우, 사전 정의된 템플릿 파일을 가져와 사용할 수 있습니다.

**핵심 참고사항:** Analytic Model은 다른 SAP Datasphere 스페이스로 공유(Share)할 수 없습니다. 따라서 JSON 파일 형태로 제공되며, 개인 스페이스에 직접 임포트해야 합니다.

### 사전 정의된 오브젝트 위치

- 스페이스: **CENTRAL DATA**
- 폴더: **WORKBOOK_OVERVIEW**
- 공유 오브젝트 이름 접두사: `4OV_`

### 단계별 실습

**JSON 파일 업로드**
1. `4OV_SALES_ANALYTIC_MODEL.JSON` 파일을 로컬에 다운로드
2. 사이드 네비게이션에서 **Data Builder** 선택
3. 개인 스페이스 선택
4. **Import** 아이콘 → **Import Objects from CSN/JSON File** 선택
5. 다운로드한 JSON 파일 선택
6. 팝업에서 **4OV_Sales Analytic Model** 선택 후 **Import CSN File** 클릭

**모델 배포 및 열기 (Deploy and Open Model)**
1. 임포트 완료 알림 확인
2. **Deploy** 버튼으로 모델 배포
3. 배포 완료 후 모델 열기
4. **Preview** 전환하여 데이터 확인

> 이 템플릿을 통해 SAP Analytics Cloud와의 라이브 연결(Live Connection) 소스로 활용할 수 있습니다.
