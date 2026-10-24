# Lisa Wright | QA Engineer

**Payments, KYC & Integrations | Web & Mobile Release Testing | API Testing | AI-Assisted Automation**
Greater Boston · [LinkedIn](https://www.linkedin.com/in/lwright-tech) · [GitHub](https://github.com/lwrightqa) · [Website](https://lwright.tech)

- [Summary](#summary)
- [How I Test Today](#how-i-test-today)
- [Work Samples](#work-samples)
- [Experience](#experience)
- [Tools & Skills](#tools--skills)
- [Education & Credentials](#education--credentials)
- [Upskilling Resources](#upskilling-resources)

## Summary
QA engineer at a B2B iGaming platform, testing regulated flows where defects have financial and compliance consequences: sign-up and identity verification (KYC), deposits and withdrawals, and third-party provider integrations. I test release candidates across desktop web, mobile web, iOS and Android, for white-label apps in English and Spanish.

Before QA I spent over a decade in technical support and release management, so I write bug reports that developers can act on and test plans that support teams can read. I'm strongest at API testing, test design for failure paths and edge cases, and cross-team communication. I use AI tools to test faster (agent-driven end-to-end runs on real devices, LLM help turning Jira tickets into test cases) and I check their output rather than trust it.

## How I Test Today
What a typical feature looks like on my desk, from ticket to sign-off:

1. **Before it's built:** read the ticket for testability. Missing acceptance criteria, unexplained feature flags or undocumented endpoints go back to refinement as questions, not surprises later.
2. **Test design:** named techniques, not guesswork: boundary values, state transitions for payment lifecycles (pending → approved → settled, or declined and retried), decision tables for KYC outcomes, and pairwise combinations for provider × currency × platform.
3. **Below the UI:** Postman for request and response bodies, webhook delivery and retries; network captures and logs to confirm what the app sent and what the backend did.
4. **Automation where it pays:** Playwright for multi-step web flows, Maestro on real Android devices, small Python scripts for smoke checks, and AI agents for exploratory runs.
5. **Release candidates:** a risk-ranked smoke checklist per release, run across web and mobile, with evidence attached to each result.

## Work Samples

### From my current role (private code, described here)
The code and data belong to my employer, so these are described rather than linked.
- **Web flow automation (Playwright, TypeScript):** multi-step registration and verification flows.
- **Mobile regression flows (Maestro):** account and login flows for white-label apps in English and Spanish, run on a real Android device.
- **Payment smoke scripts (Python):** quick deposit and withdrawal checks to confirm a provider is healthy before deeper testing.
- **Test plans and release-candidate checklists:** per-ticket plans and risk-ranked smoke checklists covering verification and payment flows.

### Public projects

#### [Clawd Tank widescreen](https://github.com/lwrightqa/clawd-tank-widescreen): embedded firmware + desktop app (C, Python)
A fork of an open-source desk display that shows Claude Code session status, ported to a different ESP32-S3 board and a 640 × 172 screen. Adds a Windows tray app, a macOS flyout and a CI workflow that runs the host tests and renders UI snapshots on GitHub's Mac runner. The README separates what was tested on real hardware from what was not.

#### [Urban Routes](https://github.com/lwrightqa/Urban-Routes): UI automation (Python, Selenium, PyTest)
Page Object Model suite for a ride-ordering flow, handling dynamic elements and asynchronous behavior.
- **Best place to start:** [`test_fill_phone_number`](https://github.com/lwrightqa/Urban-Routes/blob/main/tests/test_urban_routes.py), which tests phone verification end to end. It enters a number, reads the SMS confirmation code the app generates from Chrome's performance logs (using a course-provided helper), enters it, and asserts the field values at each step. The page object is in [`urban_routes.py`](https://github.com/lwrightqa/Urban-Routes/blob/main/urban_routes.py).
- Also covers route entry, plan selection, card details, driver comments, extras and the final order.
- Note: the target app was a temporary training environment and is no longer online, so the tests can't be run today.
#### [Urban Scooter](https://github.com/lwrightqa/Urban-Scooter): manual, mobile and API testing
Test cases for a scooter delivery app's mobile app, web app and backend API: functional, negative, UI-vs-design and connectivity testing; boundary value analysis and equivalence partitioning; Postman checks for status codes and payloads.

#### [Coin Collector](https://github.com/lwrightqa/Coin-Collector): unit testing (Python, pytest)
A small Pygame Zero game extended with a timer and WASD controls, plus a pytest suite for the game logic.

#### [Garage Manager](https://github.com/lwrightqa/Garage-Manager): command-line Python app with unit tests

## Experience

### Manual Software QA Specialist, B2B iGaming platform
*Jan 2026 – Present · Boston, MA (hybrid)*
QA for the integrations domain (authentication, identity verification and payments) across desktop web, mobile web, iOS and Android.
- Test third-party payment and identity verification integrations, including Postman API checks for response behavior, webhook delivery and retries.
- Test new payment provider integrations end to end: card and wallet deposits, withdrawals, saved cards and failure paths across multiple currencies and regions.
- Run release-candidate smoke testing for white-label web and mobile apps in English and Spanish.
- Verify backend behavior that has no UI through network captures and logs, attaching the evidence to Jira.
- Automate repetitive setup and regression, and use AI agents for end-to-end runs on real mobile devices.
- Review tickets for testability before they reach QA, raising missing acceptance criteria, flag values and API details in refinement.
- Go-to resource for the integrations domain on authentication, KYC and payment provider behavior.

### Professional Upskilling & Independent QA Projects
*Jan 2024 – Jan 2026 · Remote*
- Completed a QA Engineering program covering Agile/Scrum and manual and automated testing.
- Built Python and Selenium test suites, wrote Postman API tests, and authored test plans, test cases and bug reports in Jira.

### QA & Release Manager, Thought Industries
*Jan 2020 – Oct 2023*
- Cut the bug and feature-request backlog by 40% and sped up time-to-market by running biweekly releases with regression and functional test strategies.
- Improved SLA adherence by writing test plans and feature guides for each release in Jira and Google Workspace.
- Subject matter expert for the LMS: diagnosed critical defects and trained colleagues on the platform.

### Earlier: technical and product support, 2011 – 2019
Technical and Product Support Specialist at Thought Industries (CSAT above 80%, support response time cut from 3 days to 1, ticket volume down 15% after a Zendesk knowledge base migration); Support Genius at LevelUp; Product Support Specialist at MeYou Health (built the first support system and trained new staff); Support Specialist at HubSpot (300+ tickets a month, spotting recurring patterns that pointed to product defects).

## Tools & Skills

| | |
|---|---|
| **Testing** | Manual, exploratory, regression, integration, API, release-candidate smoke testing, localization, test planning, bug reporting |
| **Test design** | Boundary values, equivalence partitioning, state transitions, decision tables, pairwise combinations |
| **Automation** | Playwright, Maestro, Python, Selenium, PyTest, Page Object Model |
| **AI-assisted testing** | Claude Code, agent-driven end-to-end testing, LLM test case generation |
| **API & network** | Postman, webhooks, Chrome DevTools, HAR analysis, SQL |
| **Tools** | Jira, Confluence, TestRail, Git and GitHub, Android Studio |
| **Domain** | Payments, KYC / identity verification, third-party integrations |

## Education & Credentials
**Certificate in Quality Assurance Engineering**, [TripleTen](https://tripleten.com), completed 07/2025
Agile, API testing, automation testing, bug reports, Chrome DevTools, Jira, manual testing, Postman, Python, regression testing, Selenium, SQL, test cases, web application testing

**Bachelor of Arts, Communications**, [Curry College](https://www.curry.edu/), Milton, MA. Graduated cum laude.

## Upskilling Resources
<details>
<summary>Books, blogs and communities I learn from</summary>

**Books**
- *Explore It! Reduce Risk and Increase Confidence with Exploratory Testing*, Elisabeth Hendrickson
- *Software Testing: An ISTQB-BCS Certified Tester Foundation Level guide (CTFL v4.0)*, 5th edition, Geoff Thompson et al.
- *Dear Evil Tester*, Alan Richardson

**Blogs**
- [EvilTester.com](https://www.eviltester.com/)
- [QA Blog by Mindful QA](https://www.mindfulqa.com/blog/)
- [Software Testing Weekly](https://softwaretestingweekly.com/)

**Communities**
- [Ministry of Testing](https://www.ministryoftesting.com/)
- [QA & Testing Group](https://www.linkedin.com/groups/95831/)

</details>

*Last updated: October 2026*
