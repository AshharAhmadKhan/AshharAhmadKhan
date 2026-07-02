# Ashhar Ahmad Khan

Fourth-year CS student at Jamia Hamdard, New Delhi. I have a habit of reading codebases until I find something broken, and an equally bad habit of not stopping there but fixing it.

## Research

**Stewardship Gaps and Debt Visibility: A Multi-Case Study of Latent Technical Debt in Apache Fineract**

An empirical paper studying three debt instances in Apache Fineract that persisted four to eleven years each, built directly from contribution work. The central argument is that visibility, not severity, determines how technical and security debt gets detected and retired.

Preprint: https://doi.org/10.5281/zenodo.20539368

Replication package: https://github.com/AshharAhmadKhan/debt-visibility-fineract

## Open Source

**Apache Fineract** — 14+ merged PRs since November 2025.

The most significant was removing the self-service module entirely: 142 files, around 11,000 lines, one commit. The module had been disabled after a security audit found multiple OWASP-class vulnerabilities, all rooted in the same architectural decision.

After that I found an API endpoint that had been silently throwing an error on every single call since August 2015. The implementation was a stub from its very first commit, never finished, never noticed for 11 years. Traced it through git history, raised it on the Apache dev mailing list, got community consensus, removed it.

Other contributions: PostgreSQL schema fixes, removal of stale report data, fixing undo and adjust transactions for Fixed Deposit accounts, batching N+1 database queries across several services.

**Apache Fory** - Added IEEE 754 float16 type support to the Rust runtime.

**Hiero SDK Python** - CI automation, repr method implementations, and cryptography documentation.

## Projects

**MeetingMind** - AWS AIdeas 2026 Semi-Finalist (Top 1000 of 10,000+ entries)

Serverless meeting intelligence platform across 14 AWS services. Uploads a recording, returns a transcript with speaker labels, extracted decisions, action items with risk scores, and a Kanban board to track follow-through. The part I think about most is the Graveyard — tasks untouched for 30 days get an AI-generated note on why they probably died. `

**BrewAlgo**

Online coding judge built from scratch. Code runs in isolated Docker containers with strict CPU, memory, and time limits. WebSocket verdicts in real time. Backend structured in four Clean Architecture layers so the business logic is fully independent of Spring and the database. 100+ DSA problems, Java and Python support.

**QuietText 2.0** - [Live Demo](https://quiet-text-2-0-offline.vercel.app)

Offline-first accessibility platform for dyslexic users. Simplifies text, PDFs, and images across 7 languages using Gemma 4 vision with a 128K context window, running fully on-device via Ollama. Chrome extension that passively applies dyslexia-friendly formatting across every website with no setup required.

## Stack

Java, Spring Boot, Python, FastAPI, TypeScript, Node.js, React, Docker, PostgreSQL, AWS

## Contact

itzashhar@gmail.com · [LinkedIn](https://linkedin.com/in/ashhar-ahmad-khan) · [Apache Fineract PRs](https://github.com/apache/fineract/pulls?q=is%3Apr+author%3AAshharAhmadKhan)
