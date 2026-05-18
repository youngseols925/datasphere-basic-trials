# 32. Additional Content 소개 (Introduction)

**소요 시간:** 약 2분

## 학습 목표

추가 콘텐츠 단원의 전체 주제를 개관합니다.

## 주요 내용

이 단원에서는 SAP Datasphere의 추가 기능인 데이터 수집과 모델링의 심화 측면을 다룹니다. 이전 단원의 데이터 모델을 기반으로 하지만, **독립적으로 학습**할 수 있도록 자체 완결적으로 구성되어 있습니다.

### 주제 1: Open SQL Schema를 통한 데이터 통합

**Database User**를 생성하여 SAP Datasphere 스페이스에 연결하고, Open SQL Schema에 데이터를 읽고 쓰는 방법을 학습합니다.

- SAP Datasphere 스페이스가 노출하는 데이터를 읽거나 스페이스에 연결된 Open SQL Schema에 데이터를 쓰기 위한 **Database User** 생성
- ODBC를 통해 런타임 SAP HANA Cloud 데이터베이스에 접근하여 스페이스와 데이터를 안전하게 교환
- **SAP HANA Database Explorer**를 활용한 테이블 생성 및 데이터 삽입 실습
- 결과를 SAP Datasphere에 노출

### 주제 2: Data Access Control (행 수준 보안)

**Data Access Control**을 통해 오브젝트에 행 수준 보안(Row-Level Security)을 적용합니다.

- 데이터 접근 제어가 적용된 오브젝트를 직접 또는 소스로 사용하는 다른 오브젝트를 통해 조회하는 모든 사용자는, 지정된 기준에 따라 **권한이 있는 레코드만** 조회 가능
- 권한 테이블(Authorization Table)과 Data Access Control 정의
- Fact View에 Data Access Control을 연결하여 레코드 제한 적용 실습
