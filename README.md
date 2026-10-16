# AI-QA Portfolio

Hands-on projects built while transitioning from QA/test-automation into AI evaluation engineering. Each project maps to a module in my [AI-QA Field Manual](../AI-QA/AI-QA-Master-Study-Plan.md) study plan and builds toward being able to write a real **Test Strategy** for a chatbot or an AI agent product.

## Projects

| Project | What it tests | Builds on | Primary tool(s) |
|---|---|---|---|
| [`projects/p1-rag-testing`](projects/p1-rag-testing) | RAG chatbot: retrieval precision/recall, faithfulness, groundedness, hallucination checks | RAG Architecture & Testing | LangChain + DeepEval |
| [`projects/p2-llm-judge`](projects/p2-llm-judge) | LLM-as-a-Judge pipeline, human vs. LLM grading on a golden dataset | AI Evaluation Metrics | DeepEval / custom rubric |
| [`projects/p3-agent-pyramid`](projects/p3-agent-pyramid) | Tool-using agent tested at all 4 layers of the AI-Native Test Pyramid | Agentic Workflows & Tool-Use Testing | Custom agent + pytest |
| [`projects/p4-redteam`](projects/p4-redteam) | Prompt regression + red-teaming/guardrail test suite, mapped to OWASP LLM Top 10 | Prompt Testing / AI Safety & Red Teaming | PromptFoo |
| [`projects/p5-framework`](projects/p5-framework) | Full DeepEval-based test framework, data-driven, CI/CD, HTML reports | DeepEval / Framework Design & CI/CD | DeepEval + GitHub Actions |
| [`projects/p6-reliability`](projects/p6-reliability) | Canary rollout + rollback plan, load-test findings (prompt-uniformity trap) | Production Reliability & Release Engineering | Toy load test + rollout-runbook doc |
| [`docs/`](docs) | Capstone: Test Strategy documents (chatbot + AI agent) | Everything above | — |

## Structure

```
ai-qa-portfolio/
├── datasets/       golden datasets (jsonl) shared across projects
├── metrics/        custom evaluation metric implementations
├── tests/          data-driven test suites
├── utils/          shared helpers: judge-model wrapper, RAG chain wrapper, config
├── reports/         generated HTML evaluation reports
├── projects/       one folder per portfolio project (P1-P6)
├── docs/           write-ups, including the final Test Strategy documents
└── .github/workflows/   CI pipeline (added in the framework-design phase)
```

## Status

Scaffolding only — projects are filled in as each corresponding study module is completed. See the module map in the Field Manual for hours/pacing.
