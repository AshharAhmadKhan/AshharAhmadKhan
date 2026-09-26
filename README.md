# Ashhar Ahmad Khan

Backend engineering student at Jamia Hamdard, New Delhi, seeking software engineering internships. I read codebases until I find something broken, then fix it.

## Open Source

**Apache Fineract** - 40+ merged pull requests, contributor since February 2026.

- Removed the entire self-service module (142 files, ~11,000 lines, a single commit) after a security audit found multiple OWASP-class vulnerabilities rooted in one architectural decision.
- Identified multiple API endpoints silently failing for 3–13 years, some stubbed since their first commit. Traced each through Git history, raised them with the development community, and removed them after consensus.
- Implemented undo/adjust support for Fixed Deposit transactions, batched N+1 queries across several services, hardened Feign method names across five modules, and fixed a range of PostgreSQL compatibility and NullPointerException issues.

## Research

**Stewardship Gaps and Debt Visibility: A Multi-Case Study of Latent Technical Debt in Apache Fineract** - preprint

An empirical study of three technical-debt instances in Apache Fineract that persisted 4–11 years each, built from the author's own contribution work. Argues that visibility, not severity, determines how debt gets detected and retired.

[Preprint](https://doi.org/10.5281/zenodo.20539368) · [Replication package](https://github.com/AshharAhmadKhan/debt-visibility-fineract)

## Projects

**MeetingMind** - AWS AIdeas 2026, Top 1000 of 10,000+ entries

Serverless meeting intelligence platform across 14 AWS services. Transcribes recordings, extracts decisions and action items with risk scores, and tracks follow-through on a Kanban board. Includes a Graveyard: tasks untouched for 30 days get an AI-generated note on why they probably died.

**BrewAlgo**

Online coding judge with Docker-isolated sandboxed execution, strict CPU/memory limits, and real-time WebSocket verdicts. Backend structured in four Clean Architecture layers, fully independent of Spring and the database. 100+ DSA problems, Java and Python support.

**QuietText 2.0** - [Live Demo](https://quiet-text-2-0-offline.vercel.app)

Offline-first accessibility platform for dyslexic users. Simplifies text, PDFs, and images across 7 languages using Gemma 4 vision, running fully on-device via Ollama. Chrome extension applies dyslexia-friendly formatting across every website with no setup.

## Stack

Java, Python, JavaScript, SQL, Spring Boot, REST APIs, WebSockets, Docker, React, PostgreSQL, MySQL, DynamoDB, AWS (Lambda, Bedrock, Transcribe, Cognito, CloudFront, SES)

## Contact

itzashhar@gmail.com · [LinkedIn](https://linkedin.com/in/ashhar-ahmad-khan) · [Apache Fineract PRs](https://github.com/apache/fineract/pulls?q=is%3Apr+author%3AAshharAhmadKhan)
