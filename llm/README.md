# 🧠 Adversarial Attacks & Defenses in Large Language Models (LLMs)

A **high-confidence, research-grade** collection of core papers on adversarial attacks and defenses in LLMs.

Focus:
- Prompt injection
- Jailbreak attacks
- Automated adversarial prompting
- Alignment failures
- Defense mechanisms (with real-world status)

---

## ⚡ Quick Jump

- [Prompt Injection](#prompt-injection)
- [Jailbreak Attacks](#jailbreak-attacks)
- [Automated / Optimization-based Attacks](#automated-attacks)
- [Transfer & Generalization](#transfer--universal-attacks)
- [Defenses](#defenses)
- [Broken Defenses (Critical Reading)](#broken-defenses)

---

# ⚔️ Attacks

---

## 💉 Prompt Injection

### 2023
- [Prompt Injection Attacks Against Large Language Models](https://arxiv.org/abs/2302.12173) — *arXiv*  
  `instruction-override`  
  → Overrides system instructions via crafted input

### 2025
- [Adversarial Attacks on LLM-as-a-Judge Systems](https://paperswithcode.com/paper/adversarial-attacks-on-llm-as-a-judge-systems) — *ACL Workshop*  
  `evaluation-manipulation`  
  → Manipulates LLM evaluators using prompt injection :contentReference[oaicite:0]{index=0}  

---

## 🔓 Jailbreak Attacks

### 2023
- ["Do Anything Now": Jailbreak Prompts Study](https://arxiv.org/abs/2308.03825) — *arXiv*  
  `in-the-wild jailbreaks`  
  → Large-scale analysis of 1,400+ jailbreak prompts :contentReference[oaicite:1]{index=1}  

### 2023
- [MasterKey: Automated Jailbreak](https://arxiv.org/abs/2307.08715) — *arXiv*  
  `automated jailbreak`  
  → Generates jailbreak prompts across models :contentReference[oaicite:2]{index=2}  

---

## 🤖 Automated Attacks

### 2023
- **AutoDAN: Generating Stealthy Jailbreak Prompts** — *arXiv*  
  `gradient-based prompting`  
  → Uses gradients to generate readable adversarial prompts :contentReference[oaicite:3]{index=3}  

### 2023
- **ReNeLLM: Automated Jailbreak Framework** — *arXiv*  
  `LLM-generated attacks`  
  → Uses LLMs to recursively generate stronger jailbreaks :contentReference[oaicite:4]{index=4}  

---

## 🔁 Transfer & Universal Attacks

### 2023–2025
- Universal jailbreak prompts transfer across models  
  → Attack success generalizes across GPT, Claude, LLaMA :contentReference[oaicite:5]{index=5}  

---

## 🧠 Emerging Attack Classes

- Role hijacking (system prompt override)
- Context poisoning (multi-turn attacks)
- Prompt leakage (extract hidden instructions)
- Encoding attacks (Base64, obfuscation)
- Tool misuse (agent-level attacks)

---

# 🛡️ Defenses

---

## 🧱 Prompt-based Defenses

### 2025
- [SecurityLingua: Prompt Compression Defense](https://arxiv.org/abs/2506.12707) — *arXiv*  
  → Extracts true intent of prompts  
  **Status:** 🟡 Partially Effective :contentReference[oaicite:6]{index=6}  

---

## 🧠 Alignment-based Defenses

- RLHF (Reinforcement Learning from Human Feedback)
- Constitutional AI

**Status:** 🔴 Fundamentally Breakable  
→ Jailbreaks bypass alignment consistently :contentReference[oaicite:7]{index=7}  

---

## 🔍 Detection / Guardrails

### 2025
- [Bypassing Prompt Injection Detection](https://aclanthology.org/2025.llmsec-1.8/) — *ACL LLMSEC*  
  → Shows guardrails can be bypassed  
  **Status:** 🔴 Broken :contentReference[oaicite:8]{index=8}  

---

## 🔐 System-level Defenses

- Sandboxing
- Tool isolation
- Multi-model verification

**Status:** 🟡 Promising but incomplete  

---

# 🚨 Broken Defenses

---

## Core Finding (Very Important)

- Guardrails fail under adaptive attacks  
- Detection systems can be bypassed  
- Alignment is not a security guarantee  

### Evidence

- Jailbreak success rates up to ~95% on major models :contentReference[oaicite:9]{index=9}  
- Guardrail evasion can reach near 100% :contentReference[oaicite:10]{index=10}  

---

# 🧠 Key Insights

---

### 1. Unlike vision, attacks are semantic
- No perturbation constraint (L∞, L2)
- Language space = unbounded attack surface

---

### 2. Security ≠ alignment
- RLHF improves behavior
- Does NOT guarantee robustness

---

### 3. Automation is the biggest threat
- Auto-generated jailbreaks outperform humans

---

### 4. Defenses are lagging behind attacks
- Most are reactive, not principled

---

# 📊 Benchmarks & Evaluation

- HarmBench (LLM safety evaluation)
- Jailbreak success rate (ASR)
- Refusal rate
- Transferability across models

---

# 🏁 Takeaway

If you understand:
- Prompt injection
- Jailbreak prompting
- Automated adversarial prompting
- Guardrail failures

→ You understand the **core of LLM adversarial security**

---

# 🚀 Open Problems

- Formal robustness guarantees for LLMs
- Secure system prompts
- Multi-turn attack defenses
- Agent-level security
