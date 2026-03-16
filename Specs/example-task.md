# SPEC-001: Example Task

## Overview
This is an example specification for a task to be performed during the Night Shift.

## Requirements
1.  Verify that the `Specs/` and `Docs/` directories exist and contain a `.gitkeep` file (optional, but good for git tracking if empty).
2.  Add a simple utility function in `src/utils.ts` that capitalizes a string, if it doesn't already exist.
3.  Add a test for this utility in `tests/utils.test.ts`.

## Acceptance Criteria
-   `capitalize("hello")` returns `"Hello"`.
-   `capitalize("World")` returns `"World"`.
-   `capitalize("")` returns `""`.
-   All tests pass.
-   Code is formatted and type-checked.
