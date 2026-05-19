# Remote Tables 정의

> **원본 레슨**: dsp-overview-remote-table | **소요시간**: 5분

## 학습 목표
비즈니스 파트너 데이터 소스에 접근하기 위한 Remote Table을 정의합니다.

## 주요 내용

### 개요
두 개의 소스 시스템(Microsoft SQL Server, SAP BW/4HANA)에서 Remote Table을 가져와 스페이스에서 데이터를 사용 가능하게 합니다. 페더레이션(가상) 방식으로 접근하므로 원본 데이터는 소스 시스템에 그대로 남아 있습니다.

### 1단계: SQL Server 소스 연결 확인
1. 사이드 내비게이션에서 **Connections**를 선택합니다.
2. **MSSQL** 연결을 선택하고 **Validate**를 클릭합니다.
3. 연결 가용성 및 지원 기능 메시지를 확인합니다.
4. **BW4_DSP** 연결도 동일하게 검증합니다.

### 2단계: 제품 데이터 소스에 페더레이션 접근
Microsoft SQL 데이터베이스를 기반으로 제품 영역 테이블 2개를 가져옵니다.
1. **Data Builder**를 선택합니다.
2. **New Graphical View**를 클릭하여 그래픽 뷰 편집기를 엽니다.
3. **Sources** 패널에서 **MSSQL** 연결의 제품 테이블을 드래그하여 추가합니다.
4. 뷰를 저장합니다. 데이터는 SAP Datasphere가 아닌 SQL Server에 유지됩니다.

### 3단계: 비즈니스 파트너 데이터에 페더레이션 접근
SAP BW/4HANA의 aDSO(Advanced DataStore Object)를 **Data Builder** 시작 페이지에서 직접 가져옵니다.
1. **Data Builder** 시작 페이지에서 **Import Remote Tables**를 선택합니다.
2. **BW4_DSP** 연결에서 Business Partners, Addresses aDSO를 선택합니다.
3. 가져오기를 완료합니다.

### 4단계: 비즈니스 파트너 데이터 영속 접근으로 전환
페더레이션 Remote Table을 영속 데이터로 전환합니다.
1. 가져온 Remote Table을 열고 **Enable Data Replication**을 활성화합니다.
2. 복제를 실행하면 데이터가 SAP Datasphere 스페이스에 저장됩니다.

## 핵심 포인트
- Remote Table은 데이터를 이동하지 않고 소스 시스템에 직접 연결
- Microsoft SQL, SAP BW/4HANA 등 다양한 소스 지원
- 페더레이션 → 영속 데이터로 클릭 한 번에 전환 가능
- **Graphical View Editor**와 **Import Remote Tables** 두 가지 방식으로 가져오기 가능

## 화면 스크린샷

![화면1](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image01.png)

![화면2](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image04.png)

![화면3](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image12.png)

![화면4](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image13.png)

![화면5](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image14.png)

![화면6](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image15.png)

![화면7](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image16.png)

![화면8](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image20.png)

![화면9](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image18.png)

![화면10](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image19.png)

![화면11](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image25.png)

![화면12](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image26.png)

![화면13](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image27.png)

![화면14](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image28.png)

![화면15](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image29.png)

![화면16](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_5_image30.png)
