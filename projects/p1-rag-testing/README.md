# P1 — RAG Chatbot Test Suite

Builds a simple RAG chain, then tests it deliberately:

- Retrieval: context precision, context recall
- Generation: faithfulness, groundedness, hallucination checks
- Break tests: shrink chunk size until answers degrade, ask a question the docs don't cover, ask a question where two retrieved chunks conflict

Corresponds to Module 4 (RAG Architecture & RAG Testing) in the Field Manual.
