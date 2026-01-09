---

description: "Task list template for feature implementation"
---

# Tasks: [FEATURE NAME]

**Input**: Design documents from `/specs/[###-feature-name]/`
**Prerequisites**: plan.md (required), spec.md (required for user stories)

**Organization**: Tasks are grouped by user story to enable independent implementation and testing of each story.

## Format: `[ID] [P?] [Story] Description`

- **[P]**: Can run in parallel (different files, no dependencies)
- **[Story]**: Which user story this task belongs to (e.g., US1, US2, US3)
- Include exact file paths in descriptions

## Path Conventions

- **Next.js App**: `app/`, `components/`, `lib/`, `tests/` at repository root

<!-- 
  ============================================================================
  IMPORTANT: The tasks below are SAMPLE TASKS for illustration purposes only.
  
  The /speckit.tasks command MUST replace these with actual tasks based on:
  - User stories from spec.md (with their priorities P1, P2, P3...)
  - Feature requirements from plan.md
  
  Tasks MUST be organized by user story so each story can be:
  - Implemented independently
  - Tested independently
  - Delivered as an MVP increment
  
  DO NOT keep these sample tasks in the generated tasks.md file.
  ============================================================================
-->

## Phase 1: Setup

**Purpose**: Project initialization and basic structure

- [ ] T001 Create project structure per implementation plan
- [ ] T002 Initialize ESLint and Prettier
- [ ] T003 Configure Vitest and React Testing Library

---

## Phase 2: User Story 1 - [Title] (Priority: P1) 🎯 MVP

**Goal**: [Brief description of what this story delivers]

**Independent Test**: [How to verify this story works on its own]

### Tests for User Story 1 (TDD) ⚠️

> **NOTE: Write these tests FIRST, ensure they FAIL before implementation**

- [ ] T004 [P] [US1] Write failing unit test for [component] in `tests/components/[component].test.tsx`
- [ ] T005 [P] [US1] Write failing integration test for [user flow] in `tests/[flow].test.tsx`

### Implementation for User Story 1

- [ ] T006 [P] [US1] Create [Component] in `components/[component].tsx`
- [ ] T007 [US1] Implement [logic] in `lib/[logic].ts`
- [ ] T008 [US1] Create page in `app/(pages)/[page]/page.tsx`
- [ ] T009 [US1] Ensure all tests for US1 are passing
- [ ] T010 [US1] Run ESLint and Prettier checks

**Checkpoint**: At this point, User Story 1 should be fully functional and testable independently

---

[Add more user story phases as needed, following the same pattern]

---

## Phase 3: Polish & Cross-Cutting Concerns

**Purpose**: Improvements that affect multiple user stories

- [ ] TXXX [P] Documentation updates
- [ ] TXXX Code cleanup and refactoring
- [ ] TXXX Performance optimization
- [ ] TXXX Security hardening
- [ ] TXXX Final verification of 70% test coverage

---

## Implementation Strategy

### TDD and MVP First (User Story 1 Only)

1. Complete Phase 1: Setup
2. Write failing tests for User Story 1
3. Implement User Story 1 until tests pass
4. **STOP and VALIDATE**: Test User Story 1 independently
5. Deploy/demo if ready

### Incremental Delivery

1. Complete Setup
2. Add User Story 1 (TDD) → Test independently → Deploy/Demo (MVP!)
3. Add User Story 2 (TDD) → Test independently → Deploy/Demo
4. Each story adds value without breaking previous stories
