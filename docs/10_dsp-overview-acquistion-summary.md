# 데이터 수집 요약 (Data Acquisition Summary)

> **원본 레슨**: dsp-overview-acquistion-summary | **소요시간**: 2분

## 학습 목표
데이터 수집 단원에서 배운 내용을 정리합니다.

## 주요 내용

### 단원 요약
이 단원에서는 SAP 및 비SAP 소스로부터 다양한 방법으로 데이터를 수집하는 방법을 실습했습니다.

**실습한 데이터 수집 방법:**
- **Replication Flow**: SAP HANA Cloud에서 Sales Order, Sales Order Items 테이블 복제
- **Data Flow**: Google Cloud Storage에서 제품 감성 데이터 로드 및 변환
- **Remote Table (페더레이션)**: Microsoft SQL Server와 SAP BW/4HANA에서 비즈니스 파트너, 제품 데이터 가상 접근
- **CSV 업로드**: 국가 데이터 직접 업로드

**생성된 데이터 오브젝트:**
- SalesOrder, SalesOrderItems (복제 테이블)
- ProductSentiments (Data Flow 결과 테이블)
- BusinessPartners, Addresses (Remote Table, 영속화)
- Products, ProductTexts (Remote Table, 페더레이션)
- Countries, CountryTexts (로컬 테이블, CSV 업로드)

### 다음 단계
수집된 데이터를 기반으로 **Data Modeling** 단원에서 차원(Dimension)과 팩트(Fact) 뷰를 구성합니다.

## 핵심 포인트
- 페더레이션과 복제를 비즈니스 요건에 맞게 조합하여 사용
- 모든 수집 오브젝트는 **CENTRAL_DATA** 공유 스페이스에도 사전 준비되어 있음
- 다음 단원(Data Modeling)을 독립적으로 시작할 수 있음

## 화면 스크린샷

![화면1](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_8_image01.png)

![화면2](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/510_DSP_Data_Acquisition/Images/510_8_image03.png)
