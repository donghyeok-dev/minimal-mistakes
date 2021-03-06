---

layout: customPost
title:  "JIRA와 Confluence"
categories: 
  - Tools
  - JIRA
---
### JIRA 소개

성공적인 프로젝트를 위해서는 팀이 더 효과적으로 업무를 수행하고 진행 상황과 의견을 공유하고 협업하며 업무 이력을 관리하는 것이 중요합니다. atlassian가 개발한 JIRA는 버그, 이슈 트래커, 요구 사항 관리, 애자일 소프트웨어 개발 관리까지 제공하는 `강력한 프로젝트 관리 도구`입니다.  제품군으로는 JIRA Software, JIRA Core, JIRA Align, JIRA Service Desk 등 다양한 제품군이 있으며 소규모(10인 이하) 이용자들은 무료로 이용할 수 있습니다. JIRA는 개별 업무의 이력을 검색 기능이 뛰어나며 검색 언어인 JQL(JIRA Query Language) 로 이슈를 상세 검색하는 방법도 제공합니다. 그 외에도 다양한 가젯과 플러그인을 제공합니다. 



### Confluence 소개

JIRA는 Issue, 일정 등 프로젝트 관리라면 Confluence는 프로젝트에 관련된  요구사항,  설계, 회의록 등의 문서를 관리하고 공유하는 솔루션입니다. Confluence는 스페이스 단위로 운영이 가능하며 각 스페이스 별 사용자 및 권한을 관리할 수 있습니다. 스페이스 내에 페이지(문서)들을 생성할 수 있으며, 페이지를 쉽게 꾸밀수 있도록 다양한 템플릿도 제공합니다. 또한 유료 플러그인 앱을 사용하면 기존 워드나 파워포인트를 페이지로 변환 및 편집 기능도 제공합니다.



JIRA와 Confluence는 상호 연동이 쉽게 되기 때문에 같이 사용하면 더욱 큰 힘을 발휘합니다.

JIRA와 Confluence의 간단한 사용방법을 소개합니다.



간단한 용어 정리

- Sprint : Epic 들을 진행하는 단위. (Sprint 1차, Sprint 2차 형식으로 진행될 수 있음)
- Issue Type
  - Epic : 1개 또는 여러 Sprint에 속할 수 있고 Stroy의 집합. 주로 Major Feature 중심의 작업 단위.
  - Story : UI와 직접적인 기능의 작업 단위.
  - Chore : UI와 관련되지 않는 작업들(Server Logging, Secure Coding 등)의 단위.
  - Improvement: 개선사항
  - New Feature :  새로운 기능
  - Task :  Story나 Chore들을 보통 3일 내에 끝나는 Task 작업 단위로 분리 함.
  - Sub Task : 만약 작업량이 많은 Task라면 Sub Task로 분리하여 여러 개발자가 진행하는 작업 단위.
  - Bug: 오류사항을 수정하는 작업 단위.
- Priority Levels(우선순위 레벨)
  - Blocker (긴급) : 가장 우선적으로 처리해야 할 이슈.
  - Critical (심각): 데이터 손실, 서비스 다운 등 심각한 결함과 같은 치명적인 이슈.
  - Major (높음): 기능 수행 자체에 영향을 주는 이슈.
  - Minor (보통): 기능의 최소한의 손실이나 간단한 문제점을 발생시키는 이슈.
  - Trivial (낮음):  오타 또는 간격 등 표면적이며 기능자체와 직접적인 연관은 없는 사소한 이슈.
- Status
  - TODO 또는 OPEN:  이슈 초기
  - In Progress: 검토 또는 개발 진행
  - Resolved: 해결
  - Reopened: 재시작
  - Closed: 종료
  - Done: 완료
- workflow : Status 상태의 흐름을 정의. (예 InProgress 상태에서는 Done상태로만 변경할 수 있다.)



## JIRA 사용방법



![image-20210316014333216](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/image-20210316014333216.png)

![N_2](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_2.PNG)



![N_3](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_3.PNG)

![N_5](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_5.PNG)

![N_6](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_6.PNG)

백로그에서  Epic, Task 등의 issue를 만들고 스프린트로 드래그&드랍하여 스프린트를 생성할 수 있습니다.

![N_14](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_14.PNG)

생성된 스프린트내에  issue들이  상태로 나뉘어 표시되고 드래그로 상태를 이동시킬 수 있습니다.



![N_8](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_8.PNG)

로드맵에서 Epic 단위로 작업의 디펜던시 및 시각화가 가능하고, Epic의 하위 Story 또는 Task 상태에 따라 Epic 아래 Progress 상태가 바뀝니다. 또한 완료된 issue는 가운데줄로 표시 해줍니다. 그 외 상단에 내보내기 기능으로 로드맵 이미지를 다운받을 수 있습니다.

![N_20](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_20.PNG)

issue 타입은 우측상단 설정 >  이슈 유형 구성표에서 설정 가능합니다.



Workflow 설정

![N_25](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_25.PNG)

![image-20210316020001792](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/image-20210316020001792.png)

![N_23](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_23.PNG)

![N_28](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_28.PNG)

![N_29](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_29.PNG)

![N_31](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_31.PNG)

![N_32_1](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_32_1.PNG)

![N_35](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_35.PNG)

![N_36](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_36.PNG)

![N_37](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_37.PNG)



스프린트 보더 설정하기 

![N_38](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_38.PNG)

![N_39](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_39.PNG)



버전관리

![N_40](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_40.PNG)

![N_41](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/N_41.PNG)





## Confluence 사용방법

![image-20210317013424287](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/image-20210317013424287.png)

![image-20210317013458018](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/image-20210317013458018.png)

![6](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/6.PNG)![5](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/5.PNG)

![7](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/7.PNG)



![image-20210317013815875](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/image-20210317013815875.png)



아래는 JIRA에서 Confluence의 문서를 등록하는 화면이며, Confluence에서도 JIRA Issue를 등록할 수 있습니다.

![10](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/10.PNG)

![image-20210317014021948](https://cdn.jsdelivr.net/gh/donghyeok-dev/donghyeok-dev.github.io@master/assets/images/posts/image-20210317014021948.png)