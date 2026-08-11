# AI Agents Workshop

Student-facing materials for the **AI Agents Workshop**, developed for the
UCLA Master of Quantitative Economics program in Spring 2026.

The four-session curriculum moves from a first tool-using agent to retrieval,
multi-agent orchestration, and production deployment. Examples focus on
economic and financial research.

## Curriculum

1. **Foundations and single agents** — structured outputs, tool calling, FRED,
   and a ReAct loop. [Notebook](notebooks/01-foundations.ipynb) ·
   [Slides](slides/01-foundations.pdf)
2. **RAG and document intelligence** — document chunking, vector retrieval,
   grounded synthesis, and evaluation.
   [Notebook](notebooks/02-rag-document-intelligence.ipynb) ·
   [Slides](slides/02-rag-document-intelligence.pdf)
3. **Multi-agent orchestration** — a reproducible macro research crew that
   compares Federal Reserve Beige Book releases.
   [Notebook](notebooks/03-multi-agent-orchestration.ipynb) ·
   [Slides](slides/03-multi-agent-orchestration.pdf)
4. **Deployment and production** — MCP-style interfaces, specifications,
   guardrails, cost controls, evaluation, and observability.
   [Notebook](notebooks/04-deployment-production.ipynb) ·
   [Slides](slides/04-deployment-production.pdf)

See the [notebook guide](notebooks/README.md) for session prerequisites and the
[public syllabus](docs/syllabus.md) for learning objectives.

## Quick start

You need Python 3.11 or newer and JupyterLab.

```bash
git clone https://github.com/lorayc/ai-agents.git
cd ai-agents
python -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
cp .env.example .env
jupyter lab
```

Add your own API keys to `.env` before Sessions 1 and 2:

- `ANTHROPIC_API_KEY` — required for Claude API exercises.
- `FRED_API_KEY` — available free from the
  [Federal Reserve Bank of St. Louis](https://fred.stlouisfed.org/docs/api/api_key.html).

Never commit `.env`. API use may incur charges from the relevant provider.
Sessions 3 and 4 include workflows that can be explored without an LLM API key.

## Repository scope

This public repository contains participant materials only. Instructor
solutions, internal teaching notes, credentials, and generated research data
are intentionally excluded.

## License

Code and educational materials are available under the [MIT License](LICENSE).
