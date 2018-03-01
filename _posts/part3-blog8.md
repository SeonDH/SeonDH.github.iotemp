---
layout: post
title: 성능테스트5
date: 2018-03-01
tags: 정리글
author: SeonDH

---


### Part3 Identify the Test Environment (테스크 환경 식별)

#### ch8. Evaluating Systems to Increase Performance-Testing Effectiveness (성능 테스트 효율성 향상을 위한 시스템 평가)

##### Overview(개요)
시스템 평가는 성능 테스트 전반적으로 진행 중인 과정이지만, 특히 테스트 초기에 더욱 효과 있다. 시스템 평가의 목적은 성능 테스트에 도움이 되는 정보를 수집하는 것이다.
테스트 중인 시스템에 대한 철저한 이해는 성공적인 테스트 작업에 매우 중요하다. 이는 성능 요구 사항을 지정하고, 미리 위험을 식별하는 등 판단하기 위한 토대를 제공한다.

##### Capture System Functions and/or Business Processes(시스템 기능 및 비즈니스 프로세스 파악)
성능 수용 기준을 정의하는데 도움이 되는 핵심 기능을 식별한다. 성능 테스트를 위해서는 테스트 중인 시스템의 핵심 기능을 식별하는 것이 필수적이다. 시스템 기능을 결정하는 유용한 리소스는 다음과 같다.

- 시스템 결정 리소스
  - 이해 관계자 인터뷰
  - 계약서
  - 비슷한 응용 프로그램 사용 방법에 대한 정보
  - 고객의 기대
  - 유사한 응용 프로그램에 대한 자신의 경험
  - 디자인 문서
  - 상태 전이 다이어그램
  - 요구 사항 및 사용 사례
  - 마케팅 자료
  - 프로젝트 계획
  - 비즈니스 사이클
  - 주요 비즈니스 프로세스
- 참고 사항
  - 이해 관계자와 만나 시스템의 목적을 결정할 것
  - 계약과 문서는 시스템에 대한 이해 관계자의 관점에서 벗어날 수 있음을 명심
  - 인터뷰, 문서 및 계획에는 묵시적인 기능이 많이 포함 될 수 있음

##### Capture User Activities(사용자 활동 파악)
애플리케이션의 주요 사용자 활동을 식별한다. 모든 사용자의 활동을 식별하는 것은 불가능 하기 때문에 시뮬레이션 할 중요한 활동을 결정해야한다. 시스템 기능을 결정하는 유용한 리소스는 다음과 같다.

- 시스템 결정 리소스
  - 비슷한 응용 프로그램 사용 방법에 대한 정보
  - 고객의 기대
  - 유사한 응용 프로그램에 대한 자신의 경험
  - 요구 사항 및 사용 사례
  - 이해 관계자 인터뷰
  - 마케팅 자료
  - 도움말 및 사용자 문서
  - 고객 조직도
  - 네트워크 또는 응용 프로그램 보안 매트릭스
  - 과거 데이터 (송장, 웹 로그 등)
  - 주요 비즈니스주기 (월별 계산, 연말 프로세스, 5 년 보관 등)
- 참고 사항
  - 경쟁 업체를 평가할 것
  - 가능한 모든 범주의 사용자를 고려
  - 중요하다고 생각되거나 경쟁 애플리케이션의 활동이 누락 된 경우 빠르게 팀원에게 문의

##### Capture the Logical and Physical Architecture(논리적 및 물리적 아케텍처 파악)
응요 프로그램과 하드웨어 및 소프트웨어 구조 사이의 관계를 식별한다. 특정 관심 영역을 해결하고, 병목현상을 찾는 테스트를 설계 할 때 유용하다. 논리적 및 물리적 아키텍처를 파악하기 위해 기술적 이해 관계자, 설계자 및 관리자와 만나야 한다. 테스터는 시스템의 구성 요소 또는 계층이 서로 어떻게 통신하고 구성되는지 알아야 한다.

- Logical Architecture
  - 논리적 아키텍처란 소프트웨어 구조, 코드의 구조, 상호 작용 및 추상화를 의미한다. 웹 기반의 응용 프로그램의 가장 기본적인 아키텍처는 **3 계층 아키텍처** 이다.
    - 클라이언트 계층(사용자 시스템)
    - 프레젠테이션 계층(웹서버)
    - 데이터 저장소 계층(데이터베이스 서버)
  -논라적 아키텍처는 데이터의 흐름을 나타낸다
- Physical Architecture
  - 물리적 아키텍처는 실제 하드웨어를 이야기한다
- System Architecture
  - 논리적 및 물리적 아키텍처를 통합한 것
  - 아키텍처의 모든 측면을 포함하지는 않지만 성능 테스트의 중요한 지표

##### Summary(요약)
시스템 평가는 테스트 전반에 걸쳐 중요하지만 특히 초기에 더 중요하다. 테스트를 수행하는데 필요한 정보를 수집하고, 이 정보를 이용해 성능 목표 및 요구사항을 정의하고, 작업 부하 특징을 식병하고, 성능 테스트 전략 및 계획 작성, 위험 평가 등을 한다.