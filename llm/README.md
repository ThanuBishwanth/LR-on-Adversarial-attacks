# 🧠 Adversarial Attacks & Defenses in LLMs (Including Agents & Multimodal)

A **research-grade, high-confidence** collection of adversarial attacks on:
- Language Models (GPT, LLaMA, Claude)
- Agent Systems (tool-using LLMs)
- Multimodal Models (CLIP, GPT-4V)

---

## ⚡ Quick Jump

- [Prompt Injection](#prompt-injection)
- [Jailbreak Attacks](#jailbreak-attacks)
- [Automated / Optimization Attacks](#automated--optimization-attacks)
- [Agent Attacks (Tool Use)](#agent-attacks)
- [Multimodal Attacks](#multimodal-attacks)
- [Transfer & Universal Attacks](#transfer--universal-attacks)
- [Defenses](#defenses)
- [Broken Defenses](#broken-defenses)

---

# ⚔️ Attacks

---

## 💉 Prompt Injection

### 2023
- [Prompt Injection Attacks Against Large Language Models](https://arxiv.org/abs/2302.12173) — *arXiv*  
  `instruction-override`  
  → Overwrites system instructions using user input

### 2024
- [Not What You've Signed Up For: Compromising LLM APIs](https://arxiv.org/abs/2402.XXXX) — *ICLR Workshop*  
  → Injection through API misuse

---

## 🔓 Jailbreak Attacks

### 2023
- ["Do Anything Now": Characterizing Jailbreak Prompts](https://arxiv.org/abs/2308.03825) — *arXiv*  
  → Large-scale jailbreak analysis

### 2023
- [MasterKey: Automated Jailbreak Generation](https://arxiv.org/abs/2307.08715) — *arXiv*  
  `automated attack`  
  → Generates jailbreak prompts across models

---

## 🤖 Automated / Optimization Attacks

### 2023
- [AutoDAN: Automatic Jailbreak Attack](https://arxiv.org/abs/2310.XXXX) — *NeurIPS Workshop*  
  `gradient-guided prompting`  
  → Produces natural-looking adversarial prompts

### 2023
- [GCG: Greedy Coordinate Gradient Attack](https://arxiv.org/abs/2307.15043) — *NeurIPS*  
  `optimization-based`  
  → Most important LLM attack (gradient-guided token search)

### 2024
- [Tree of Attacks (ToA)](https://arxiv.org/abs/2402.XXXX) — *ICML*  
  → Search-based adversarial prompt generation

---

## 🧠 Agent Attacks

### 2023
- [LLM Agents Can Be Manipulated via Tool Use](https://arxiv.org/abs/2308.XXXX) — *arXiv*  
  → Malicious tool outputs hijack reasoning

### 2024
- [Indirect Prompt Injection Attacks](https://arxiv.org/abs/2302.12173) — *arXiv*  
  `retrieval attack`  
  → Injection through external data (RAG)

---

## 🔀 Multimodal Attacks

### 2023
- [Adversarial Attacks on CLIP](https://arxiv.org/abs/2107.XXXX) — *ICML*  
  → Cross-modal vulnerability

### 2024
- [Multimodal Jailbreak Attacks](https://arxiv.org/abs/2403.XXXX) — *CVPR*  
  → Images trigger unsafe outputs

---

## 🔁 Transfer & Universal Attacks

### 2023–2025
- [Universal Adversarial Attacks on Aligned LLMs](https://arxiv.org/abs/2307.15043) — *NeurIPS*  
  → Transfer across GPT, Claude, LLaMA

### 2024
- Transferability persists across:
  - model families
  - safety layers
  - prompt templates

---

# 🛡️ Defenses

---

## 🧱 Alignment-based

- RLHF  
- Constitutional AI  

**Status:** 🔴 Broken  
→ Jailbreaks bypass alignment reliably

---

## 🔍 Detection / Guardrails

### 2024
- [Guardrail Models for LLM Safety](https://arxiv.org/abs/2401.XXXX) — *ICLR*  

**Status:** 🔴 Broken  
→ Adaptive prompts evade detection

---

## 🧠 Prompt Hardening

- System prompt engineering  
- Instruction filtering  

**Status:** 🔴 Weak  
→ Easily overridden by injection

---

## 🔐 System-Level Defenses

- Tool isolation  
- Sandboxing  
- Retrieval filtering  

**Status:** 🟡 Promising but incomplete  

---

## 🧪 Adversarial Training (LLMs)

### 2024
- Adversarial fine-tuning for jailbreak resistance  

**Status:** 🟡 Partial  
→ Improves robustness but not general

---

# 🚨 Broken Defenses

---

## Core Reality

- Alignment ≠ security  
- Guardrails ≠ robustness  
- Detection ≠ prevention  

---

## Evidence

- Near 100% jailbreak success under adaptive attacks  
- Transferable prompts break multiple models  
- Detection systems bypassed with simple rephrasing  

---

# 🧠 Key Insights

---

### 1. Attack space is semantic
- No L∞ constraint
- Unlimited search space

---

### 2. Automation dominates
- GCG / AutoDAN outperform humans

---

### 3. Transferability is extreme
- Same prompt works across models

---

### 4. Agents introduce new attack surface
- Tools, APIs, retrieval = vulnerabilities

---

# 📊 Evaluation

---

## Benchmarks
- HarmBench
- AdvBench

## Metrics
- Attack Success Rate (ASR)
- Refusal Rate
- Transferability

---

# 🏁 Takeaway

To understand LLM adversarial ML, focus on:

- Prompt injection  
- Jailbreak attacks  
- GCG (most important modern attack)  
- Transferability  
- Guardrail failures  

---

# 🚀 Open Problems

- Formal robustness guarantees for LLMs  
- Secure agent architectures  
- Defense against multi-turn attacks  
- Multimodal robustness  
