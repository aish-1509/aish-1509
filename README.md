<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=6C63FF&center=true&vCenter=true&width=700&lines=Aishwarya+Anand;AI+%2F+ML+Engineer+%7C+Computer+Vision+%7C+GenAI;NTU+Computer+Science+%E2%80%94+AI+Specialisation;Building+production+AI+systems+from+research+to+deployment" alt="Typing SVG" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/aishwarya-anand-b963661b3)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://aishwarya-portfolio-tau.vercel.app)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aish0021@e.ntu.edu.sg)

</div>

---

## 👩‍💻 About Me

Final-year **Computer Science (Honours with Distinction)** at **Nanyang Technological University, Singapore**, specialising in **Artificial Intelligence** — graduating June 2026. Nanyang Scholar · NTU-University Scholars Programme.

I build end-to-end AI systems — from implementing Graph-Mamba and equivariant GNNs for molecular research, to multi-task computer vision pipelines, to production LLM evaluation frameworks and agentic workflows.

- 🔬 **Research:** A+ FYP · Hybrid Graph-Mamba for protein binding affinity · GEPBind paper at **ECCB 2026** (Geneva)
- 🏭 **Industry:** Generative AI Engineer @ **Panasonic R&D** · DevOps Lead @ **MISUMI** · SWE @ **DXC** · CV Intern @ **Inspiraz**
- 🏆 **Hackathons:** NGODonate Winner · TechFest Top 5 Nationwide · PSA Finalist · Dell InnovateFest Finalist
- 📍 Singapore PR · Available June 2026

---

## 🚀 Featured Projects

### 🧬 AAPred — Antibody-Antigen Binding Affinity Prediction
> **NTU Final Year Project · A+ · GPA 5.00 · ECCB 2026 Peer-Reviewed Manuscript**

Hybrid **Graph-Mamba** framework predicting ΔΔG (binding free energy change) between antibody-antigen protein complexes — enabling computational pre-screening of antibody drug candidates.

| Component | Detail |
|---|---|
| Sequence encoder | ESM-2 (650M protein language model, Meta AI) |
| Structure encoder | E(3)-equivariant GatedGCN — invariant to molecular rotation/translation |
| Fusion layer | Mamba SSM cross-attention — O(n) vs O(n²) attention for long sequences |
| Evaluation | GroupKFold by protein family — prevents identity leakage |
| Result | **Pearson 0.507 vs 0.491 baseline** · 45+ ablations |

`PyTorch` `DGL` `ESM-2` `Mamba` `Python` `HPC`

---

### 👁️ Person Attribute Recognition (PAR) — Multi-Task Computer Vision
> **Take-home assignment · Cynapse AI · Test macro-F1: 0.8216**

Multi-task deep learning pipeline predicting **6 pedestrian attributes simultaneously** from a single shared backbone — Age, Headgear, Gender, Glasses, Upper-body colour, Lower-body colour.

**Key engineering decisions:**
- **Architecture:** ConvNeXt-Small backbone (50M params, ImageNet-pretrained via `timm`) + 6 independent linear classification heads — one model, not six
- **Identity leakage prevention:** GroupShuffleSplit with 101-seed Monte Carlo search on Market-1501 re-ID naming convention (same person across multiple crops)
- **469:1 class imbalance:** Tri-axis strategy — inverse-square-root class weights + **Focal Loss (γ=2)** + homoscedastic uncertainty weighting (Kendall et al. 2018 `log_var` parameters)
- **Colour-safe augmentation:** Deliberately excluded hue/saturation shifts — UB/LB clothing colour are prediction targets
- **Pedestrian aspect ratio:** 256×128 (not square) — preserves body proportions
- **Training:** AdamW · ReduceLROnPlateau · mixed precision · early stopping (patience=5)
- **Result:** Test mean macro-F1 **0.8216** on 7,021 held-out crops from ~70,000 pedestrian images

`PyTorch` `ConvNeXt` `timm` `Focal Loss` `Albumentations` `Python`

---

