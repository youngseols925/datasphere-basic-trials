# 데이터 모델링 소개 (Data Modeling Introduction)

> **원본 레슨**: dsp-overview-modeling-intro | **소요시간**: 2분

## 학습 목표
데이터 모델링의 시맨틱 사용 유형을 이해하고, 시나리오의 데이터 오브젝트 및 타겟 차원과 팩트 구조를 파악합니다.

## 주요 내용

### SAP Datasphere 데이터 모델링 개요
**Data Builder**에서 데이터를 가져오고, 결합하여 SAP Analytics Cloud 및 기타 BI 클라이언트에서 소비할 수 있도록 준비합니다. 원격/로컬 테이블 위에 그래픽 뷰와 SQL 뷰를 생성하여 데이터 모델링의 기반을 구축합니다.

### 시맨틱 사용 유형 (Semantic Usage Types)
- **Fact**: 분석 가능한 하나 이상의 측정값(Measure)을 포함하는 엔티티
- **Dimension**: 다른 엔티티의 측정값을 분석·분류하는 속성(Attribute)을 포함하는 엔티티
- **Hierarchy**: 차원 멤버의 부모-자식 관계를 포함하는 엔티티
- **Text**: 텍스트 속성 번역을 위한 언어 식별자가 포함된 문자열 엔티티
- **Relational Dataset**: 즉각적인 분석 목적 없이 일반적으로 중간 엔티티로 사용되는 컬럼 집합

### 단원 핵심 내용
- 데이터 수집 레이어의 원격/로컬 테이블 결합
- Dimension, Fact, Text 뷰 생성
- 뷰의 측정값 및 속성 시맨틱 조정
- 차원·텍스트·팩트 엔티티 간 연관(Association) 구성
- 차원 뷰의 마스터 데이터 영속화

### 이 단원에서 생성할 뷰
- **Product Dimension 뷰**: Products + Product Texts + Product Sentiments
- **Address Dimension 뷰**: Addresses + Countries
- **Business Partner Dimension 뷰**: Business Partners
- **Sales Fact 뷰**: Sales Order + Sales Order Items

## 핵심 포인트
- 데이터 모델링은 **Data Builder**에서 뷰(View) 형태로 수행
- 시맨틱 유형 지정으로 BI 도구가 데이터를 올바르게 해석 가능
- 모듈식 접근: **CENTRAL_DATA** 공유 데이터를 활용해 이전 단원 없이도 진행 가능

## 화면 스크린샷

![화면1](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/515_DSP_Data_Modeling/Images/515_1_image01.png)

![화면2](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/515_DSP_Data_Modeling/Images/515_1_image02.png)

![화면3](https://da4ug0lohul1.cloudfront.net/prod/AcademyContentFileImage/Trial_BTP-Datasphere/515_DSP_Data_Modeling/Images/515_1_image04.png)
