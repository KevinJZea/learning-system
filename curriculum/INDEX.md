# Curriculum Index

Router for the learning system. Keep this skimmable. Deep content lives in `topics/<slug>.md`.

**This file is the single owner of topic status, mastery, Bloom, last reviewed, and next_review.** Do not duplicate those fields in `progress.md`.

## How to use

- **Session start:** read this file with `PROFILE.md` and `progress.md`
- **Due reviews:** any row with `Next review` ≤ today → offer as review candidate
- **Teaching a topic:** open `topics/<slug>.md` if it exists
- **New topic:** copy `templates/topic.md` → `topics/<slug>.md`, then add a row here
- **Suggested next:** prefer gaps that unlock AI Engineering + backend/systems breadth (see PROFILE)

## Status legend

| Status | Meaning |
|--------|---------|
| `not_started` | No lesson file or only a stub |
| `in_progress` | Actively learning |
| `review` | Learned once; needs reinforcement |
| `mastered` | Meets mastery criteria in `AGENTS.md` |

## Topic map

| Topic | Slug | Status | Mastery | Bloom | Last reviewed | Next review | Prerequisites | Next | File |
|-------|------|--------|---------|-------|---------------|-------------|---------------|------|------|
| HTTP fundamentals | `http-fundamentals` | not_started | 0/5 | — | — | — | — | `api-design`, `caching-strategies` | — |
| Networking basics | `networking-basics` | not_started | 0/5 | — | — | — | — | `http-fundamentals` | — |
| OS mental model | `os-mental-model` | not_started | 0/5 | — | — | — | — | `docker-fundamentals` | — |
| API design | `api-design` | not_started | 0/5 | — | — | — | `http-fundamentals` | `auth-fundamentals`, `data-modeling` | — |
| Auth fundamentals | `auth-fundamentals` | not_started | 0/5 | — | — | — | `api-design` | `security-fundamentals` | — |
| Data modeling | `data-modeling` | not_started | 0/5 | — | — | — | `api-design` | `relational-databases` | — |
| Relational databases | `relational-databases` | not_started | 0/5 | — | — | — | `data-modeling` | `system-design` | — |
| Docker fundamentals | `docker-fundamentals` | not_started | 0/5 | — | — | — | `os-mental-model` | `cloud-fundamentals` | — |
| Cloud fundamentals | `cloud-fundamentals` | not_started | 0/5 | — | — | — | `docker-fundamentals` | `system-design` | — |
| System design | `system-design` | not_started | 0/5 | — | — | — | `api-design`, `relational-databases` | `distributed-systems`, `caching-strategies` | — |
| Distributed systems | `distributed-systems` | not_started | 0/5 | — | — | — | `system-design` | `message-queues` | — |
| Caching strategies | `caching-strategies` | not_started | 0/5 | — | — | — | `http-fundamentals` | `distributed-systems` | — |
| Message queues | `message-queues` | not_started | 0/5 | — | — | — | `system-design` | `distributed-systems` | — |
| Python for engineering | `python-for-engineering` | not_started | 0/5 | — | — | — | — | `data-pipelines`, `ml-fundamentals`, `llm-app-architecture` | — |
| Data pipelines | `data-pipelines` | not_started | 0/5 | — | — | — | `python-for-engineering` | `ml-fundamentals` | — |
| ML fundamentals | `ml-fundamentals` | not_started | 0/5 | — | — | — | `python-for-engineering` | `llm-app-architecture` | — |
| LLM app architecture | `llm-app-architecture` | not_started | 0/5 | — | — | — | `api-design`, `python-for-engineering` | `prompt-engineering`, `rag`, `llm-evals` | — |
| Prompt engineering | `prompt-engineering` | not_started | 0/5 | — | — | — | — | `llm-app-architecture`, `rag` | — |
| RAG | `rag` | not_started | 0/5 | — | — | — | `llm-app-architecture` | `production-ai` | — |
| LLM evals | `llm-evals` | not_started | 0/5 | — | — | — | `llm-app-architecture` | `production-ai` | — |
| Production AI | `production-ai` | not_started | 0/5 | — | — | — | `rag`, `llm-evals`, `observability` | — | — |
| Testing strategies | `testing-strategies` | not_started | 0/5 | — | — | — | — | `ci-cd` | — |
| CI/CD | `ci-cd` | not_started | 0/5 | — | — | — | `testing-strategies` | `observability` | — |
| Observability | `observability` | not_started | 0/5 | — | — | — | — | `production-ai` | — |
| Security fundamentals | `security-fundamentals` | not_started | 0/5 | — | — | — | `api-design` | `auth-fundamentals` | — |

## Suggested learning paths (high level)

Not a rigid syllabus—use as orientation. Adjust from progress and interest.

### Path A — Systems foundation (supports everything)

1. `networking-basics` → `http-fundamentals` → `os-mental-model`
2. `api-design` → `auth-fundamentals` → `data-modeling` → `relational-databases`
3. `docker-fundamentals` → `cloud-fundamentals`
4. `system-design` → `caching-strategies` → `distributed-systems` → `message-queues`

### Path B — Toward AI Engineering

1. `python-for-engineering`
2. `data-pipelines` · `ml-fundamentals`
3. `llm-app-architecture` · `prompt-engineering`
4. `rag` · `llm-evals`
5. `production-ai` (also needs `observability`)

### Path C — Quality & delivery

1. `testing-strategies` → `ci-cd`
2. `observability`
3. `security-fundamentals` (after `api-design`)

## Next recommended (from current state)

_No topics completed yet._

Given PROFILE (strong frontend → AI Engineering):

1. Pick a **systems** foundation topic (`http-fundamentals`, `api-design`, or `docker-fundamentals`) **or**
2. Pick an **AI Engineering** entry topic (`llm-app-architecture` after some API + Python, or start `python-for-engineering` / `prompt-engineering`)

Confirm with the learner’s motivation for the session.
