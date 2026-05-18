# 33. Open SQL Schema (데이터베이스 사용자 및 Open SQL Schema)

**소요 시간:** 약 15분

## 학습 목표

Database User 생성과 SAP HANA Cloud의 Open SQL Schema를 이해하고, 제품 카테고리 텍스트 데이터를 테이블에 적재한 후 SAP Datasphere 모델링 도구에서 재활용합니다.

## 주요 내용

SAP Datasphere 스페이스에 **Database User**를 생성하여 SAP Datasphere가 실행되는 SAP HANA Cloud 데이터베이스에 직접 쓰기 작업을 수행합니다. 각 Database User는 SAP Datasphere 스페이스 스키마와 연결된 **Open SQL Schema**를 보유합니다.

**SAP HANA Database Explorer** 또는 서드파티 SQL 도구를 통해 Open SQL Schema에 테이블을 생성하고 CSV 파일 업로드 또는 SQL INSERT 명령으로 데이터를 적재한 뒤, SAP Datasphere 모델링 도구에서 해당 데이터를 재사용합니다.

### 단계별 실습

**1단계: Database User 생성**
1. 좌측 내비게이션 메뉴에서 **Space Management** 선택
2. 내 스페이스의 **Edit** 버튼 클릭
3. 스페이스 속성 화면에서 **General Settings**의 Space ID 확인
4. **Database Users** 섹션으로 이동 후 **Create** 선택
5. **Create Database User** 팝업에서 이름 접미사 입력 및 스페이스 스키마의 Read/Write 옵션 설정
6. **Deploy**로 Database User 배포 → 접속 정보(호스트명, 포트, 인증서) 확인

**2단계: Database User로 로그인**
- SAP HANA Database Explorer에 Database User 자격증명으로 접속

**3단계: 테이블 생성 및 데이터 적재**
- Open SQL Schema에 테이블 생성
- CSV 파일 업로드 또는 SQL INSERT 명령으로 제품 카테고리 텍스트 데이터 삽입

**4단계: Data Builder에서 테이블 확인**
- **Data Builder**를 열어 Open SQL Schema의 테이블이 SAP Datasphere에서 표시되는지 확인

**5단계 (선택): 데이터 모델 고도화**
- 새로 적재된 테이블을 기존 데이터 모델에 연결하여 모델 확장

> 💡 SAP Help Portal의 **Integrating Data via Database Users/Open SQL Schemas** 문서를 참조하세요.
