# Requirements Index

이 문서는 현재 프로젝트의 정제된 요구사항 레지스트리다.

## status definitions

- `proposed`: 아이디어 또는 요청은 있으나 아직 요구사항으로 확정되지 않음
- `refining`: 범위, 예외, 승인 기준을 정리 중
- `approved`: 구현 가능한 상태로 승인됨
- `in_progress`: 구현 또는 반영 진행 중
- `done`: 승인 기준까지 반영 완료
- `obsolete`: 더 이상 유효하지 않음

## active requirements

| ID | Title | Type | Priority | Status | Source | Owner |
| --- | --- | --- | --- | --- | --- | --- |
| REQ-001 | 요구사항 intake와 추적 레이어 제공 | process | high | proposed | template bootstrap | - |

## usage rules

- 새 항목은 먼저 이 표에 등록한다.
- 상태가 `approved` 이상이면 반드시 `items/REQ-xxx-*.md` 문서가 있어야 한다.
- `Source`에는 `raw/`, `extracted/`, `wiki/`, 외부 요청 등 최초 근거를 적는다.
- 구현이 시작되면 관련 task, decision, 코드 경로를 개별 요구사항 문서에 연결한다.
- `done`으로 바꾸기 전에는 승인 기준별 검증 방법이 문서에 적혀 있어야 한다.

## status transition guide

- `proposed -> refining`: 요구를 구조화하고 범위를 정리하기 시작함
- `refining -> approved`: 범위, 승인 기준, 출처가 충분히 정리됨
- `approved -> in_progress`: 연결된 task를 만들고 구현에 착수함
- `in_progress -> done`: 승인 기준 검증까지 완료됨
