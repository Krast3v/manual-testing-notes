# Topic 07 — Test Techniques

## Black Box vs White Box vs Grey Box

| | Black Box | White Box | Grey Box |
|---|---|---|---|
| **Code access** | No | Yes | Partial |
| **Who tests** | QA | Developer | QA + Dev |
| **Focus** | Behavior / output | Logic / code | Combination |
| **Example** | Testing login form without seeing code | Testing every if/else branch | Know API structure, test behavior |

---

## Equivalence Partitioning

Divide inputs into groups the system treats the same way. Test one value from each group — no need to test every possible input.

**Example — age field (1-120):**
- Invalid below limit: -1, 0
- Valid: 1-120 → test with 50
- Invalid above limit: 121, 999

3 tests instead of 120.

---

## Boundary Value Analysis

Test at the edges — that's where off-by-one errors happen most often.

**Example — field accepts 1 to 100:**

| Value | Type |
|---|---|
| 0 | Below lower boundary |
| 1 | Lower boundary |
| 2 | Just above lower boundary |
| 99 | Just below upper boundary |
| 100 | Upper boundary |
| 101 | Above upper boundary |

> Off-by-one error: developer writes `< 100` instead of `<= 100` — system blocks at 99 instead of 100.

---

## Decision Table Testing

Used when behavior depends on a combination of conditions.

**Example — discount logic:**

| Member | Purchase > 100 BGN | Result |
|---|---|---|
| Yes | Yes | 20% discount |
| Yes | No | 10% discount |
| No | Yes | 5% discount |
| No | No | No discount |

---

## Interview Q&A

**Q: What is the difference between Black Box and White Box testing?**
A: Black Box testing focuses on behavior — the tester doesn't see the code, only inputs and outputs. White Box testing examines internal logic — the tester has access to the code and tests specific paths and conditions.

**Q: What is Equivalence Partitioning?**
A: A technique where we divide inputs into groups the system treats the same way, and test one value from each group. It reduces the number of test cases while maintaining coverage.

**Q: Why do we test boundary values specifically?**
A: Because off-by-one errors at boundaries are among the most common developer mistakes — writing `< 100` instead of `<= 100`. Testing at, just below, and just above the limit catches these bugs.
