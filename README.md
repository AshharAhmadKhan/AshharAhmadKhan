# Ashhar Ahmad Khan

Third-year CS student at Jamia Hamdard, New Delhi. I have a habit of reading codebases until I find something broken, and an equally bad habit of not stopping there but fixing it. Fuelled by an unreasonable amount of coffee.

---

## Open Source

**Apache Fineract** — 12+ merged PRs since January 2026.

The most significant was removing the self-service module entirely: 142 files, around 11,000 lines, one commit. The module had been disabled after a security audit found multiple OWASP-class vulnerabilities, all rooted in the same architectural decision.

After that I found an API endpoint that had been silently throwing an error on every single call since August 2015. The implementation was a stub from its very first commit — never finished, never noticed for 11 years. Traced it through git history, raised it on the Apache dev mailing list, got community consensus, removed it.

Other contributions: PostgreSQL schema fix in the query service layer, removal of stale Pentaho report data, fixing undo and adjust transactions for Fixed Deposit accounts, batching N+1 database queries across several services.

**Apache Fory** — Added IEEE 754 float16 type support to the Rust runtime.

**Hiero SDK Python** — CI automation (conventional PR title enforcement), repr method implementations, and docstring improvements.

---

## Projects

**[MeetingMind](https://github.com/AshharAhmadKhan/MeetingMind)** — AWS AIdeas 2026 Semi-Finalist (Top 1000 of 10,000+ entries)

Serverless meeting intelligence platform across 14 AWS services. Uploads a recording, returns a transcript with speaker labels, extracted decisions, action items with risk scores, and a Kanban board to track follow-through. The part I think about most is the Graveyard — tasks untouched for 30 days with an AI-generated note on why they probably died. [Live demo](https://dcfx593ywvy92.cloudfront.net/login)

**[BrewAlgo](https://github.com/AshharAhmadKhan/BrewAlgo)**

Online coding judge built from scratch. Code runs in isolated Docker containers with strict CPU, memory, and time limits. WebSocket verdicts in real time. Backend structured in four Clean Architecture layers so the business logic is fully independent of Spring and the database. 100+ DSA problems, Java and Python support.

**[QuietText](https://github.com/AshharAhmadKhan/QuietText)**

Chrome extension that makes any webpage easier to read for people with dyslexia. Three reading presets with the OpenDyslexic font and adjusted spacing. AI simplification using Groq that breaks down complex text into shorter sentences and clearer structure.

---

## Stack

Java, Spring Boot, Python, FastAPI, TypeScript, Node.js, React, Docker, PostgreSQL, AWS

---

## Contact

itzashhar@gmail.com · [LinkedIn](https://linkedin.com/in/ashhar-ahmad-khan) · [Apache Fineract PRs](https://github.com/apache/fineract/pulls?q=author%3AAshharAhmadKhan)
