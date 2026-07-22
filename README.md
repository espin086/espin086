# JJ Espinoza. AI/ML Engineering Projects

10+ years building distributed ML systems, LLM platforms, and production AI infrastructure across AWS, GCP, and Azure. Ranked by engineering depth, most to least.

## Ranked projects

### 1⃣ 🧩 [configurable-llm-classifier](https://github.com/espin086/configurable-llm-classifier)
- 🎯 **Problem it solves:** Classification policy (labels, taxonomy, thresholds) usually lives in code, so every policy change needs an engineer and a redeploy. This service moves the policy into a YAML config so it changes without touching the container.
- 🛠️ **Technologies:** Python, FastAPI, OpenAI API, Docker, Kubernetes (ConfigMap/Secret), pytest, GitHub Actions CI, custom eval harness (golden-set accuracy scoring).
- 💡 **What it demonstrates:** Config-as-code platform design, decoupling decision logic from the deployment unit, CI-graded evals for a policy change before it reaches production. the same separation a production rules engine needs at scale.

### 2⃣ 🛡️ [SageMakerLlamaGuard](https://github.com/espin086/SageMakerLlamaGuard)
- 🎯 **Problem it solves:** LLM applications need a safety layer that screens prompts and responses for policy violations before they reach a user or a downstream system. this deploys that layer as a managed, autoscaling endpoint.
- 🛠️ **Technologies:** AWS SageMaker, Meta LlamaGuard 3, Terraform (Infrastructure as Code), IAM, Python.
- 💡 **What it demonstrates:** Responsible AI / bias and risk mitigation infrastructure, AWS ML platform deployment, version-controlled and destroyable infra instead of manual console setup.

### 3⃣ 💼 [GPT-Jobhunter](https://github.com/espin086/GPT-Jobhunter)
- 🎯 **Problem it solves:** Manually comparing a resume against thousands of job postings doesn't scale and keyword search misses semantically-matching roles. this scores every posting 0-100% by real similarity and rewrites the resume per target job.
- 🛠️ **Technologies:** Python, OpenAI embeddings, FastAPI, Streamlit, SQLite, Docker, CI/CD pipeline (GitHub Actions).
- 💡 **What it demonstrates:** Full ML product lifecycle (ingestion → embeddings → serving → CI/CD), retrieval architecture, decoupled backend/frontend for independent scaling.

### 4⃣ 🤖 [adk-and-mcp](https://github.com/espin086/adk-and-mcp)
- 🎯 **Problem it solves:** Hand-rolled function-calling glue between an agent and its tools doesn't scale past one or two integrations. this standardizes tool access on a protocol so new tools plug in without touching agent code.
- 🛠️ **Technologies:** Google Agent Development Kit (ADK), Model Context Protocol (MCP), Gemini, GPT-4.1 and Claude Opus via LiteLLM, Poetry.
- 💡 **What it demonstrates:** AI platform / agent-tooling architecture, standards-based integration over point-to-point glue, multi-agent delegation and session-state design across a model-agnostic runtime.

### 5⃣ ⚡ [deepseek-ollama-fastapi](https://github.com/espin086/deepseek-ollama-fastapi)
- 🎯 **Problem it solves:** A chat UI that blocks until a full LLM response is ready reads as broken. this serves both a synchronous endpoint and a token-streaming one so a client can render output as it's generated.
- 🛠️ **Technologies:** FastAPI, Uvicorn, Ollama, DeepSeek-R1, Docker.
- 💡 **What it demonstrates:** Inference-serving architecture, latency-sensitive API design (sync vs. streaming), containerized MLOps deployment.

### 6⃣ 🔎 [AIProtoCritic](https://github.com/espin086/AIProtoCritic)
- 🎯 **Problem it solves:** A regex-based linter catches syntax problems but misses "technically valid but bad practice" issues in a Protobuf schema. this uses an LLM grounded in Google's own style guide to catch those instead.
- 🛠️ **Technologies:** Python, open-source LLMs, Protobuf (.proto) parsing, Google Protobuf style guide as a grounding source.
- 💡 **What it demonstrates:** LLM-as-reviewer patterns, applying models to structured/technical artifacts instead of free text.

### 7⃣ 🥗 [api-diet-optimizer](https://github.com/espin086/api-diet-optimizer)
- 🎯 **Problem it solves:** Finding the lowest-cost nutrition plan that satisfies calorie, macro, and budget constraints simultaneously is a constrained-optimization problem, not a search problem.
- 🛠️ **Technologies:** Python, linear programming solver, REST API.
- 💡 **What it demonstrates:** Optimization under constraints, and knowing when the right tool for a job is a solver, not a model.

### 8⃣ 🗄️ [BigQueryChat](https://github.com/espin086/BigQueryChat)
- 🎯 **Problem it solves:** Non-SQL users need to ask data questions in plain English and get back a query that actually runs against the real schema, not a plausible-looking one that fails.
- 🛠️ **Technologies:** Python, Google BigQuery, LLM-driven SQL generation.
- 💡 **What it demonstrates:** LLM-to-structured-query translation, schema-grounded generation.

### 9⃣ 🏆 [MyKaggleCompetitions](https://github.com/espin086/MyKaggleCompetitions)
- 🎯 **Problem it solves:** A monorepo tracking model-selection and feature-engineering work across multiple Kaggle competitions, spanning tabular and NLP problem types.
- 🛠️ **Technologies:** Python, pandas, scikit-learn, Jupyter.
- 💡 **What it demonstrates:** Model selection and evaluation methodology, feature engineering depth across problem types.

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
  <img src="https://github-readme-stats.vercel.app/api?username=espin086&show_icons=true&locale=en" alt="espin086" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=espin086&" alt="espin086" />
</p>
