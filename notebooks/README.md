# Notebook Guide

Work through the sessions in order. Each notebook combines short explanations,
guided code, and exercises.

## Session 1: Foundations

[Open the notebook](01-foundations.ipynb)

Build a first Claude-powered agent, define structured outputs, call a FRED data
tool, and assemble a ReAct loop.

Requires `ANTHROPIC_API_KEY` and `FRED_API_KEY`.

## Session 2: RAG and document intelligence

[Open the notebook](02-rag-document-intelligence.ipynb)

Load and chunk policy documents, store embeddings in ChromaDB, retrieve
evidence, combine retrieval with live economic data, and evaluate results.

Requires `ANTHROPIC_API_KEY` and `FRED_API_KEY`.

## Session 3: Multi-agent orchestration

[Open the notebook](03-multi-agent-orchestration.ipynb)

Separate a Beige Book research pipeline into planning, collection, parsing,
scoring, comparison, and validation responsibilities. The baseline uses
ordinary Python classes so that orchestration and handoffs remain visible.

The baseline does not require an LLM key, but it downloads public Federal
Reserve pages and therefore requires internet access.

## Session 4: Deployment and production

[Open the notebook](04-deployment-production.ipynb)

Turn an agent concept into a deployment specification with MCP-style tools,
permissions, guardrails, model routing, cost estimates, evaluation gates, and
an inspectable runtime trace.

This lab is offline and API-free.

## Working safely

- Copy `.env.example` to `.env` and keep real keys only in that ignored file.
- Review notebook code before running it, especially cells that call external
  services.
- Treat model output as untrusted input and validate it before using it in
  analytical or operational decisions.
- API behavior, model names, and pricing change over time; consult provider
  documentation when reproducing the exercises.
