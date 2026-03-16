# Night Shift Agent Loop

This document defines the autonomous loop to be followed when running in "Night Shift" mode.

## Objective
Work autonomously to implement features and fix bugs specified in the `Specs/` directory while maintaining high code quality and system integrity.

## The Loop

1.  **Preparation**
    *   Clean the working tree: Analyze uncommitted work. Stash or commit as appropriate.
    *   Run the full test suite (`mise run test`).
    *   If any tests fail, fix them before proceeding.

2.  **Task Selection**
    *   Prioritize bug fixes (if any are tracked).
    *   Select a feature spec from `Specs/`. Ignore files named `draft-*`.

3.  **Analysis**
    *   Read and analyze the selected spec.
    *   Load relevant documentation from `Docs/` and `AGENTS.md`.
    *   Explore relevant source code in `src/`.

4.  **Testing Plan**
    *   Develop a comprehensive testing plan.
    *   Write extensive tests for the feature/fix.
    *   Run the tests and verify they fail as expected.

5.  **Planning & Review**
    *   Develop a detailed implementation plan.
    *   Simulate/Run review agents based on `REVIEW_PERSONAS.md`.
    *   Refine the plan based on feedback until all "personas" give a green light.

6.  **Implementation**
    *   Implement the changes according to the plan.
    *   Update documentation in `Docs/` if necessary.

7.  **Verification**
    *   Run type checking (`mise run typecheck`).
    *   Run linting/formatting (`mise run format`).
    *   Run relevant tests and iterate until they pass.
    *   Run the *entire* test suite to ensure no regressions.

8.  **Final Review**
    *   Perform a self-review of the implementation diff.
    *   Optionally run review personas again on the final diff.

9.  **Wrap-up**
    *   Record unrelated TODOs noticed during the process in a `TODO.md` (if it exists) or a new doc.
    *   Update `CHANGELOG.md` (if applicable).
    *   Commit changes with a detailed commit message.

10. **Iterate**
    *   Loop back to Step 2 if there are more tasks and time/budget allows.

11. **Final Report**
    *   Once all tasks are complete or the session is ending, write a concise summary of the work accomplished for the human "Day Shift" to review.
