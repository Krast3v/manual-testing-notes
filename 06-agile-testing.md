# Topic 06 — Agile & Testing in Agile

## Waterfall vs Agile

| | Waterfall | Agile |
|---|---|---|
| **Structure** | Linear — each phase completes before the next | Iterative — small cycles (sprints) |
| **Testing** | Only after development | Parallel with development |
| **Changes** | Difficult and costly | Expected and welcome |
| **Delivery** | One big release at the end | Small deliverables each sprint |

---

## Agile Basics

**Sprint** — fixed period (usually 2 weeks) in which the team builds and tests a set of features.

**User Story** — description of a feature from the user's perspective:
> *"As a user, I want to reset my password so that I can regain access to my account."*

**Acceptance Criteria** — the specific conditions under which a User Story is considered done. QA writes test cases directly from them. Each criterion = at least one test case.

---

## QA Role in Agile

- Involved from the start of the sprint, not waiting for the end
- Tests in parallel with development
- Gives early feedback — bugs are cheaper to fix the earlier they are found
- Participates in **Sprint Review** and **Retrospective**

---

## Regression in Agile

Every sprint adds new code → regression testing after each sprint is mandatory. This is why automation is valuable — manual regression on a large application is slow.

---

## Interview Q&A

**Q: What is the difference between Waterfall and Agile testing?**
A: In Waterfall, testing happens only after development is complete. In Agile, testing is continuous — QA works in parallel with developers within each sprint, catching issues early.

**Q: What are Acceptance Criteria and how do you use them?**
A: Acceptance Criteria define the specific conditions under which a User Story is considered done. As a QA, I use them directly to write test cases — each criterion becomes at least one test.

**Q: Why is regression testing especially important in Agile?**
A: Because new code is added every sprint. Without regression testing after each sprint, existing functionality can break without anyone noticing until much later.
