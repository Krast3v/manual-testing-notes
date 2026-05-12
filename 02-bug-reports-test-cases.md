# Topic 02 — Bug Reports & Test Cases

## Bug Report — Required Fields

| Field | Purpose | Example |
|---|---|---|
| **ID** | Unique identifier | BUG-042 |
| **Title** | Short, clear summary | "Login button unresponsive on mobile Safari" |
| **Environment** | Where it was found | iOS 16, Safari 15, staging |
| **Steps to Reproduce** | Exact sequence to trigger | 1. Open app. 2. Enter credentials. 3. Tap Login. |
| **Expected Result** | What should happen | User is redirected to dashboard |
| **Actual Result** | What actually happens | Nothing happens, button doesn't respond |
| **Severity** | Technical impact | High |
| **Priority** | Business urgency | Critical (launch in 2 days) |
| **Attachments** | Screenshot, video, logs | screenshot.png |

> A good bug report lets a developer reproduce the issue without asking you a single question.

---

## Bug Report — Example

**Title:** Cart total not updated after removing item

**Environment:** Chrome 120, Windows 11, production

**Steps to Reproduce:**
1. Add 2 items to cart
2. Go to cart page
3. Remove one item using the "×" button

**Expected Result:** Cart total updates immediately to reflect remaining item

**Actual Result:** Total stays the same; page refresh required to see correct total

**Severity:** Medium — wrong data shown, no crash

**Priority:** High — affects checkout flow

---

## Test Case — Required Fields

| Field | Purpose |
|---|---|
| **ID** | Unique reference (TC-001) |
| **Title** | What is being tested |
| **Preconditions** | What must be true before the test |
| **Steps** | Numbered actions |
| **Expected Result** | What success looks like |
| **Test Data** | Inputs used |
| **Pass/Fail** | Result after execution |

---

## Test Case — Example

**ID:** TC-007
**Title:** Successful login with valid credentials

**Preconditions:** User account exists. App is on login page.

**Steps:**
1. Enter username: `tomsmith`
2. Enter password: `SuperSecretPassword!`
3. Click "Login" button

**Expected Result:** User is redirected to `/secure`. Flash message: "You logged into a secure area!"

**Test Data:** username=tomsmith, password=SuperSecretPassword!

---

## Test Case Types

| Type | Definition | Example |
|---|---|---|
| **Positive** | Valid input, expect success | Login with correct credentials |
| **Negative** | Invalid input, expect rejection | Login with wrong password |
| **Boundary** | Values at the edge of limits | Max 255 chars in username field |
| **Edge Case** | Unusual but valid scenarios | Username with special characters: `user@name` |

> Always write negative and boundary tests — that's where bugs hide.

---

## Interview Q&A

**Q: What makes a good bug report?**
A: A good bug report has a clear title, exact steps to reproduce, expected vs actual result, environment details, and severity/priority. The goal is that a developer can reproduce the issue without asking you anything.

**Q: What is the difference between a positive and a negative test case?**
A: A positive test verifies that the system works correctly with valid input. A negative test verifies that the system handles invalid input correctly — for example, showing an error message instead of crashing.

**Q: Why do we test boundary values?**
A: Because boundary conditions are where developers most commonly make off-by-one errors. Testing exactly at, just below, and just above the limit catches bugs that random inputs would miss.
