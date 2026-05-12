# Topic 03 — Test Plan & Test Strategy

## Test Plan vs Test Strategy

| | Test Plan | Test Strategy |
|---|---|---|
| **What** | Document for a specific project | Document for the entire organization |
| **Scope** | One release / feature | All projects |
| **Who writes it** | Test Lead / QA Lead | QA Manager |
| **Contains** | Scope, schedule, resources, risks | Approaches, standards, tools |

> Test Strategy = "How we test as a company." Test Plan = "How we test THIS feature."

---

## Test Plan — Required Sections

| Section | Content |
|---|---|
| **Scope** | What is tested and what is NOT tested |
| **Test Objectives** | What we want to verify |
| **Test Approach** | Manual, automated, or combination |
| **Resources** | People, tools, environments |
| **Schedule** | Start and end dates |
| **Entry/Exit Criteria** | When to start / when to stop |
| **Risks** | What could go wrong |

---

## Entry vs Exit Criteria

**Entry Criteria** — conditions to *start* testing:
- Build is stable
- Test environment is ready
- Requirements are finalized

**Exit Criteria** — conditions to *stop* testing:
- 95%+ test cases executed
- No open Critical or High bugs
- Deadline reached

> Exit criteria answer: "When can we say — done?"

---

## In Scope vs Out of Scope

Not everything is tested in a given cycle.

**Example:**
- **In scope:** Login, cart, checkout
- **Out of scope:** Admin panel, reporting module (next sprint)

> Clear scope prevents endless testing and manages expectations.

---

## Interview Q&A

**Q: What is the difference between a Test Plan and a Test Strategy?**
A: A Test Strategy is a high-level document defining how the entire organization approaches testing — tools, standards, methodologies. A Test Plan is project-specific — scope, schedule, resources, and risks for one release or feature.

**Q: What are Entry and Exit Criteria?**
A: Entry criteria define when testing can begin — build is stable, environment is ready. Exit criteria define when testing is complete — 95%+ test cases passed, no open Critical or High bugs.

**Q: Why is it important to define what is Out of Scope?**
A: Without a defined scope, testing can go on indefinitely. Out of scope sets clear boundaries — what is tested now and what is deferred — managing time and expectations.
