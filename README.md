# Sudaverse Ecosystem

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
└── SudaTutor             → Fine‑tuned Sudanese‑Arabic LLM
```

Each component plugs into the next to form a complete dialect‑focused AI development pipeline.

---

## 📚 Subsidiary Projects

| Project                            | Role in Ecosystem                  | Key Features                                                                                                | Repository                                                                   |
| ---------------------------------- | ---------------------------------- | ----------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **SudaTutor**                      | Fine‑tuned LLM for Sudanese Arabic | - First Sudanese‑dialect LLM<br>- Tuned on real + synthetic corpora<br>- Strong conversational ability      | [https://github.com/O96a/sudatutor-v6](https://github.com/O96a/sudatutor-v6) |
| **SuData**                         | Normalization & curation pipeline  | - Noise, emoji, PII cleanup<br>- Dialect spelling normalization<br>- Exports JSON/CSV/JSONL datasets        | [https://github.com/O96a/SuData](https://github.com/O96a/SuData)             |
| **Corpus Refinery (LLMCorpusKit)** | High‑scale Arabic corpus cleaning  | - Uses Gemini for deep cleaning<br>- Punctuation/spacing repair<br>- Batch processing for millions of lines | [https://github.com/O96a/LLMCorpusKit](https://github.com/O96a/LLMCorpusKit) |
| **Synthetic Data Generator**       | Generates Sudanese synthetic text  | - Region‑aware dialect simulation<br>- Dialogue, slang, storytelling<br>- Fills data gaps for training      | *(Repo link pending)*                                                        |
| **Sudanese Dialect Benchmark**     | Tokenizer/model evaluator          | - Measures token count efficiency<br>- Slang + dialect coverage<br>- Supports BPE, SP, WordPiece            | *(Repo link pending)*                                                        |

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
                         ▼
                    [ SudaTutor ]
     Fine‑tuning → evaluation → dialect optimization
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
* **Discord ([Server Link](https://discord.gg/3nbnQ9Cy))**

---

## 💛 Built for Sudan. Built for Culture. Built for the Future.

Sudaverse exists to ensure Sudanese Arabic — our language, identity, and stories — continue into the AI era.
