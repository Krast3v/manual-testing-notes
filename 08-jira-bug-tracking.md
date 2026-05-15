# Topic 08 — Jira Basics & Bug Tracking

## What is Jira

Jira is a tool for tracking tasks and bugs. Almost every IT company in Bulgaria uses it. QA works in it every day.

---

## Ticket Types

| Type | Description |
|---|---|
| **Epic** | Large feature (Login system) |
| **Story** | User Story — specific user need |
| **Task** | Technical task without direct user value |
| **Bug** | Defect in the application |
| **Sub-task** | Small step toward a Story or Task |

---

## Bug Ticket in Jira — Fields

- **Summary** — short title
- **Description** — Steps to Reproduce, Expected Result, Actual Result
- **Priority** — Blocker / Critical / Major / Minor / Trivial
- **Status** — Open / In Progress / Fixed / Closed (NOT the same as Priority)
- **Assignee** — who it's assigned to
- **Reporter** — who found the bug
- **Fix Version** — which release it should be fixed in
- **Labels / Components** — for filtering

---

## Ticket Workflow

```
To Do → In Progress → In Review → Done
```

Bug lifecycle:
```
Open → Assigned → In Progress → Fixed → Retest → Closed / Reopen
```

---

## Useful Jira Features for QA

- **Filters** — find all open Critical bugs in current sprint
- **Dashboards** — sprint status overview
- **Linking tickets** — connect a bug to the Story it belongs to
- **Comments** — communicate with the developer directly in the ticket

---

## Interview Q&A

**Q: Have you worked with Jira?**
A: Not in a commercial project yet, but I understand the workflow — creating bug tickets with all required fields, tracking defect status through its lifecycle, and linking bugs to the relevant user stories.

**Q: What information do you include when logging a bug in Jira?**
A: Summary, steps to reproduce, expected vs actual result, environment, priority, and attachments like screenshots or recordings.

**Q: What is the difference between Priority: Blocker and Priority: Critical?**
A: Blocker means the entire process cannot continue until it's fixed. Critical means severe impact on functionality, but work can proceed on other areas in the meantime.
