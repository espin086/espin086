# JJ Espinoza. AI/ML Engineering Projects

10+ years building distributed ML systems, LLM platforms, and production AI infrastructure across AWS, GCP, and Azure. Ranked by engineering depth, most to least.

## Ranked projects

### 1⃣ [configurable-llm-classifier](https://github.com/espin086/configurable-llm-classifier)
- **What it is:** A containerized LLM classification service where the label taxonomy lives in a YAML config, not code. swap the config and the same service classifies a different taxonomy with no redeploy.
- **Stack:** FastAPI, Docker, Kubernetes (ConfigMap/Secret), OpenAI API, pytest, GitHub Actions CI, a golden-set eval harness.
- **Relevant to:** LLM optimization, configurable rules engines, platform design for non-engineering iteration.

### 2⃣ [SageMakerLlamaGuard](https://github.com/espin086/SageMakerLlamaGuard)
- **What it is:** Deploys Meta's LlamaGuard 3 safety-classification model as a managed AWS SageMaker endpoint to screen LLM inputs/outputs for policy violations before they reach production.
- **Stack:** AWS SageMaker, Terraform (IaC), IAM, Python.
- **Relevant to:** Responsible AI governance, bias/risk mitigation infrastructure, AWS ML platform deployment.

### 3⃣ [GPT-Jobhunter](https://github.com/espin086/GPT-Jobhunter)
- **What it is:** An embeddings-based resume/job matching engine. scores a resume against thousands of postings 0-100% and generates a tailored resume rewrite per target job.
- **Stack:** Python, GPT embeddings, SQLite, Streamlit, Docker, CI/CD pipeline.
- **Relevant to:** Full ML product lifecycle (data → embeddings → serving → CI/CD), retrieval architecture.

### 4⃣ [adk-and-mcp](https://github.com/espin086/adk-and-mcp)
- **What it is:** A set of agents on Google's Agent Development Kit that reach external tools through MCP (Model Context Protocol) instead of hand-rolled function-calling glue, plus stateful multi-agent delegation.
- **Stack:** Google ADK, MCP, Gemini/GPT-4.1/Claude via LiteLLM, Poetry.
- **Relevant to:** AI platform / agent-tooling architecture, standards-based integration over point-to-point glue.

### 5⃣ [deepseek-ollama-fastapi](https://github.com/espin086/deepseek-ollama-fastapi)
- **What it is:** A Dockerized FastAPI/Uvicorn service wrapping Ollama for LLM inference, with both synchronous and token-streaming endpoints.
- **Stack:** FastAPI, Uvicorn, Ollama, Docker.
- **Relevant to:** Inference-serving architecture, latency-sensitive API design, containerized MLOps deployment.

### 6⃣ [AIProtoCritic](https://github.com/espin086/AIProtoCritic)
- **What it is:** Analyzes Protobuf schema files against Google's own Protobuf style guide and flags violations with an LLM-generated rationale, not just a lint-rule match.
- **Stack:** Python, open-source LLMs, Google Protobuf style guide as a grounding source.
- **Relevant to:** LLM-as-reviewer patterns, applying models to structured/technical artifacts instead of free text.

### 7⃣ [api-diet-optimizer](https://github.com/espin086/api-diet-optimizer)
- **What it is:** A linear-programming API that solves for the lowest-cost nutrition plan meeting a set of constraints (calories, macros, budget).
- **Stack:** Python, linear programming solver, REST API.
- **Relevant to:** Optimization under constraints, knowing when the right tool is a solver, not a model.

### 8⃣ [BigQueryChat](https://github.com/espin086/BigQueryChat)
- **What it is:** A chatbot that translates natural-language questions into BigQuery SQL and returns results conversationally.
- **Stack:** Python, Google BigQuery, LLM query generation.
- **Relevant to:** LLM-to-structured-query translation, schema-grounded generation.

### 9⃣ [MyKaggleCompetitions](https://github.com/espin086/MyKaggleCompetitions)
- **What it is:** A monorepo of Kaggle competition solutions across tabular and NLP problems.
- **Stack:** Python, pandas, scikit-learn, Jupyter.
- **Relevant to:** Model selection and evaluation methodology, feature engineering depth.

---

## Stack

<p align="left">
  <a href="https://aws.amazon.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/> </a>
  <a href="https://azure.microsoft.com/en-in/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/microsoft_azure/microsoft_azure-icon.svg" alt="azure" width="40" height="40"/> </a>
  <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a>
  <a href="https://cloud.google.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/> </a>
  <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a>
  <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a>
  <a href="https://opencv.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg" alt="opencv" width="40" height="40"/> </a>
  <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a>
  <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a>
  <a href="https://pytorch.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-icon.svg" alt="pytorch" width="40" height="40"/> </a>
  <a href="https://scikit-learn.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="scikit_learn" width="40" height="40"/> </a>
  <a href="https://seaborn.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" alt="seaborn" width="40" height="40"/> </a>
  <a href="https://www.sqlite.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/sqlite/sqlite-icon.svg" alt="sqlite" width="40" height="40"/> </a>
  <a href="https://www.tensorflow.org" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg" alt="tensorflow" width="40" height="40"/> </a>
</p>

---

<h3 align="left">GitHub Activity</h3>

<p align="left">
  <a href="https://github.com/ryo-ma/github-profile-trophy">
    <img src="https://github-profile-trophy.vercel.app/?username=espin086" alt="espin086" />
  </a>
</p>

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=espin086&show_icons=true&locale=en&layout=compact" alt="espin086" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=espin086&show_icons=true&locale=en" alt="espin086" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=espin086&" alt="espin086" />
</p>
