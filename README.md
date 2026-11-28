# JJ Espinoza

**ML/AI engineer and economist with 10+ years of experience.** I build LLM applications, ML platforms and the cloud infrastructure that runs them in production.

| | |
|---|---|
| **Focus** | LLM applications and agents, model evaluation, MLOps, applied econometrics |
| **Cloud** | AWS, GCP, Azure |
| **Core stack** | Python, SQL, FastAPI, Docker, Kubernetes, Terraform, GitHub Actions |
| **Open source** | [GPT-Jobhunter](https://github.com/espin086/GPT-Jobhunter): 97 stars, 21 forks |

## Featured projects

### [GPT-Jobhunter](https://github.com/espin086/GPT-Jobhunter)
An AI job-search app. It scores every job posting from 0 to 100% against a resume and rewrites the resume for the target job.
- **Skills shown:** end-to-end ML product, embeddings and semantic search, API and UI built as separate services
- **Tech:** Python, OpenAI embeddings, FastAPI, Streamlit, SQLite, Docker, GitHub Actions

### [econometrics](https://github.com/espin086/econometrics) [![CI](https://github.com/espin086/econometrics/actions/workflows/ci.yml/badge.svg)](https://github.com/espin086/econometrics/actions/workflows/ci.yml)
An open-source econometrics tool for graduate research at Cal State Fullerton. It pulls FRED and IMF data and estimates structural VAR models of how foreign shocks move a small economy, with published reports on Nicaragua and Brazil.
- **Skills shown:** time-series econometrics, a tested Python package with an automated release pipeline, AI coding agents working under review gates
- **Tech:** Python CLI, FRED and IMF data, Docker, GitHub Actions (tests, CodeQL, release pipeline)

### [configurable-llm-classifier](https://github.com/espin086/configurable-llm-classifier) [![CI](https://github.com/espin086/configurable-llm-classifier/actions/workflows/ci.yml/badge.svg)](https://github.com/espin086/configurable-llm-classifier/actions/workflows/ci.yml)
An LLM guardrail service. A business team changes what gets flagged by editing a config file, with no engineer and no redeploy.
- **Skills shown:** platform design, automated model evaluation in CI, Kubernetes deployment
- **Tech:** Python, FastAPI, OpenAI API, Docker, Kubernetes, pytest, GitHub Actions

### [SageMakerLlamaGuard](https://github.com/espin086/SageMakerLlamaGuard)
An AI safety layer on AWS. It deploys Meta's LlamaGuard 3 as an autoscaling endpoint that screens prompts and responses for policy violations.
- **Skills shown:** responsible AI, AWS ML deployment, infrastructure as code
- **Tech:** AWS SageMaker, Terraform, IAM, Python

### [api-diet-optimizer](https://github.com/espin086/api-diet-optimizer)
An optimization API. It finds the lowest-cost diet that meets calorie, macro and budget limits.
- **Skills shown:** linear programming, API design, tested and containerized service
- **Tech:** Python, FastAPI, Docker, Terraform

**More:** [adk-and-mcp](https://github.com/espin086/adk-and-mcp) (AI agents on Google ADK and the Model Context Protocol) · [deepseek-ollama-fastapi](https://github.com/espin086/deepseek-ollama-fastapi) (streaming API for a local LLM) · [AIProtoCritic](https://github.com/espin086/AIProtoCritic) (LLM code review for Protobuf schemas) · [EmoTrack](https://github.com/espin086/EmoTrack) (real-time emotion detection from a webcam)

## Skills

- **AI and ML:** LLM applications, AI agents, embeddings and retrieval, model evaluation, AI safety guardrails, scikit-learn, pandas
- **LLM platforms:** OpenAI, Claude and Gemini APIs, Google ADK, Model Context Protocol (MCP), LlamaGuard, Ollama
- **Backend:** Python, SQL, FastAPI, REST APIs, Streamlit, SQLite, BigQuery
- **Cloud and DevOps:** AWS (SageMaker, IAM), GCP (BigQuery), Docker, Kubernetes, Terraform, CI/CD with GitHub Actions
- **Quantitative:** econometrics (VAR and structural VAR), linear programming and optimization

## How I work

- **Spec before code.** A change starts as a written proposal, and each requirement gets a test.
- **AI agents under review.** I use Claude Code and Codex daily, behind the same tests, CI checks and review gates as my own code.
- **Models are tested like code.** A prompt or policy change is scored against a known-answer set before it ships.
