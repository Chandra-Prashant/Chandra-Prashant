# Hi, I'm Prashant Chandra 👋

**AI Research & Systems Engineer**  
*B.Tech Computer Engineering @ Aligarh Muslim University (Class of 2027)*  
*Focus: Applied Agentic AI, Tool Governance, Decoupled Deep Learning Architectures, & Local RAG Systems*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/prashant-chandra-)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://prashant-chandra.vercel.app)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:prashant.chandra.aligarh@gmail.com)

---

### 🏛️ Academic & Research Summary

* **University:** Aligarh Muslim University (AMU), India
* **Undergraduate:** B.Tech in Computer Engineering — **CGPA: 8.21 / 10**
* **Prior Credentials:** Diploma in Computer Engineering — **CGPA: 9.66 / 10 (Rank 1 / Gold Medalist)**
* **Research Focus:** Preparing for competitive MS in Computer Science / AI Research roles.
* **Hackathons:** Selected — AIsome 2026.

---

### 🔬 Active Research Internships

* 🔬 **MANIT Bhopal** — *Research Intern* (Jun. 2026, On-site)
  * Designed a ~118K-parameter decoupled denoising and cross-modal fusion pipeline achieving **29.85 dB PSNR**, **0.99 SSIM**, and **237 FPS** inference (measured directly from the notebook's evaluation run - see `Lightweight-Multispectral-Image-Fusion`).
  * Formulated an Inverse-Attention Gating Mask to bypass sensor degradation on the MSRS dataset.

* 🎓 **RV University** — *Research Intern* (Jun. – Jul. 2026, Remote)
  * Engineering zero-cloud local RAG pipelines (Qdrant, Ollama/Mistral-7B) for automated security report generation.
  * Building NetworkX-based Graph Causal Engines to reduce OS telemetry log volume by >80% while preserving causal lineage.

* 🧠 **Bodhi Hub** — *AI Intern* (Aug. – Sep. 2026, Hybrid)
  * Built the anti-hallucination architecture for an LLM-driven Verra VCS v5.0 audit-automation engine: all regulated numeric calculation lives in an isolated, AI-free domain layer, extraction output is schema-guarded against every value the engine computes, and generated narrative text is rejected outright if it contains a digit.
  * Shipped with 956 backend and 51 frontend tests passing, including a RAG index that strips quantities before indexing so there's nothing for the model to copy from a past client report.

---

### 📄 Publications & Manuscripts

1. **Decoupled Dual-Phase Network for Multispectral Image Fusion under Sensor Degradation**
   * *Venue:* NPDSM 2026 (MANIT Bhopal), **Springer** Lecture Notes in Mechanical Engineering (LNME) — selected & presented June 26, 2026. *(Published)*
2. **Robustness-Fairness Gap in Facial Recognition Architectures Under Stressors**
   * *Venue:* **IC3AI 2026**, NIT Jalandhar (18–19 December) — evaluating 52.5K matching trials across demographic and geometric resilience boundaries. *(Accepted)*
3. **A Selective Classification Framework for High-Reliability Anomaly Detection in Satellite Telemetry**
   * *Venue:* **UPCON 2026**. *(Under Review)*
4. **Cross-Lingual Stance Detection for Climate Change Discourse in Hindi and Bengali: Comparing Zero-Shot Transfer and Fine-Tuned Multilingual Transformers**
   * *Venue:* **ICACECT 2027**. *(Under Review)*

---

### 🛠️ Technical Stack

| Domain | Stack / Tooling |
| :--- | :--- |
| **Agentic AI & LLMs** | Google GenAI SDK (Gemini 2.5), Ollama, Qdrant Vector DB, RAG Pipelines, Tool Supervision |
| **Deep Learning & CV** | PyTorch, OpenCV, Computer Vision, Multispectral Fusion, XAI (Grad-CAM, SHAP), CUDA |
| **Systems & Graph Engine**| Python, C, C++, NetworkX, FastAPI, Docker, Microservices, SQL, `pytest`, `shlex` |
| **Web Infrastructure** | Next.js, React, TypeScript, Tailwind CSS, Vercel |

---

### 🚀 Featured Repositories

#### 🧠 [Bodhi Hub: Verifiable Audit Automation](https://github.com/Chandra-Prashant/bodhi-hub-vcs5)
*LLM-driven carbon-credit audit engine that is architecturally forbidden from touching a number.*
* All regulated calculation lives in an AI-free domain layer; extraction is schema-guarded, RAG context is number-redacted, and generated narrative is rejected if it contains a digit.
* **956 backend + 51 frontend tests passing.**
* **Stack:** FastAPI, PostgreSQL/pgvector, React, Docker, Alembic.

#### 🔧 [autoheal-sre: Self-Healing Code Repair Agent](https://github.com/Chandra-Prashant/autoheal-sre)
*An agent that fixes failing Python tests, but only ever ships a patch a human approved.*
* tree-sitter call-graph retrieval (not text chunking) feeds a 4-node LangGraph diagnose→plan→code→verify loop; every patch is verified against the *full* test suite inside a network-isolated Docker sandbox and rejected outright if it touches a test file.
* PR creation is gated behind explicit human approval — a passing patch never ships itself.
* **Stack:** Python, LangGraph, tree-sitter, ChromaDB, Docker, FastAPI.

#### 👤 [Face Bias Study](https://github.com/Chandra-Prashant/face-bais-study)
*A 52,500-trial fairness audit — accepted at IC3AI 2026 (NIT Jalandhar).*
* Three face-verification models across 14 intersectional demographic cohorts under five image stressors; a two-way ANOVA confirms a statistically significant cohort × stressor interaction, with VGG-Face's true positive rate collapsing to 2.4% for one cohort under eye occlusion.
* **Stack:** Python, DeepFace, statsmodels, Grad-CAM.

#### 🌡️ [Lightweight Multispectral Image Fusion](https://github.com/Chandra-Prashant/Lightweight-Multispectral-Image-Fusion)
*A 117.5K-parameter decoupled denoising + fusion network — the basis for the NPDSM 2026 (Springer LNME) paper.*
* An inverse-attention gating layer down-weights thermal features exactly where a noise map says the sensor was least reliable.
* **29.85 dB PSNR, 0.99 SSIM, 237 FPS**, measured directly from the evaluation run.
* **Stack:** PyTorch, OpenCV, thop.

#### 🛡️ [Malware Log Synthesis for DFIR](https://github.com/Chandra-Prashant/malware-log-synthesis-dfir)
*Local, LLM-assisted malware triage — the RV University internship work.*
* NetworkX causal-graph filtering prunes OS noise from a sandbox log's process tree before anything gets indexed into a local Qdrant store; a local Mistral-7B (Ollama) drafts the triage report, and a hallucination auditor blocks the PDF export if it cites a process that isn't actually in the log.
* **Stack:** Python, NetworkX, Qdrant, Ollama, Streamlit.

---

### 📈 GitHub Activity & Stats

<p align="center">
  <img src="https://github-readme-stats.hackclub.dev/api?username=Chandra-Prashant&show_icons=true&theme=tokyonight&hide_border=true" alt="Prashant's GitHub stats" width="48%" />
  <img src="https://github-readme-stats.hackclub.dev/api/top-langs/?username=Chandra-Prashant&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" width="48%" />
</p>

---

<p align="center">
  <sub>Scientific Rigor + Systems Engineering</sub>
</p>
