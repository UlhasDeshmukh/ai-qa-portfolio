# P3 — Agent Test Pyramid

A calculator-tool agent that solves word problems, tested at all 4 layers of the AI-Native Test Pyramid:

1. Tool-level — unit-test the calculator function directly
2. Tool-calling — verify the model picks the calculator tool (not another) for a math question
3. Workflow/orchestration — a 2-step problem requiring sequenced tool calls
4. End-to-end — full task correctness

Includes one deliberately broken layer (e.g. malformed tool schema) with a trace of how far up the pyramid the failure surfaces.

Corresponds to Module 7 (Agentic Workflows & Tool-Use Testing) in the Field Manual.
