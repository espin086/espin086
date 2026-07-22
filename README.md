# JJ Espinoza. AI/ML Engineering Projects

10+ years building distributed ML systems, LLM platforms, and production AI infrastructure across AWS, GCP, and Azure. The projects below are personal builds, ranked by engineering depth. architecture, scale, and design tradeoffs, not just "uses an LLM."

## Ranked projects

### 1. [configurable-llm-classifier](https://github.com/espin086/configurable-llm-classifier)
A containerized text classification system where the classification logic. labels, prompts, thresholds. is driven entirely by a YAML config file, not hardcoded. Swap a config, redeploy nothing, and the same service classifies a different taxonomy. This is the platform pattern behind a rules engine: separate the decision logic from the deployment unit so product and ops can iterate without an engineering release cycle.
**Relevant to:** LLM optimization, configurable rules engines, platform design for non-engineering iteration.

### 2. [SageMakerLlamaGuard](https://github.com/espin086/SageMakerLlamaGuard)
Deploys a LlamaGuard-class safety/guardrail model on AWS SageMaker to screen LLM inputs and outputs for policy violations before they reach a production path. The engineering problem here isn't the model, it's the infrastructure: real-time inference latency budget, endpoint autoscaling, and where in the request path a safety check can sit without doubling response time.
**Relevant to:** Responsible AI governance, bias/risk mitigation infrastructure, AWS ML platform deployment.

### 3. [GPT-Jobhunter](https://github.com/espin086/GPT-Jobhunter)
An embeddings-based resume/job matching engine. computes semantic similarity between a resume and thousands of job postings, scores each 0-100%, and generates a tailored resume rewrite per target job. Backed by SQLite, containerized, with a CI/CD pipeline that runs the test suite on every push. The interesting engineering choice: matching runs on embeddings rather than keyword search, which is what makes the 0-100% score meaningful instead of a fuzzy string match.
**Relevant to:** Full ML product lifecycle (data to embeddings to serving to CI/CD), retrieval architecture.

### 4. [adk-and-mcp](https://github.com/espin086/adk-and-mcp)
An agent built on Google's Agent Development Kit that reaches external tools through MCP (Model Context Protocol) instead of hand-rolled function-calling glue. The architectural bet: standardize tool integration on a protocol so new tools plug in without touching the agent's core logic. the same problem a platform team solves when it needs one agent runtime to serve many product teams' tools.
**Relevant to:** AI platform / agent-tooling architecture, standards-based integration over point-to-point glue.

### 5. [deepseek-ollama-fastapi](https://github.com/espin086/deepseek-ollama-fastapi)
A Dockerized FastAPI/Uvicorn service wrapping Ollama for LLM inference, with both synchronous and token-streaming endpoints. Streaming matters here for a concrete reason: a chat UI waiting on a full generation before showing anything reads as broken, so the service has to keep a connection open and flush tokens as the model produces them, not buffer the whole response.
**Relevant to:** Inference-serving architecture, latency-sensitive API design, containerized MLOps deployment.

### 6. [AIProtoCritic](https://github.com/espin086/AIProtoCritic)
Analyzes Protobuf schema files against Google's own Protobuf style guide and flags violations with an LLM-generated rationale, not just a lint rule match. Useful case study in using an LLM as a reviewer against a written spec instead of a fixed rule set. catches the "technically valid but bad practice" violations a regex-based linter misses.
**Relevant to:** LLM-as-reviewer patterns, applying models to structured/technical artifacts instead of free text.

### 7. [api-diet-optimizer](https://github.com/espin086/api-diet-optimizer)
A linear-programming API that solves for the lowest-cost nutrition plan meeting a set of constraints (calories, macros, budget). Not an LLM project. it's a constrained-optimization service, and it's here because distinguished-engineer-level work includes knowing when the right tool is a solver, not a model.
**Relevant to:** Optimization under constraints, API design for a computationally distinct problem class.

### 8. [BigQueryChat](https://github.com/espin086/BigQueryChat)
A chatbot that translates natural-language questions into BigQuery SQL and returns results conversationally. The hard part is the schema-grounding step: the model has to know the actual table structure before it can write a query that runs, not just a query that looks plausible.
**Relevant to:** LLM-to-structured-query translation, schema-grounded generation.

### 9. [MyKaggleCompetitions](https://github.com/espin086/MyKaggleCompetitions)
A monorepo of Kaggle competition solutions. feature engineering, model selection, and evaluation across tabular and NLP problems. Ranked lower here because competition notebooks are a different discipline than production systems, but they're the clearest evidence of raw modeling technique.
**Relevant to:** Model selection and evaluation methodology, feature engineering depth.

---

## Not on this list

Older tutorial-following repos (`LangChainCrashCourse`, `lang-graph-course`, `agent-development-kit-masterclass`, `KubernetesCrashCourse`), forks of other people's tools (`Jobs_Applier_AI_Agent_AIHawk`, `FoloUp`), and non-AI utility repos are excluded. this list is scoped to original AI/ML engineering work.

## Repos that need a visibility change

Three of the projects above are currently **private** and need to be switched to public before the links resolve for anyone but me:

- `configurable-llm-classifier`
- `SageMakerLlamaGuard`
- `sagemaker-jumpstart-deployer` (SageMaker JumpStart deployment tooling. held back from the ranked list pending a README pass, but worth making public regardless)

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
