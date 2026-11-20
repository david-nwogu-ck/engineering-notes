# David Nwogu

[CITY, STATE] | [EMAIL] | [PHONE] | [LINKEDIN URL] | [GITHUB URL]

## SUMMARY

Software engineer on Credit Karma's web platform team (an Intuit company), building the Next.js and React framework, CI guardrails, release pipeline and observability that 30+ product web apps run on. [YEARS OF EXPERIENCE] years of experience building web applications and platforms. Owns initiatives from design through staged rollout, and turns recurring problems into automated checks, shared tooling and documentation.

## TECHNICAL SKILLS

- **Languages:** TypeScript, JavaScript, GraphQL
- **Frameworks and Libraries:** React, Next.js (App Router), React Server Components
- **Testing:** Jest, Cypress, Vitest, Appium
- **Build, CI/CD and Observability:** ESLint (custom plugin authoring), esbuild, Nx, CircleCI, New Relic, Splunk, sourcemaps
- **Practices:** technical design docs, ADRs, staged rollouts with feature flags and experiments, release management, on-call, code review, AI coding agents, MCP servers

## PROFESSIONAL EXPERIENCE

**Credit Karma, an Intuit company** | [CITY, STATE]
**Software Engineer II, Web Platform (Frontend Framework)** | [START DATE MM/YYYY] – Present

*Client-side code delivery platform*

- Authored the three-phase execution plan and a leadership overview for a platform that ships framework code to 50+ web apps without per-app deploys, co-owned with two engineers. Each app deploys on its own schedule, so fixes stall: one fleet-wide onboarding took 69 days and an emergency security fix took 8 days across 50 apps.
- Specified the platform's guarantees (version-tagged events, sourcemaps, error attribution, integrity hashing, bundle-size budgets, non-blocking two-stage loading, hash-based caching) and designed the per-script ramp model: one experiment flag per script, retired once its ramp settles. Own the rollback-gating design.
- Delivered the first guarantees: telemetry tagged with the release version and sourcemaps published to New Relic (validated on three apps), so errors from CDN-delivered code show their version and readable stack traces.
- Built a per-PR bundle-size check in shared tooling and rewrote the first-stage inline scripts as typed, tested TypeScript compiled with esbuild, moving the analytics tracker and image-error queue onto the two-stage load. Found that every release changed every script URL and recorded the fix, content-hashed assets, in an ADR.
- Moved the analytics tracker onto the platform behind its own experiment flag and shipped its release with a New Relic dashboard. Wrote the fix (in review) for a front-end gateway gap blocking its production ramp for embedded mobile web views and cookieless native requests.

*Framework guardrails and developer experience*

- Unblocked React Server Component adoption by adding a security-team global-state scanner to framework CI as a blocking check, contributing to that team's repo to support frontend code. Raised framework packages passing from ~60% to 100% and fixed 45+ files so 30+ apps start clean; [METRIC?: apps now using React Server Components].
- Built a custom ESLint plugin (three rules, rule generator) that ships to 30+ Next.js apps with zero setup, and typed test utilities that cut unit-test setup from 50+ lines to one call.
- Authored 12 framework guides in three months from recurring chat and code-review questions, using an AI-assisted template. Partnered with the developer-productivity team so the guides feed an MCP server for AI coding agents; reduction in repeat support questions: [METRIC?].

*Observability and reliability*

- Took image-error reporting from design to production: wrote the design doc, took over a pull request that had stalled for five months, co-authored roughly half of its final code and tests, merged it, and co-owned the first production ramp (1% to 100%). Later rewrote the event queue in TypeScript, generating its inline script from the typed source.
- Diagnosed a spike in embedded-web-app abandonment with lifecycle logging in New Relic, finding that several apps never reported end-of-load timing and created false abandonment events. Fixed a blocking iOS bug in another team's Appium framework.

*Cross-team rollouts and release ownership*

- Rolled out framework performance reporting to 9 production apps in four weeks and upgraded 8 apps owned by other teams to a new major framework version, one app per pull request to limit blast radius.
- Shipped the Android navigation-transition system for embedded web apps after joining another team's initiative, bringing Android to parity with iOS for millions of users.
- Ran seven staged production releases (ramp plans, approvals, monitoring), including a navigation release ramped 0% to 100% with no aborts or rollbacks and a same-day release to unblock a teammate. Reviewed 250+ pull requests and served on call.

## EDUCATION

[EDUCATION: degree, major, school, year]

## EARLIER EXPERIENCE

[EARLIER EXPERIENCE: prior roles, companies, dates, or delete this section]
