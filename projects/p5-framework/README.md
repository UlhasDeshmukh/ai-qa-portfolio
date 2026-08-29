# P5 — DeepEval Framework + CI/CD

Reimplements the P1 (RAG) and P2 (LLM-as-Judge) checks as real DeepEval test cases with real metric objects, wired into the repo's shared `datasets/`, `metrics/`, `utils/`, and `reports/` folders, plus a GitHub Actions workflow (`.github/workflows/`) that runs the suite on every push and publishes the HTML report as a build artifact.

Corresponds to Module 9 (DeepEval Framework Deep-Dive) and Module 10 (AI Testing Framework Design & CI/CD) in the Field Manual.
