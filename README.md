# Hi, I'm Pramit Roy

Software engineering student at **McMaster University** (B.Tech, expected 2028) in **Toronto**, with **5+ years of IT support** behind me: L1 and L2 support, device imaging and Chromebook support. I build software the way a support team needs it to behave: testable, observable, and honest about what it does not do.

I am looking for **full-time and co-op roles** in application and production support, QA automation and software development.

**Portfolio:** [pramitroy.tech](https://pramitroy.tech)

## Featured project: IT Ticketing System

[![CI](https://github.com/proyneon-hub/it-ticketing-system/actions/workflows/ci.yml/badge.svg)](https://github.com/proyneon-hub/it-ticketing-system/actions/workflows/ci.yml)
[![CodeQL](https://github.com/proyneon-hub/it-ticketing-system/actions/workflows/codeql.yml/badge.svg)](https://github.com/proyneon-hub/it-ticketing-system/actions/workflows/codeql.yml)

A role-based IT service desk with SLA tracking: a layered TypeScript/Express API on MongoDB, a React client, an OpenAPI contract, and the operational tooling around it. [**Live demo**](https://it-ticketing-system-pi.vercel.app/) · [**Repository**](https://github.com/proyneon-hub/it-ticketing-system) · [**Defect log**](https://github.com/proyneon-hub/it-ticketing-system/blob/main/docs/DEFECT_LOG.md)

![Creating a ticket, assigning it, working it to resolved and reading its history](https://raw.githubusercontent.com/proyneon-hub/it-ticketing-system/main/docs/screenshots/demo.gif)

What is in it, with the evidence in the repository:

- **723 automated tests in six layers**: API tests on a real MongoDB, an OpenAPI contract test, mocked and real-stack browser tests in three browsers, Axe accessibility checks, and Python monitoring scripts.
- **22 defects found and fixed**, each written up with how it was found, why the tests missed it, and a regression test that fails without the fix. Some were bugs that every mocked test passed and only a smoke test against the real stack, or the deployed site, caught.
- **Measured performance**: a text index cut search from 68 ms to 9 ms (p50) on 10,000 tickets. The same document records what got slower later (password hashing) and that it is not fixed yet.
- **Operations built in**: request ids that connect a user's error to a log line, Prometheus metrics with a Grafana dashboard, a runbook, and an hourly check of the live site that opens an incident issue when it fails.
- **Security and correctness decisions written down**: eight decision records covering authentication with rotating refresh tokens, optimistic concurrency, and a transactional outbox for notifications.

## Where I am strongest

| Application and production support                        | QA automation                                                 | Software development                                   |
| --------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------ |
| Runbooks, incident handling, monitoring, tracing an error | Playwright, Vitest, API and contract tests, accessibility, CI | TypeScript, React, Node/Express, MongoDB, Docker, REST |

## Get in touch

See my portfolio at [pramitroy.tech](https://pramitroy.tech).
