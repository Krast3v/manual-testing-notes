# Topic 01 — SDLC, STLC, Testing Basics

## SDLC vs STLC

**SDLC** (Software Development Life Cycle) — the full process of building software:
```
Requirements → Design → Development → Testing → Deployment → Maintenance
```

**STLC** (Software Testing Life Cycle) — the testing portion only:
```
Analysis → Planning → Test Design → Execution → Reporting → Closure
```

> Testing is a *phase* within SDLC. STLC is how testers organize *their* work inside that phase.

---

## QA vs QC vs Testing

| | What | When | Example |
|---|---|---|---|
| **QA** (Quality Assurance) | Improves the process | Before and during | Code reviews, standards |
| **QC** (Quality Control) | Checks the product | After development | Test execution |
| **Testing** | Finds defects | During QC | Running test cases |

> QA = proactive (prevents defects). QC = reactive (detects defects). Testing is a tool of QC.

---

## Verification vs Validation

- **Verification** = "Are we building it right?" — checking documentation, design, requirements
- **Validation** = "Are we building the right thing?" — checking the final product against user needs

---

## Testing Types

| Type | Definition |
|---|---|
| **Functional** | Does the feature work as specified? |
| **Smoke** | Quick build health check — does the app open at all? (run after every build) |
| **Sanity** | Narrow check after a specific fix — did it work without side effects? |
| **Regression** | Did new code break existing features? |
| **Exploratory** | Unscripted, intuition-based testing without predefined test cases |
| **UAT** | End users confirm the product meets business requirements |

### Smoke vs Sanity
- **Smoke** = check the whole build quickly
- **Sanity** = check one specific thing after a change

---

## Severity vs Priority

**Severity** = how badly something is broken (technical impact)
**Priority** = how urgently it needs to be fixed (business impact)

| Example | Severity | Priority |
|---|---|---|
| Pay button not working | Critical | High |
| Wrong logo color | Low | High (before launch) |
| Crash on rare input combo | High | Low (affects 0.1% of users) |

> Severity and Priority can differ. A wrong logo is low severity but high priority if the launch is tomorrow.

---

## Interview Q&A

**Q: What is the difference between Smoke and Regression testing?**
A: Smoke is a quick check to verify the build is stable before investing in full testing. Regression checks whether new changes broke existing functionality — it runs after every code change.

**Q: Give an example where Severity is Critical but Priority is Low.**
A: A crash that occurs only when a user enters 500+ characters in a text field. Technically critical, but low priority if no real user ever does that.

**Q: What is the difference between QA and QC?**
A: QA (Quality Assurance) is proactive — it focuses on improving the development process to prevent defects. QC (Quality Control) is reactive — it checks the finished product for defects.
