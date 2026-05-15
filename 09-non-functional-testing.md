# Topic 09 — Non-Functional Testing

## Functional vs Non-Functional

| | Functional | Non-Functional |
|---|---|---|
| **Question** | Does it work? | Does it work *well*? |
| **Example** | Does login work? | Is login fast under 10,000 users? |

---

## Types of Non-Functional Testing

| Type | What it tests | Example |
|---|---|---|
| **Performance** | Speed and response time | Page loads in < 2 seconds |
| **Load** | Behavior under expected traffic | 1000 concurrent users |
| **Stress** | Behavior under extreme traffic | 10,000 users — when does it break? |
| **Security** | Vulnerabilities and protection | SQL injection, XSS |
| **Usability** | Ease of use | User finds the button intuitively |
| **Compatibility** | Works across devices/browsers | Chrome, Safari, Firefox, iOS, Android |
| **Reliability** | Stability over long usage | Runs 72 hours without crash |

---

## Performance Testing — Key Terms

- **Response Time** — how fast the system responds to a request
- **Throughput** — number of requests per second
- **Bottleneck** — the slowest part of the system
- **Spike Testing** — sudden traffic surge (Black Friday)

---

## Interview Q&A

**Q: What is the difference between Load and Stress testing?**
A: Load testing checks behavior under expected traffic — for example, 1000 concurrent users. Stress testing pushes beyond the limit to find the breaking point — when does the system crash or degrade?

**Q: Give an example of a non-functional bug.**
A: The login page works correctly but takes 8 seconds to load. Functionally it passes — the user can log in. Non-functionally it fails — the response time is unacceptable.

**Q: Why is Compatibility testing important?**
A: Because users access the application from different browsers, operating systems, and devices. A feature that works perfectly on Chrome may break on Safari or on a mobile screen.
