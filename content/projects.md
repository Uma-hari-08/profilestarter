# Projects

## Agentic Support Triage System (EdTech)

Automatically classifies and routes student support tickets: app bugs, loginfailures, payment issues, content errors and exam queries.

- Agents assign severity, gather context from logs, retrieve answers from a knowledge base, and escalate high-risk cases to a human.
- Built with LangGraph and LangChain, Pydantic structured outputs, Pinecone for retrieval, FastAPI and Redis.
- Hardest problems: non-deterministic escalation, context overflow in long tickets, and observability gaps. Fixed with explicit state, typed outputs and tracing.

## EdTech Learning Assistant (RAG)

A study assistant that answers learner questions from course material.

-  OCR pipeline to turn scanned material into searchable text.
- Hybrid retrieval with BM25 and dense embeddings, merged with RRF, then cross-encoder reranking.
- RAGAS evaluation gates in CI.
- An ML engineer on the team owned the classification models; I integrated their outputs into the pipeline.

## This portfolio chatbot

A live chat that answers questions about my experience, grounded in these notes.

- Retrieval over my own markdown files, answers generated with the Groq API.
- Guard layer to keep answers on topic and grounded.
- Evaluation set measuring retrieval hit rate and answer correctness separately.
- Deployed on Vercel with serverless functions.

## Smaller builds

- File Organiser Agent: a Python agent for practising tool use.
- Meal planning web app in Python.
- Story generation for special needs kids 
