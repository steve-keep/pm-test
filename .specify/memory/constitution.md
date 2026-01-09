<!--
Sync Impact Report:
- Version change: 0.0.0 → 1.0.0
- List of modified principles: None
- Added sections: Core Principles, Development Workflow, Code Quality Gates, Governance
- Removed sections: None
- Templates requiring updates:
  - ✅ .specify/templates/plan-template.md
  - ✅ .specify/templates/spec-template.md
  - ✅ .specify/templates/tasks-template.md
- Follow-up TODOs: None
-->

# ProdMill Constitution

## Core Principles

### I. TypeScript First
All code MUST be written in TypeScript to ensure type safety and improve code quality.

### II. Next.js Framework
The project MUST use the Next.js framework for building the React application.

### III. Vitest and React Testing Library
All unit and integration tests MUST be written using Vitest and React Testing Library.

### IV. Minimum 70% Test Coverage
The test suite MUST maintain a minimum of 70% code coverage.

### V. ESLint and Prettier for Code Quality
ESLint and Prettier MUST be used to enforce a consistent code style and identify potential errors.

## Development Workflow

The development workflow should follow Test-Driven Development (TDD) principles where applicable.

## Code Quality Gates

All code must pass ESLint and Prettier checks before being merged.

## Governance

All pull requests must be reviewed and approved by at least one other team member. The constitution can be amended with a pull request and approval from the project maintainers.

**Version**: 1.0.0 | **Ratified**: 2026-01-09 | **Last Amended**: 2026-01-09
