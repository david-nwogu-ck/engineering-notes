# David Nwogu

**Software Engineer · Frontend & Web Platform (React, Next.js, TypeScript)**
[EMAIL] · [PHONE] · [LOCATION] · [LINKEDIN / GITHUB]

> DRAFT: resolve every `[BRACKET]` and `[METRIC?]` before submitting (see `notes.md`).

## Summary

Frontend platform engineer on Credit Karma's internal Next.js/React framework, building the guardrails, tooling, observability and delivery systems that 50+ web apps depend on. Authored the technical design and leadership overview for shipping framework code to those apps without each one redeploying.

## Experience

**Software Engineer II, Web Platform (frontend framework) team**: Credit Karma, an Intuit company
[START DATE] – Present · [LOCATION]

**Client-code delivery: framework code without app redeploys**

- Wrote the execution design (18 tickets, three phases, about 9–11 engineer-weeks) and, with two co-owners, the leadership overview for a team initiative to deliver client-side framework code to 50+ apps without per-app redeploys. The problem: an emergency security fix took 8 days across 50 apps, onboarding the fleet onto shared packages took 69, and one app ran an old framework version after its fix existed.
- Moved the behavioral-event tracker onto the pipeline as its first migrated script. Designed the ramp model (one experiment per script, old flag removed once the ramp settles), tested it with segment overrides, and shipped the release with a ramp plan and dashboard; its production ramp awaits review of a gateway fix I wrote. Own the open design for per-script rollback gating.
- Made CDN-delivered code debuggable: version-tagged telemetry and sourcemaps in New Relic, tested on three frontends, so errors show their version and readable stack traces. Added a CI bundle-size check on every PR in shared tooling that other packages can adopt.
- Rewrote first-stage inline scripts from hand-written strings into typed, tested TypeScript, and moved the tracker onto them. Found that every release changed every script URL and wrote the decision record for hash-based caching (implementation in review).

**Guardrails and developer experience**

- Led integration of a global-state static analyzer into framework CI as a blocking check, taking framework packages from about 60% to 100% passing after refactoring 45+ files. Contributed to the Security team's scanner, unblocking React Server Components adoption across the org.
- Designed a custom ESLint plugin (three tested rules, applied through shared config) that moved framework-pattern checks into the IDE for 30+ Next.js apps, and cut unit-test setup from 50+ lines to one call with typed mocks that fail at compile time.
- Wrote 12 framework guides in one quarter from recurring Slack and code-review questions, using an AI-built template I validated; partnered with a developer-efficiency team to feed them to an MCP server for AI coding agents. [METRIC?]

**Observability and performance**

- Wrote the design for web image-error reporting (CDN and failure type in New Relic). Took over a pull request stalled for about five months, wrote about half its final code, merged it, and owned the first production release and its 1% to 100% ramp (50 minutes). Later rewrote the image event queue in TypeScript.
- Rolled out framework performance reporting to 9 production apps owned by different teams in four weeks: proved it on one app, then reused an AI-assisted playbook with one independently mergeable PR per app. [METRIC?]

**Cross-team delivery**

- Owned ramp plans and staged releases of shared frontend packages, four in one quarter, all shipped cleanly. Ramped a shared navigation package from 0 to 100% in 72 minutes with no aborts or rollbacks. Cover on-call weeks.
- Upgraded 8 apps owned by different teams to a new major framework version, splitting one large multi-app upgrade into per-sub-app PRs so each could ship safely.
- Shipped Android navigation transitions for embedded web views after another team pulled me in, matching iOS for millions of users. Fixed an iOS bug blocking the QE team's Appium automation for every team using it.
- Reviewed about 260 PRs in two years. Organized the cross-team discussion that decided to fold the embedded-web client into the framework.

## Skills

- **Frontend:** React, Next.js (App Router, Server Components), TypeScript, GraphQL, Storybook
- **Quality and tooling:** ESLint, Jest, Cypress, Appium, CircleCI, Jenkins, esbuild, Nginx
- **Operations:** New Relic, Splunk, staged ramps, on-call
- **Practices:** design docs and ADRs, cross-team rollouts, AI-assisted development, MCP

## Education

[EDUCATION]

## Earlier Experience

[EARLIER EXPERIENCE: roles, employers and dates before this one]
