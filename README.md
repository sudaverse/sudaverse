# 🌌 Sudaverse Ecosystem

**Building Sudanese Arabic into the Heart of AI**
An open‑source AI ecosystem dedicated to developing, training, evaluating, and scaling models that understand and generate **Sudanese Arabic dialect** — built for culture, community, and the future.

<p align="center">
  <img src="https://raw.githubusercontent.com/ruvnet/agentic-flow/main/assets/logo.png" width="120" />
</p>

---

## 📑 Quick Navigation

| Section                                     | Description                                     |
| ------------------------------------------- | ----------------------------------------------- |
| [Vision & Mission](#vision--mission)        | Why Sudaverse exists and what drives it         |
| [Ecosystem Overview](#ecosystem-overview)   | The high‑level architecture of the ecosystem    |
| [Subsidiary Projects](#subsidiary-projects) | Breakdown of each core project in the ecosystem |
| [Architecture](#architecture--flow)         | Flow of data → models → evaluation              |
| [Getting Started](#-getting-started)        | Installation, setup, workflows                  |
| [Contribution Guide](#-contribution-guide)  | How to contribute to any Sudaverse component    |
| [Community](#-community--resources)         | Links, contact, and community channels          |

---

## 🎯 Vision & Mission

> *Preserving Sudanese heritage in the age of AI.*

### **Vision**

A digital future where Sudanese Arabic is **fully represented** across AI systems — understood, generated, and respected.

### **Mission**

* Build the largest open‑source **Sudanese Arabic corpus**
* Normalize and clean dialect data using advanced AI tools
* Generate high‑quality synthetic Sudanese text
* Train and fine‑tune state‑of‑the‑art LLMs
* Evaluate models with a Sudanese‑specific benchmark and tokenizer suite
* Create an active community of developers, linguists, and data contributors

---

## 📦 Ecosystem Overview

```
Sudaverse Ecosystem
│
├── SuData                → Data normalization & curation pipeline
├── Corpus Refinery       → High‑scale corpus cleaning using AI
├── Synthetic Data Gen    → Dialect‑aware synthetic data generation
├── Sudanese Benchmark    → Tokenizer & LLM dialect evaluation
└── SudaTutor             → Curriculum‑anchored educational RAG
```

Each component plugs into the next to form a complete dialect‑focused AI development pipeline.

---

## 📚 Subsidiary Projects

### 📁 Repository Index

A quick-access table listing all Sudaverse ecosystem repositories and utilities.

| Project Name                       | Description                                       | Repository Link                                                              |
| ---------------------------------- | ------------------------------------------------- | ---------------------------------------------------------------------------- |
| **SudaTutor**                      | Sudanese Curriculum‑anchored educational RAG      | [https://github.com/O96a/sudatutor-v6](https://github.com/O96a/sudatutor-v6) |
| **SuData**                         | COmplete Data normalization & curation pipeline   | [https://github.com/O96a/SuData](https://github.com/O96a/SuData)             |
| **Corpus Refinery (LLMCorpusKit)** | Cleaning & refining large Arabic corpora          | [https://github.com/O96a/LLMCorpusKit](https://github.com/O96a/LLMCorpusKit) |
| **Synthetic Data Generator**       | Synthetic Sudanese dialect data generation        | *(Link coming soon)*                                                         |
| **Sudanese Dialect Benchmark**     | Tokenizer benchmark optimized for Sudanese Arabic | *(Link coming soon)*                                                         |

---

Below is a comprehensive summary of the core and satellite projects that make up the Sudaverse ecosystem. Each row includes the project's role, quick feature highlights, repository link, and current status.



* 117 subjects across primary & secondary tracks
* Bilingual (Arabic & English), source-grounded answers with citations
* Docker & Vite deployment guides; dev & production instructions | [https://github.com/O96a/sudatutor-v6](https://github.com/O96a/sudatutor-v6) | ✅ Public / Production-ready (pilot)
  | **SuData** | End‑to‑end data normalization & curation pipeline | - Robust cleaning (noise, emojis, HTML)
* Dialect-aware spelling normalization & deduplication
* PII removal, tokenization friendliness
* Exports JSON / JSONL / CSV for model training | [https://github.com/O96a/SuData](https://github.com/O96a/SuData) | ✅ Public / Actively maintained
  | **Corpus Refinery (LLMCorpusKit)** | Large-scale Arabic corpus cleaning & polishing | - Deep-cleaning workflows (sentence repair, punctuation, spacing)
* Integrates with AI APIs for semantic repairs (Gemini / similar)
* Bulk & streaming processors for millions of lines | [https://github.com/O96a/LLMCorpusKit](https://github.com/O96a/LLMCorpusKit) | ✅ Public / Stable
  | **Synthetic Data Generator** | High-quality Sudanese dialect synthetic text generator | - Region-aware dialect simulation (Khartoum, Darfur, East, South)
* Dialogue, scenario, and instruction-style data formats
* Controls for style, register, and sentiment balance | *(Link: coming soon — will be added here)* | ⚠️  Link pending
  | **Sudanese Dialect Benchmark** | Tokenizer & model benchmark tailored to Sudanese Arabic | - Tokenization accuracy & efficiency metrics
* Coverage tests for slang, orthographic variants, elongations
* Evaluates major tokenizers: SentencePiece, BPE, WordPiece, TikToken | *(Link: coming soon — will be added here)* | ⚠️  Link pending
  | **Data Hub (Future)** | Central registry & metadata catalog for datasets | - Dataset manifests, licensing, contributor credits
* Versioning, sample previews, and download links | *(TBD)* | ⚠️ Planned

> Tip: click a repository link to open its README for full install & usage instructions.


---

## 🧬 Architecture & Flow

```
      Raw Sudanese Text (social media, chats, transcripts)
                         │
                         ▼
                    [ SuData ]
    Cleaning → Normalization → PII removal → Deduplication
                         │
                         ▼
             [ Corpus Refinery / LLMCorpusKit ]
 Advanced polishing → punctuation → spacing → structure repair
                         │
         ┌───────────────┴────────────────┐
         ▼                                ▼
 Synthetic Data Generator            Clean Final Corpus
         │                                │
         └───────────────┬────────────────┘
                         │
                         ▼
          [ Sudanese Dialect Benchmark ]
  Tokenization accuracy → segmentation quality → dialect fitness
```

---

## 🚀 Getting Started

### 1. Clone the main ecosystem

```bash
git clone https://github.com/sudaverse/sudaverse.git
cd sudaverse
```

### 2. Install dependencies (per component)

* SuData → `pip install -r sudata/requirements.txt`
* Corpus Refinery → `pip install -r llmcorpusskit/requirements.txt`
* SudaTutor → environment for training

### 3. Run normalization

```bash
python sudata/run.py --input raw/ --output clean/
```

### 4. (Optional) Run advanced corpus refining

```bash
python corpus_refinery/refine.py --input clean/ --output refined/
```

### 5. Generate synthetic data

```bash
python synthetic_gen/generate.py --samples 50000
```

### 6. Train SudaTutor

```bash
python sudatutor/train.py --config configs/base.yaml
```

### 7. Benchmark the result

```bash
python benchmark/run.py --model outputs/sudatutor/
```

---

## 👥 Contribution Guide

We welcome contributions from developers, linguists, researchers, and Sudanese Arabic speakers.

### 1. Fork the repo

### 2. Create a feature branch

```bash
git checkout -b feature/your-feature
```

### 3. Commit your work

```bash
git commit -m "feat: add new normalization rule"
```

### 4. Push and open a PR

```bash
git push origin feature/your-feature
```

Use **Issues** for bugs & proposals, and **Discussions** for planning.

---

## 🌐 Community & Resources

* **Website:** [https://www.sudaverse.com](https://www.sudaverse.com)
* **Email:** [team@sudaverse.com](mailto:team@sudaverse.com)
* **Docs:** See each sub‑repo's `docs/`
* **Twitter/X (coming soon)**
* **Discord (coming soon)**

---

## 💛 Built for Sudan. Built for Culture. Built for the Future.

Sudaverse exists to ensure Sudanese Arabic — our language, identity, and stories — continue into the AI era.
