---
layout: post
title: 성능테스트7
date: 2018-03-01
tags: 정리글
author: SeonDH

---


### Part5 Plan and Design Tests (테스트 계획 및 디자인)

#### ch12. Modeling Application Usage(애플리케이션 사용 모델링)

##### Overview
웹 로드 테스트의 일반적인 목적은 사용자의 경험을 가능한 현실적으로 시뮬레이션 하는 것이다. 이를 위해서는 테스크된 워크 로드가 실제 운영 시나리오를 따라야한다. 신뢰 할 수 있게 성능을 예측하는 것은 쉽지 않고, 포괄적인 작업이 아니다. 비현실적인 워크 로드 모델을 시뮬레이션하는 것은  성능 테스트를 수행할 때 팀에 유용한 정보를 제공할 수 있는 것은 분명하지만, 실제 워크 로드 모델을 시뮬레이션 할 때에만 프로덕션 환경의 성능을 예측하거나 최적화 우선 순위를 지정할 수 있다.

##### Approach for Modeling Application Usage (모델링을 위한 접근법)

- 목표 확인
- 주요 사용 시나리오 확인
- 주요 시나리오의 탐색 경로 지정
- 개별 사용자 데이터 및 분산을 결정
- 시나리오의 상대적 분포를 결정
- 목표 부하 수준을 확인
- 모델 구현 준비

각각의 자료들을 수치화해서 쓴다.

##### Summary
생산 성능을 이해, 예측 또는 조정하기 위해 성능 테스트를 실시 할때는 조건이 실제 상황과 비슷해야 하는 것이 중요하다. 정확하고 예측 가능한 테스트 결과를 위해 사용자가 웹 사이트와 상호 작용하는 방식관 관련된 지표들을 기반으로 모델링해야 한다.

#### ch13. Determining Individual User Data and Variances(개별 사용자 데이터 및 변수 결정)

##### Overview
개별 사용자 지연, 사용자 데이터 및 종료를 결정하는 프로세스를 설명한다. 성능 테스트를 통해 프로덕션 환경의 어플리케이션을 이해하는 것에 직접적으로 활용할 수 있는 결과를 얻으려면 워크로드가 실제 프로덕션 환경과 유사해야 한다. 대표적인 사용자 군에서 발견되는 것과 유사한 가변성과 무작위성으로 사용자를 모델링 해야한다.

##### Consequences of Improperly Modeling User Delays(부적절한 모델링 사용자 지연)
모든 사용자가 똑같이 들어올 것이라고 예상하는 것은 부적절한다. 실제 사용자를 잘 표현한 자료를 사용해야한다.
1. 사용자 지연 결정
2. 지연 범위 결정:
세가지의 정보가 필요하다.
  - 최소 지연 시간
  - 최대 지연 시간
  - 지점 간의 사용자 지연 분포 혹은 패턴
3. 분포 적용
대부분의 유형의 분포는 네가지의 수학적 모델을 따른다
  - 선형 분포
  - 정규 분포
  - 음의 지수 분포
  - double hump 정규 분포

위의 자료 등을 기반으로 실제 사용자에 맞게 적절히 모델링을 해야한다.

##### Summary
실제 사용자 지연 테스트를 설계하는 프로세스는 정확한 결과를 생성하는데 매우 중요하다. 정확한 결과를 위해 테스트된 워크로드가 사용자 지연 패턴과 같아야한다. 대표적인 사용자 군에서 발견되는 것과 유사한 가변성과 무작위성으로 사용자를 모델링 해야한다.