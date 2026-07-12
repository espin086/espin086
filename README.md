# Hi, I'm JJ! 👋 Production AI/ML, End to End

I build and ship machine learning systems: **LLM applications**, **decisioning microservices**, and **data pipelines** that run with tests, CI, and containers, not just notebooks. 14+ years in ML across media, tech, and cloud consulting; these are the personal projects where I prove out ideas in code.

I work across **AWS** and **Google Cloud**, with **Python**, **FastAPI**, **Docker**, and **Kubernetes** as the default stack.

## Featured Projects

_Every project below is public code you can run. The ones at the top carry full test suites, CI, and containerized deploys._

---

### 💼 **GPT-Jobhunter** [[repo](https://github.com/espin086/GPT-Jobhunter)] ⭐ 93 stars

An **AI job-search platform** used by real job seekers: **embedding-based similarity scoring** matches resumes to live job postings 0-100%, and an **LLM pipeline rewrites the resume** for the jobs worth chasing. This is a complete ML product, from feature generation to serving.

**Why it matters**: the same shape as production personalization and ranking systems: embed user and item text, score, rank, act on the ranking.

**Key Technologies**:
- AI/ML: **LLM embeddings**, **similarity scoring**, **LLM resume tailoring**, ATS scoring.
- Engineering: **FastAPI**, **Streamlit**, **Docker + docker-compose**, **GitHub Actions CI**, **full pytest suite**, **OpenAPI spec**.

---

### 🎛️ **Configurable LLM Classifier** [[repo](https://github.com/espin086/configurable-llm-classifier)]

A **config-driven LLM decisioning microservice**: business users change **YAML**, not code, and the service returns **label, confidence, and reasoning** for any text classification task. Built the way regulated decisioning systems get built: deterministic config, an **eval harness with a golden set and an accuracy gate in CI**, and **Kubernetes manifests** for deployment.

**Why it matters**: auditable, testable LLM decisions, the pattern behind fraud flags, credit-risk triage, and complaint routing.

**Key Technologies**:
- AI/ML: **LLM classification**, **eval harness** (golden set, accuracy gate), confidence + reasoning outputs.
- Engineering: **FastAPI**, **pytest**, **GitHub Actions CI**, **Docker**, **Kubernetes** (ConfigMap/Secret/Deployment/Service).

---

### 📰 **NewsWaveMetrics** [[repo](https://github.com/espin086/NewsWaveMetrics)]

A platform that scores **news sentiment** and correlates it against **stock market prices** and economic indicators, so a story's tone becomes a measurable market signal. **NLP sentiment models** on national and local news, joined to **time series** of real financial data.

**Why it matters**: unstructured text turned into quantitative signal against financial market data.

**Key Technologies**:
- AI/ML: **NLP sentiment analysis**, **time series analysis**.
- Engineering: **Python**, **Pandas**, **SQLite**, API integration (**Yahoo Finance**, RapidAPI).

---

### 📈 **Stocks: Portfolio Optimizer** [[repo](https://github.com/espin086/Stocks)]

A stock analysis tool that runs **portfolio optimization** over historical price data and recommends **budget allocation across holdings**. Applied quantitative finance: expected returns, risk, and allocation under constraints (I hold an M.S. in Econometrics, and it shows here).

**Key Technologies**:
- Quant: **portfolio optimization**, historical return/risk modeling.
- Engineering: **Python**, financial data APIs.

---

### 🎭 **EmoTrack** [[repo](https://github.com/espin086/EmoTrack)]

**Real-time facial-emotion analytics** from webcam input, with trend dashboards for daily and weekly patterns. Ships in three modes (standalone, full-stack, Docker) with a **tested, CI-gated** codebase.

**Key Technologies**:
- AI/ML: **AWS Rekognition** for emotion detection.
- Engineering: **FastAPI**, **Streamlit**, **SQLite**, **pytest + GitHub Actions CI**, per-service **Dockerfiles + compose**.

---

### 🏠 **PropertyBot Data AI Pipeline** [[repo](https://github.com/propertybot/data-pipeline)]

An **automated real-estate data pipeline**: **AWS Rekognition** classifies listing photos and **custom NLP models** score property descriptions, on serverless AWS infrastructure with CI/CD. Related work led to **US patent #62/774,446** (AI-driven, image-oriented real estate analysis).

**Key Technologies**:
- AI/ML: **AWS Rekognition**, **custom NLP models**.
- Engineering: **AWS Lambda, SQS, DynamoDB, RDS**, **GitHub Actions CI/CD**.

---

### 🎙️ **recapio.io** [[repo](https://github.com/AI-Solutions-Lab-LLC/recapio.io)]

A meeting **transcription and summarization product** with real users, payments, and auth: **OpenAI Whisper** for transcription, **LLMs** for summaries, **Stripe** for billing, **Auth0** for identity, on AWS.

**Key Technologies**:
- AI/ML: **OpenAI Whisper**, **LLM summarization**.
- Engineering: **Streamlit**, **Auth0**, **Stripe**, **AWS RDS, S3, EC2**.

---

<h3 align="left">Languages and Tools:</h3>

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

<h3 align="left">My GitHub Activity:</h3>

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
