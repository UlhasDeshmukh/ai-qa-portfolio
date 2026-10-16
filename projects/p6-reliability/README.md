# P6 — Canary Rollout, Rollback Plan & Load-Test Findings

A production-reliability deliverable for one of the earlier portfolio projects (P1 RAG chatbot or P3 agent):

- `rollout-runbook.md` — a canary rollout plan for the service: traffic progression (e.g. 1% → 10% → 25% → 50% → 75% → 100%), the 5 gate metrics and thresholds (latency percentiles, cost per request, error/refusal rate, output-length distribution, user-feedback rate), the project's own measured noise floor (run-to-run variance with no change), and a rollback mechanism that is a policy/config flip, not a redeploy.
- `load-test.md` — a toy load test comparing a single repeated prompt against a realistic varied-prompt distribution, demonstrating the prompt-uniformity trap (why looping one prompt makes performance look artificially good via prefix caching) with real P50/P90 numbers from both runs.

Corresponds to Module 11 (Production Reliability & Release Engineering) in the Field Manual — mined from `aiengineeringfromscratch.com`'s open-source "AI Evaluation and Reliability" career route.
