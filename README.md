# 📚 Adversarial Machine Learning — Research Repository

A structured, research-grade collection of papers on **Adversarial Attacks and Defenses** across:

- 🖼️ Computer Vision  
- 🧠 Large Language Models (LLMs)  
- 🔀 Multimodal Systems  

This repository is designed for **fast lookup, deep study, and research reference**.

---

## ⚡ Quick Navigation

### 📂 Core Sections
- 🖼️ [Vision Attacks](./vision/README.md)
- 🧠 [LLM Attacks (Prompt Injection, Jailbreaks)](./llm/README.md)
- 🛡️ [Defenses (with Broken / Holds status)](./defenses/README.md)

---

## 🧭 How to Use This Repo

### If you're new:
→ Start with **Surveys (below)**

### If you're researching:
- Vision attacks → go to *Vision README*
- Prompt injection / jailbreaks → go to *LLM README*
- Defense methods → go to *Defenses README*

---

## 🔍 Core Surveys (Start Here)

### 2023
- [SoK: Adversarial Machine Learning in the Real World](https://arxiv.org/abs/2202.07237) — *IEEE S&P*

### 2021
- [Adversarial Examples in Deep Learning: A Review](https://arxiv.org/abs/2101.00437) — *ACM Computing Surveys*

### 2018
- [Adversarial Examples: Attacks and Defenses](https://arxiv.org/abs/1712.07107) — *IEEE Access*

---

## 🧠 Taxonomy (How Papers Are Organized)

### 1. By Category
- **Attacks**
- **Defenses**
- **Evaluation**

### 2. By Attack Type
- White-box (gradient access)
- Black-box (no gradients)
- Query-based
- Transfer-based
- Universal attacks
- Physical attacks
- Prompt injection (LLMs)
- Jailbreak attacks

### 3. By Domain
- Vision
- NLP / LLMs
- Multimodal

---

## 🔥 Key Insights (Field Overview)

- Most defenses before 2018 were **broken by adaptive attacks**
- Strongest baseline today:
  → **Adversarial Training (PGD-based)**
- Certified defenses:
  → **Provable but not scalable**
- LLM security:
  → **Still an open problem**

---

## 🛡️ Defense Status Legend

- 🔴 **Broken** → defeated by adaptive attacks  
- 🟡 **Partially Broken** → works but limited  
- 🟢 **Holds** → still valid (under assumptions)  

---

## 📊 Benchmarks & Evaluation (Coming Soon)

Will include:
- AutoAttack
- RobustBench
- Robust accuracy metrics

---

## 📂 Repository Structure
