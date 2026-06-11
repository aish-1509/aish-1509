<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=6C63FF&center=true&vCenter=true&width=600&lines=Aishwarya+Anand;AI+%2F+ML+Engineer;NTU+Computer+Science+%E2%80%94+AI+Specialisation;Building+production+AI+systems" alt="Typing SVG" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/aishwarya-anand-b963661b3)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aish0021@e.ntu.edu.sg)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://aishwarya-portfolio-tau.vercel.app)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/aish-1509)

</div>

---

## 👩‍💻 About Me

Final-year **Computer Science (Honours with Distinction)** student at **Nanyang Technological University, Singapore**, specialising in **Artificial Intelligence** — graduating June 2026.

I work at the intersection of **AI research and production deployment** — from implementing Graph-Mamba architectures and equivariant GNNs for molecular prediction, to deploying LLM evaluation frameworks and real-time inference APIs in production.

- 🔬 **Research:** A+ FYP on antibody-antigen binding affinity prediction · GEPBind paper submitted to **ECCB 2026** (Geneva)
- 🏭 **Industry:** Generative AI Engineer @ **Panasonic R&D** · DevOps Team Lead @ **MISUMI Kaizen** · SWE @ **DXC Technology**
- 🏆 **Hackathons:** Dell InnovateFest Finalist · PSA Code Sprint Finalist · TechFest Top 5 · NGODonate Winner (EasyA × Ripple)
- 📍 Singapore Permanent Resident · Available from June 2026

---

## 🚀 Featured Projects

### 🧬 AAPred — Antibody-Antigen Binding Affinity Prediction
> **Final Year Project, NTU · A+ · Semester GPA 5.00/5.00 · ECCB 2026 Manuscript**

Hybrid **Graph-Mamba** deep learning framework for predicting binding free energy (ΔΔG) between antibody-antigen protein complexes.

- **Architecture:** ESM-2 (650M protein language model) → E(3)-equivariant GatedGCN → Mamba SSM cross-attention fusion → regression head
- **Why equivariant?** Predictions must be identical regardless of molecular rotation/translation — physically required
- **Why Mamba?** O(n) complexity vs O(n²) attention for long protein sequences (500–1000+ residues)
- **Evaluation:** GroupKFold by protein family (prevents data leakage) · 45+ ablations · Pearson **0.507 vs 0.491** baseline
- **Stack:** PyTorch · DGL · ESM-2 · Mamba SSM · Python · NTU HPC

---

### 🤖 ViT + CLIP from Scratch — Vision Transformers & Contrastive Learning
> **Architecture re-implementation in PyTorch · No pretrained weights**

Full implementation of Vision Transformer and CLIP to understand architecture from first principles:

- **Multi-head self-attention:** Q, K, V projections · scaled dot-product · head splitting/merging
- **Patch embedding:** Conv2d stride trick · learnable CLS token · positional embeddings
- **ViT encoder blocks:** Pre-LayerNorm · GELU FFN · residual connections
- **CLIP contrastive loss:** InfoNCE · dual encoder · symmetric image-text loss
- **Stack:** PyTorch · NumPy

---

### 🏠 HDB Resale Price Prediction — Ensemble ML
> **End-to-end ML pipeline · Singapore public housing dataset**

Ensemble of gradient boosting + transformer models for HDB resale price prediction:

- **Models:** LightGBM · XGBoost · CatBoost · FT-Transformer (tabular attention)
- **Features:** MRT proximity · school proximity · floor area · remaining lease · town · storey
- **Approach:** Weighted ensemble via stacking · time-based CV splits (no future data leakage)
- **Stack:** Python · Scikit-learn · LightGBM · XGBoost · CatBoost · PyTorch · Pandas

---

### 📊 Kaggle — Linking Writing Processes to Writing Quality · Top 9.3%
> **Team of 5 · 2,500+ competing teams**

- 80+ behavioural keystroke features engineered from raw typing logs
- Stacked LightGBM/CatBoost/XGBoost ensemble with cross-validation

---

## 🛠️ Tech Stack

**AI / ML / LLMs**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**Backend / Cloud / DevOps**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Data / Analytics**

![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)

---

## 💼 Experience

| Period | Role | Company |
|---|---|---|
| Dec 2025 – Jun 2026 | Generative AI Engineer Intern | Panasonic R&D Centre Singapore |
| Sep – Dec 2025 | DevOps Engineer Intern & Team Lead | MISUMI Kaizen OU Group |
| Jun – Sep 2025 | Full-Stack Engineering Intern | Earth Observatory of Singapore, NTU |
| May – Sep 2025 | Software Engineering Intern | DXC Technology |
| Dec 2024 – Feb 2025 | Deep Learning Engineer Intern | Inspiraz Technology |
| May – Aug 2024 | Embedded Engineering Intern | Schaeffler Hub for Advanced Research |

---

## 📈 GitHub Stats

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=aish-1509&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=aish-1509&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />

</div>

---

## 🏆 Achievements

- 🥇 **Winner** — NGODonate, Best Developer Tooling (EasyA × Ripple Hackathon)
- 🎓 **A+** — Final Year Project · GPA 5.00/5.00 · Nanyang Scholarship
- 🔬 **ECCB 2026** — Peer-reviewed research manuscript accepted (Geneva)
- 🏅 **Top 5 Nationwide** — TechFest Hackathon (AI deepfake detection)
- 🏅 **Top 10 National** — Cactus × Google Hackathon (AI function-calling)
- 🏅 **Finalist** — PSA Code Sprint · Dell InnovateFest · DSTA BrainHack · Build for Good

---

<div align="center">

*"Build it from scratch first. Then use the framework."*

</div>
