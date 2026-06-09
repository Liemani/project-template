# README.md

## structure

- extracted: 원문 그대로 추출한 md 파일
- wiki: 위키
- requirements: 요구사항 관리 시스템
- tasks: 구현 작업 단위 관리
- decisions: 설계/구현 결정 기록

## requirements system

`requirements/`는 템플릿 프로젝트에서 요구사항을 독립적으로 관리하기 위한 영역이다.

- `index.md`: 요구사항 목록과 현재 상태를 한눈에 보는 레지스트리
- `backlog.md`: 아직 정제되지 않았거나 우선순위만 잡힌 항목
- `template.md`: 개별 요구사항 문서 템플릿
- `items/`: 개별 요구사항 문서 보관 위치

## delivery layers

- `tasks/`: 요구사항을 구현 가능한 작업 단위로 분해해 관리하는 영역
- `decisions/`: 구현 방식, 트레이드오프, 선택 근거를 기록하는 영역

권장 흐름:

1. `raw/`에 원문 유입
2. `extracted/`에 기계 추출 결과 저장
3. `wiki/`에서 사람 기준으로 맥락 정리
4. `requirements/backlog.md`에 요구사항 후보 등록
5. 정제된 요구사항을 `requirements/items/REQ-xxx-*.md`로 승격
6. `tasks/`에서 구현 작업으로 분해
7. 필요한 설계 판단은 `decisions/`에 기록
8. `requirements/index.md`에서 현재 상태를 관리

## implementation rules

- 요구사항은 "무엇을 해야 하는가"를 정의한다.
- `tasks/`는 "어떻게 나눠서 진행하는가"를 정의한다.
- `decisions/`는 "왜 이 방식으로 구현하는가"를 남긴다.
- `approved` 이상인 요구사항은 가능하면 관련 task 또는 decision 링크를 가져야 한다.