### 🤖 Vision Transformer (ViT) + CLIP — From Scratch
> **Architecture re-implementation in PyTorch · Zero pretrained weights**

Built to understand modern vision architectures from first principles:

- **Scaled dot-product attention:** `Attention(Q,K,V) = softmax(QKᵀ/√d_k)·V` — written from scratch
- **Multi-head attention:** H parallel heads · head splitting/merging · output projection
- **Patch embedding:** Conv2d stride trick · learnable [CLS] token · positional embeddings
- **ViT encoder blocks:** Pre-LayerNorm · GELU FFN · residual connections · 5.7M params
- **CLIP contrastive loss:** InfoNCE · dual image+text encoder · symmetric loss · temperature scaling
- All tests pass with verified shapes and forward passes

`PyTorch` `NumPy`

---

### 🐦 BirdCLEF Audio Classification — Kaggle ML Competition
> **SC4000 NTU · Team competition · Acoustic species identification**

ML pipeline for identifying bird species from audio recordings in the BirdCLEF Kaggle competition:

- Audio preprocessing: STFT spectrograms · MFCC features · data augmentation (SpecAugment)
- Classification models: CNN on mel-spectrograms · ensemble approaches
- Handling long-tail distribution of species occurrences

`Python` `Librosa` `PyTorch` `Scikit-learn` `Kaggle`

---

### 🤖 MDP — Autonomous Robot Computer Vision
> **NTU Multidisciplinary Design Project · Group 38**

Computer vision and image recognition system for an autonomous robot navigation task:

- Real-time object detection and classification from robot-mounted camera
- Image processing pipeline: preprocessing → detection → classification → communication to robot controller
- Integrated with Raspberry Pi control system and Arduino hardware

`Python` `OpenCV` `PyTorch` `Raspberry Pi`

---

### 🏠 HDB Resale Price Prediction — Tabular ML Ensemble
> **End-to-end ML pipeline · Singapore public housing market**

Ensemble of tree-based models + tabular transformer for HDB resale price prediction:

- **Models:** LightGBM · XGBoost · CatBoost · **FT-Transformer** (captures non-linear feature interactions GBMs miss)
- **Features:** MRT proximity · school proximity · floor area · remaining lease · storey · flat type
- **Evaluation:** Time-based CV splits (prevents future data leakage) · RMSE · MAE · R²
- **Ensemble:** Weighted average via stacking meta-learner

`Python` `LightGBM` `XGBoost` `CatBoost` `PyTorch` `Pandas`

---

### 💬 Sentiment Analysis & NLP Projects
> **NLP pipeline collection**

Collection of NLP experiments including sentiment classification, text preprocessing, and language modelling tasks.

`Python` `NLTK` `Transformers` `scikit-learn`

---

### 🌐 Portfolio Website
> **[aishwarya-portfolio-tau.vercel.app](https://aishwarya-portfolio-tau.vercel.app)**

Dynamic personal portfolio showcasing projects, experience, and skills. Built with modern web technologies, deployed on Vercel.

`HTML` `CSS` `JavaScript`

---

## 🛠️ Tech Stack

**AI / ML / GenAI**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

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
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**Data / Analytics**

![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)

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

## 🏆 Awards & Recognition

| Award | Competition |
|---|---|
| 🥇 Winner — Best Developer Tooling | NGODonate · EasyA × Ripple Hackathon |
| 🎓 A+ FYP · GPA 5.00/5.00 | NTU · Nanyang Scholarship |
| 📄 Peer-reviewed manuscript | ECCB 2026, Geneva |
| 🏅 Top 5 Nationwide | TechFest Hackathon — AI deepfake detection |
| 🏅 Top 10 National | Cactus × Google Global Hackathon |
| 🏅 Finalist | PSA Code Sprint · Dell InnovateFest · DSTA BrainHack · Build for Good (OGP) |

---

## 📈 GitHub Stats

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=aish-1509&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=aish-1509&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />

</div>

---

<div align="center">
<i>"Build it from scratch first. Then use the framework."</i>
</div>
