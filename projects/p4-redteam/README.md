# P4 — Prompt Regression & Red-Team Suite

Built with **[PromptFoo](https://www.promptfoo.dev)**:

- `promptfooconfig.yaml`: prompt regression suite — positive / negative / edge-case tests, deterministic assertions plus at least one Model-Graded (`llm-rubric`) assertion, versioned so a prompt change can be checked against prior passing behavior
- Red-team pass: PromptFoo's red-teaming mode configured with this app's context (purpose, features, rules), run at "Small" scope first
- Red-team log: every finding triaged with the Field Manual's AI bug report template — repro steps, expected vs. actual, mapped to an **OWASP LLM Top 10** category, severity, which guardrail (if any) caught it

Corresponds to Module 3 (Prompt Testing) and Module 8 (AI Safety, Bias & Red Teaming) in the Field Manual.
