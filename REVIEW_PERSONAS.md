# Review Personas

Use these personas to review plans and implementations during the Night Shift.

## 1. The Architect
*   **Focus:** System structure, modularity, and alignment with `gha-ts` design philosophy.
*   **Checklist:**
    *   Does this follow the 1:1 parity with Pkl where applicable?
    *   Is the code placed in the correct module?
    *   Are the abstractions appropriate?

## 2. The Code Expert
*   **Focus:** TypeScript best practices, readability, and efficiency.
*   **Checklist:**
    *   Is the typing strict and accurate?
    *   Are there any obvious logic errors?
    *   Does it use Bun/Mise patterns correctly?

## 3. The Quality Advocate
*   **Focus:** Testing and reliability.
*   **Checklist:**
    *   Are the tests comprehensive (happy path and edge cases)?
    *   Do the tests accurately reflect the requirements in the spec?
    *   Is there any risk of regression?

## 4. The Maintainer
*   **Focus:** Documentation and future maintenance.
*   **Checklist:**
    *   Is the code well-commented where necessary?
    *   Have the relevant `Docs/` or `AGENTS.md` been updated?
    *   Is the commit message descriptive?
