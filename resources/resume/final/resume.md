# David Nwogu

[CITY, STATE] | [EMAIL] | [PHONE] | [LINKEDIN URL] | [GITHUB URL]

## SUMMARY

Frontend platform engineer on Credit Karma's Next.js and React framework team (an Intuit company), building the guardrails, tooling, observability and delivery systems that 50+ web apps depend on. [YEARS OF EXPERIENCE] years of experience building web applications and platforms. Owns initiatives from design through staged rollout, and turns recurring problems into automated checks, shared tooling and documentation.

## TECHNICAL SKILLS

- **Languages:** TypeScript, JavaScript, GraphQL
- **Frameworks and Libraries:** React, Next.js (App Router), React Server Components
- **Testing:** Jest, Cypress, Appium
- **Build, CI/CD and Observability:** ESLint (custom plugin authoring), esbuild, Nx, CircleCI, New Relic, Splunk, sourcemaps
- **Practices:** technical design docs, ADRs, staged rollouts with feature flags and experiments, release management, on-call, code review, AI coding agents, MCP servers

## PROFESSIONAL EXPERIENCE

**Credit Karma, an Intuit company** | [CITY, STATE]
**Software Engineer II, Web Platform (Frontend Framework)** | [START DATE MM/YYYY] – Present

*Client-side code delivery platform*

- Authored the execution design (18 tickets, three phases, about 9–11 engineer-weeks) and, with two co-owners, the leadership overview for a platform that delivers framework code to 50+ web apps without per-app deploys. Apps deploy on their own schedules, so an emergency security fix took 8 days across 50 apps, onboarding the fleet onto shared packages took 69, and one app ran an old framework version after its fix existed.
- Specified the guarantees the platform adds (version-tagged events, sourcemaps, error attribution, integrity hashing, bundle-size budgets, non-blocking two-stage loading, hash-based caching) and designed per-script ramps and rollback gating: one experiment flag per script, retired once its ramp settles.
- Moved the analytics tracker onto the platform as its first migrated script and shipped the release with a ramp plan and New Relic dashboard. Fixed a front-end gateway gap that blocked the tracker's production ramp for embedded mobile web views and cookieless native requests.
- Made CDN-delivered code debuggable with release-tagged telemetry and sourcemaps in New Relic (validated on three apps), so errors show their version and readable stack traces. Added a per-PR bundle-size check in shared tooling that other packages can adopt.
- Rewrote first-stage inline scripts into typed, tested TypeScript compiled with esbuild, moving the tracker and image-error queue onto the two-stage load. Found that every release changed every script URL, recorded the decision in an ADR, and shipped content-hashed assets so client caches stay valid.

*Framework guardrails and developer experience*

- Added a security-team global-state scanner to framework CI as a blocking check, taking framework packages from about 60% to 100% passing after fixing 45+ files. Contributed to that team's scanner, unblocking React Server Components adoption across the org; [METRIC?: apps now using React Server Components].
- Built a custom ESLint plugin (three rules, applied through shared config) that moves framework-pattern checks into the IDE for 30+ Next.js apps, and cut unit-test setup from 50+ lines to one call with typed mocks that fail at compile time.
- Wrote 12 framework guides in three months using an AI-built template. Partnered with the developer-productivity team to feed the guides to an MCP server for AI coding agents; [METRIC?: reduction in repeat support questions].

*Observability and reliability*

- Wrote the design for image-error reporting (CDN and failure type), took over a pull request stalled for five months, wrote about half of its final code and tests, merged it, and co-owned the first production release and its 1% to 100% ramp (50 minutes). Later rewrote the event queue in TypeScript.
- Diagnosed a spike in embedded-web-app abandonment with lifecycle logging in New Relic, finding apps that never reported end-of-load timing and created false abandonment events.

*Cross-team rollouts and release ownership*

- Ran seven staged production releases of shared frontend packages, including a navigation package ramped from 0% to 100% in 72 minutes with no aborts or rollbacks and a same-day release to unblock a teammate. Covered on-call weeks and reviewed 250+ pull requests.
- Rolled out framework performance reporting to 9 production apps in four weeks and upgraded 8 apps owned by other teams to a new major framework version, one pull request per app to limit blast radius.
- Shipped Android navigation transitions for embedded web apps after another team pulled me in, matching iOS for millions of users. Fixed an iOS bug blocking another team's Appium automation for every team using it.

## EDUCATION

[EDUCATION: degree, major, school, year]

## EARLIER EXPERIENCE

[EARLIER EXPERIENCE: prior roles, companies, dates, or delete this section]
