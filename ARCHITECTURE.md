# Ascendify Architecture (MVP-level)

## Goals
- Rapid iteration with clean boundaries: UI / API / Data / AI.
- Measurable learning outcomes: mastery pacing, weak-topic surfacing.
- Safe & auditable AI: prompt/versioning discipline, guardrails, evals.

## Proposed Components
- Web (Next.js/TS): Auth, dashboards, planners, content rendering.
- API (FastAPI/TS): Study plan + session engines, progress services.
- AI Layer: Prompt lib, RAG retrieval (syllabus extracts), evaluation harness.
- Data: Postgres (users, syllabus, sessions, mastery), object storage for assets.
- Observability: Logging, metrics (user actions, model calls), feature flags.

## Data Sketch
- users(id, name, email, school)
- topics(id, subject, unit, title, difficulty)
- mastery(user_id, topic_id, value_0_1, last_updated)
- sessions(id, user_id, date, plan_json)
- prompts(id, name, version, template)

## AI Notes
- Confidence input -> topic weight adjustment -> plan generation.
- "Low-confidence rule": if topic_conf < theta, scaffold easier variants first; pin for review.
- Eval sets: seed with past exam Qs and teacher-curated items.

## Security & Privacy
- Store minimal PII; encrypt at rest; role-based access; opt-in analytics.
