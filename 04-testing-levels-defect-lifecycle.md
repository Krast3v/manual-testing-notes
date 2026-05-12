# Topic 04 — Testing Levels & Defect Life Cycle

## Testing Levels

| Level | What is tested | Who tests |
|---|---|---|
| **Unit** | Individual function / method | Developer |
| **Integration** | Communication between modules | Developer / QA |
| **System** | Full application end-to-end | QA |
| **UAT** | Meets real user/business needs | Client / End user |

> Each level catches a different type of problem. Unit tests details, UAT tests reality.

---

## Defect Life Cycle

```
New → Assigned → Open → Fixed → Retest → Closed
                                    ↓
                                 Reopen (if bug not fixed)
```

| Status | Meaning |
|---|---|
| **New** | Bug found and logged |
| **Assigned** | Given to a developer |
| **Open** | Developer is working on it |
| **Fixed** | Developer says "done" |
| **Retest** | QA verifies the fix |
| **Closed** | QA confirms — bug is resolved |
| **Reopen** | QA finds it's still broken |

---

## Interview Q&A

**Q: What are the four levels of testing?**
A: Unit — tests individual functions, done by developers. Integration — tests how modules work together. System — tests the full application end-to-end. UAT — end users confirm the product meets business requirements.

**Q: What happens when a bug is marked "Fixed"?**
A: The QA engineer retests it. If the fix works — the bug is Closed. If the issue persists — the bug is Reopened and goes back to the developer.

**Q: Why is UAT important if we already did System testing?**
A: System testing checks technical correctness. UAT checks real-world usability — whether the product actually solves the user's problem. A system can pass all tests and still fail UAT.
