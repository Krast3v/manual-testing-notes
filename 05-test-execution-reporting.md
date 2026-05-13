# Topic 05 — Test Execution & Reporting

## Test Execution Process

```
Test Plan → Test Cases → Execute → Log Results → Report
```

Each test case result is one of three:
- **Pass** — behavior matches Expected Result
- **Fail** — behavior does not match → log bug
- **Blocked** — test cannot be executed (environment down, dependency missing)

> Blocked is NOT Fail. The test didn't run — it couldn't run.

---

## Test Metrics

| Metric | Meaning |
|---|---|
| **Test Coverage** | % of requirements covered by tests |
| **Pass Rate** | Passed / Total executed × 100 |
| **Defect Density** | Number of bugs / size of functionality |
| **Blocked Tests** | Tests that could not be executed |

> You can have 100% Pass Rate but low Coverage — tested everything you wrote, but missed large parts of the app.

---

## Test Summary Report

| Section | Content |
|---|---|
| **Summary** | Overall status — pass/fail/blocked |
| **Scope** | What was tested |
| **Test Results** | Count of passed, failed, blocked |
| **Defects Found** | Bug list with statuses |
| **Risks** | What was NOT tested and why |
| **Recommendation** | Go / No-Go for release |

---

## Go / No-Go Decision

- **Go** — Exit criteria met, product is ready for release
- **No-Go** — Open Critical/High bugs or insufficient coverage

> QA does not make the final decision — but provides the information for it.

---

## Interview Q&A

**Q: What does "Blocked" mean in test execution?**
A: A test is Blocked when it cannot be executed — not because it failed, but because a precondition is missing. For example, the environment is down or a dependency hasn't been deployed.

**Q: What is a Test Summary Report?**
A: A document at the end of a test cycle summarizing what was tested, results (passed/failed/blocked), defects found, and a Go/No-Go recommendation for release.

**Q: What is the difference between Pass Rate and Test Coverage?**
A: Pass Rate measures how many executed tests passed. Test Coverage measures how much of the requirements are covered by tests at all. You can have 100% pass rate but low coverage — meaning you tested everything you wrote, but missed large parts of the application.
