---
layout: post
title: 성능테스트6
date: 2018-03-01
tags: 정리글
author: SeonDH

---


### Part4 Identify Performance Acceptance Criteria(성능 허용 기준 파악)

#### ch9. Determining Performance Testing Objective(성능 테스트 목표 설정)

##### Overview
성능 테스트의 목표은 변화, 잠재적 위험 및 개선 기회를 파악하는 것이다.
테스트 목표를 결정할 때 다음과 같은 사항을 고려해야한다.
- 테스트 목표는 성능 검증 및 검증 활동의 시작점이다.
- 성능 테스트 목표는 비즈니스 진입점부터 시작한다. 이를 이용해 기술적 목적을 명확히 할 수 있다.
- 성능 테스트 목표는 비즈니스 요구 사항과 관련 있으므로 비즈니스 시나리오를 나타내야 한다.
- 큰 범위를 만들고 세분화 시킬 수 있다.

##### 용어 설명
- Performance-testing objectives(성능테스트 목표):
제품의 품질을 결정하거나 향상 시키는 것에 영향이 있다고 예상되는 성능 테스트 프로세스를 통해 수집된 데이터.
- Performance objectives(성능 목표):
응답 시간, 처리량 및 자원 활용도 수준
-  Performance targets(성능 목표):
응답 시간, 처리량 및 자원 활용도 수준 측면에서 지정된 프로젝트에 대해 식별 된 지표에서 원하는 값. 일반적으로 프로젝트 목표와 동일.
- Performance targets성능 임계값):
응답 시간, 처리량 및 자원 활용도 수준 측면에서 지정된 프로젝트에 대해 식별 된 지표의 최대 허용 값. 일반적으로 요구 사항과 동일.
- Performance budgets(성능 예산):
리소스에 대한 제약 사항.

##### Approach for Determining Performance Testing Objectives(성능 테스트 의 목표 설정)
- 전체 목표 결정
- 프로젝트 계획 검토
- 아키텍처 검토
- 팀원의 조언

##### Capture or Estimate Resource Usage Targets and Thresholds(리소스 사용 목표 및 임계 값 파악 또는 예상)
잘못 적용되기 쉽다. 일반적으로 프로세서 사용률이 80%를 초과하면 성능이 크게 저하됨. 이를 기반으로 70%를 Performance targets으로 하고 80%를 Performance targets로 한다. 제대로 된 이해 없이 목표롸 한계점을 설정하면 안 된다.

##### Capture or Estimate Resource Budgets(리소스 예산 파악 또는 예측)
리소스 예산 또는 할당을 결정하는 것은 팀이 함께 작업하여 목표 및 임계 값이 현실적인지 확인 하는 것이다.

##### Identify Metrics(지표 식별)
자료를 왜곡하지 않고 어디에 저장할 것인지 고민해야 한다.

##### Communicate Results(결과 전달)
객관적인 정보를 자유롭게 공유하는 것이 좋다. 잠재적 원인이 아닌 증상과 상태를 명확히 보고해야 한다.

##### Stay Aware of Changing Objectives, Targets, and Budgets (목표 및 예산 변경)
목표는 프로젝트가 진행되면서 변경 될 수 있다. 오래되고 관련성 없는 목표를 테스트하는 것은 시간 낭비이다.

##### Summary
프로젝트가 진행됨에 따라 성능테스트 목표는 수립되고 업데이트 된다. 잦은 소통으로 올바른 목표를 유지하는 것이 중요하다.

#### ch10. Quantifying End-User Response Time Goals(최종 사용자 응답 시간 목표 수치화)

##### Overview
사용자는 응답시간에 대해 수치를 알지 못한다. 애플리케이션이 느리게 보이는지 아닌지에 주목하며, 인상은 이전의 경험이나 기분 등 어떤 것이든지 기초할 수 있다. 사용자 인식을 숫자로 변환하는 방법에 대한 설명을 한다.

##### 용어 설명
- Performance requirements(성능 조건):
계약상의 의무, 수정될 수 없는 값.
- Performance goals(성능 목표):
특정 상황에서는 타협 가능하지만, 제품 출시 전 원하는 기준.

##### Quantify Captured Performance Requirements(파악한 성능 수치화)
- 요구 사항과 목표를 분리한다.
- 파악된 성능 목표를 수치화한다.
- 파악된 성능 조건을 수치화한다.

수치화하면서 여러가지는 고려해야한다.

##### Summary
응답 시간 목표의 수치화는 애플리케이션에 대한 사용자의 인식을 표현하는 것과 밀접한 관련이 있다. 대부분 사용자는 처리량, 트랜젝션 수 등 만으로 표현 할 수 없다. 사용자는 자신의 인상대로 동작을 파악한다. 이는 여러 요인의 결과이다.


#### ch11. Consolidating Various Types of Performance Acceptance Criteria(다양한 성능 허용 기준의 통합)

##### Overview
성능 요구 사항 및 목표는 여러가지 요인에서 영향을 받는다. 이러한 요인들에서 테스트의 목표를 단일 세트로 혼합하고 통합하는 방법을 설명한다.

##### Summary
성능 요구 사항 및 테스트 목표는 일반적으로 시스템 사용자, 사업체 소유자 및 프로젝트 팀의 관점, 규정 준수 기대치 및 기술적 고려 사항에서 도출된다. 시스템 수락 기준을 검증하기 위해 다른 관점에서 수집한 정보에 기초해야 하며, 이는 검증 가능하고 보완적인 성능 요건과 시험 목표의 단일 집합을 야기해야 한다. 가장 중요한 것은 애플리케이션 사용자가 성능 저하로 좌절하지 않아야 한다는 점이다.
