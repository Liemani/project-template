# DEC-001 Separate Requirements Tasks And Decisions

## Metadata

- ID: DEC-001
- Status: accepted
- Owner: project maintainer
- Requirement Links: REQ-001
- Task Links: TASK-001
- Last Updated: 2026-06-09

## Context

요구사항만으로는 실제 구현 책임, 작업 분해, 설계 판단을 함께 담기 어렵다. 템플릿 단계에서 각 역할을 분리하지 않으면 프로젝트마다 문서 의미가 뒤섞이기 쉽다.

## Decision

요구사항, 작업, 결정을 각각 `requirements/`, `tasks/`, `decisions/`로 분리한다.

## Alternatives Considered

- 요구사항 문서 하나에 구현 메모와 작업 상태를 모두 적는 방식
- `wiki/` 아래에서 모든 문서를 통합 관리하는 방식

## Consequences

- 장점: 추적성과 책임 단위가 명확해진다.
- 단점: 문서 수가 늘어나 초기 입력 비용이 조금 커진다.

## Links

- Requirements: `requirements/items/REQ-001-requirements-intake-and-traceability.md`
- Tasks: `tasks/items/TASK-001-bootstrap-requirement-delivery-layer.md`
- Code:
- Docs: `README.md`
