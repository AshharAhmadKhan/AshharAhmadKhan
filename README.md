# Ashhar Ahmad Khan

Third-year CS student at Jamia Hamdard, New Delhi. I have a habit of reading codebases until I find something broken, and an equally bad habit of not stopping there but fixing it. Fuelled by an unreasonable amount of coffee.

---

## Open Source

**Apache Fineract** — 10+ merged PRs since January 2026.

The most significant was removing the self-service module entirely: 196 files, around 11,300 lines, one commit. The module had been disabled after a security audit found seven distinct OWASP-class vulnerabilities, all rooted in the same architectural decision. Going through those files is what led me to propose the Borrower BFF (FINERACT-2439) — a standalone service that handles borrower identity and authentication correctly, separate from Fineract's back-office security model.

Other contributions include a PostgreSQL schema fix in the query service layer, removal of stale Pentaho report data, fixing undo transactions for Fixed Deposit accounts, batching N+1 database queries across several services, and removing a write path that had been silently broken since 2015.

**Apache Fory** — Added IEEE 754 float16 type support to the Rust runtime.

**Hiero SDK Python** — CI automation (conventional PR title enforcement), repr method implementations, and docstring improvements.

---

## GSoC 2026

Applied to GSoC 2026 to build the Borrower Backend-for-Frontend for Apache Fineract (FINERACT-2439 and FINERACT-2440). The proposal covers a standalone Spring Boot service with its own identity store, RS256 JWT authentication, HMAC OTP registration, idempotency enforcement, and a reference React client that validates the API end-to-end. The architecture came directly from the security analysis done during the self-service removal.

---

## Projects

**[MeetingMind](https://github.com/AshharAhmadKhan/MeetingMind)** — AWS AIdeas 2026 Semi-Finalist (Top 1000 of ~50,000 entries)
Serverless meeting intelligence platform across 14 AWS services. Uploads a recording, returns a transcript with speaker labels, extracted decisions, action items with risk scores, and a Kanban board to track follow-through. The part I think about most is the Graveyard — tasks untouched for 30 days with an AI-generated note on why they probably died. [Live demo](https://dcfx593ywvy92.cloudfront.net/login)

**[BrewAlgo](https://github.com/AshharAhmadKhan/BrewAlgo)**
Online coding judge built from scratch. Code runs in isolated Docker containers with strict CPU, memory, and time limits. WebSocket verdicts in real time. Backend structured in four Clean Architecture layers so the business logic is fully independent of Spring and the database. 100+ DSA problems, Java and Python support.

**[QuietText](https://github.com/AshharAhmadKhan/QuietText)**
Chrome extension that makes any webpage easier to read for people with dyslexia. Three reading presets with the OpenDyslexic font and adjusted spacing. AI simplification using Groq that breaks down complex text into shorter sentences and clearer structure. Built as a minor project in semester six.

---

## Stack

Java, Spring Boot, Python, FastAPI, TypeScript, Node.js, React, Docker, PostgreSQL, AWS

---

## Contact

itzashhar@gmail.com · [LinkedIn](https://linkedin.com/in/ashhar-ahmad-khan) · [Apache Fineract PRs](https://github.com/apache/fineract/pulls?q=author%3AAshharAhmadKhan)
