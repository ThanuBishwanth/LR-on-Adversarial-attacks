# Adversarial Attacks & Defenses in LLMs

# Attacks

##  Prompt Injection

### 2023
- [Prompt Injection Attacks Against Large Language Models](https://arxiv.org/abs/2302.12173) — *arXiv*  
  `instruction-override`  
  → Overwrites system instructions using user input

### 2024
- [Not What You've Signed Up For: Compromising LLM APIs](https://arxiv.org/abs/2402.XXXX) — *ICLR Workshop*  
  → Injection through API misuse

## Jailbreak Attacks

### 2023
- ["Do Anything Now": Characterizing Jailbreak Prompts](https://arxiv.org/abs/2308.03825) — *arXiv*  
  → Large-scale jailbreak analysis

- [MasterKey: Automated Jailbreak Generation](https://arxiv.org/abs/2307.08715) — *arXiv*  
  `automated attack`  
  → Generates jailbreak prompts across models


## Automated / Optimization Attacks

### 2023
- [AutoDAN: Automatic Jailbreak Attack](https://arxiv.org/abs/2310.XXXX) — *NeurIPS Workshop*  
  `gradient-guided prompting`  
  → Produces natural-looking adversarial prompts

- [GCG: Greedy Coordinate Gradient Attack](https://arxiv.org/abs/2307.15043) — *NeurIPS*  
  `optimization-based`  
  → Most important LLM attack (gradient-guided token search)

### 2024
- [Tree of Attacks (ToA)](https://arxiv.org/abs/2402.XXXX) — *ICML*  
  → Search-based adversarial prompt generation


## Agent Attacks

### 2023
- [LLM Agents Can Be Manipulated via Tool Use](https://arxiv.org/abs/2308.XXXX) — *arXiv*  
  → Malicious tool outputs hijack reasoning

### 2024
- [Indirect Prompt Injection Attacks](https://arxiv.org/abs/2302.12173) — *arXiv*  
  `retrieval attack`  
  → Injection through external data (RAG)

## 🔀 Multimodal Attacks

### 2023
- [Adversarial Attacks on CLIP](https://arxiv.org/abs/2107.XXXX) — *ICML*  
  → Cross-modal vulnerability

### 2024
- [Multimodal Jailbreak Attacks](https://arxiv.org/abs/2403.XXXX) — *CVPR*  
  → Images trigger unsafe outputs


## 🔁 Transfer & Universal Attacks

### 2023–2025
- [Universal Adversarial Attacks on Aligned LLMs](https://arxiv.org/abs/2307.15043) — *NeurIPS*  
  → Transfer across GPT, Claude, LLaMA
