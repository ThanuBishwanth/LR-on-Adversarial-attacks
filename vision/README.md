# 🖼️ Adversarial Machine Learning in Vision — Top 1% Papers

A **high-confidence, minimal-noise** collection of the most important papers in adversarial robustness for computer vision.

This list prioritizes:
- Top venues (ICLR, NeurIPS, ICML, CVPR, ICCV, S&P)
- High impact (widely cited / foundational)
- Conceptual importance (introduced new attack/defense classes)

---

## ⚡ Quick Jump

- [White-box Attacks](#white-box-attacks)
- [Black-box Attacks](#black-box-attacks)
- [Universal & Physical Attacks](#universal--physical-attacks)
- [Evaluation](#evaluation)
- [Defenses](#defenses)
- [Broken Defenses (Critical Reading)](#broken-defenses-critical-reading)

---

# ⚔️ Attacks

---

## White-box Attacks

### 2015
- [Explaining and Harnessing Adversarial Examples](https://arxiv.org/abs/1412.6572) — *ICLR*  
  **FGSM**  
  → First practical gradient-based attack

### 2016
- [DeepFool](https://arxiv.org/abs/1511.04599) — *CVPR*  
  → Minimal perturbation attack (geometry-based)

### 2017
- [Towards Evaluating the Robustness of Neural Networks](https://arxiv.org/abs/1608.04644) — *ICLR*  
  **Carlini & Wagner (C&W)**  
  → Breaks most early defenses

### 2017
- [Towards Deep Learning Models Resistant to Adversarial Attacks](https://arxiv.org/abs/1706.06083) — *ICLR*  
  **PGD Attack**  
  → Gold standard first-order adversary

---

## Black-box Attacks

### 2017
- [Practical Black-Box Attacks against Machine Learning](https://arxiv.org/abs/1602.02697) — *AsiaCCS*  
  → Transfer-based attack framework

### 2018
- [Boundary Attack](https://arxiv.org/abs/1712.04248) — *ICLR*  
  → Decision-based attack (no gradients)

---

## Query-based Attacks

### 2018
- [NES Attack (Natural Evolution Strategies)](https://arxiv.org/abs/1703.03864) — *arXiv / NeurIPS Workshop*  
  → Gradient estimation

### 2020
- [Square Attack](https://arxiv.org/abs/1912.00049) — *ECCV*  
  → Query-efficient black-box attack

---

## Universal & Physical Attacks

### 2017
- [Universal Adversarial Perturbations](https://arxiv.org/abs/1610.08401) — *CVPR*  
  → Input-agnostic attack

### 2017
- [Adversarial Examples in the Physical World](https://arxiv.org/abs/1607.02533) — *ICLR Workshop*  
  → Real-world robustness failure

### 2018
- [Adversarial Patch](https://arxiv.org/abs/1712.09665) — *NeurIPS Workshop*  
  → Localized attack

---

# 🧪 Evaluation

### 2020
- [AutoAttack: Reliable Evaluation of Adversarial Robustness](https://arxiv.org/abs/2003.01690) — *ICML*  
  → Standardized evaluation suite

---

# 🛡️ Defenses

---

## Adversarial Training (Core)

### 2017
- [Towards Deep Learning Models Resistant to Adversarial Attacks](https://arxiv.org/abs/1706.06083) — *ICLR*  
  → Robust optimization (PGD training)  
  **Status:** 🟡 Partially Broken  
  → Strong baseline, still vulnerable

---

## Robustness vs Accuracy Trade-off

### 2019
- [Theoretically Principled Trade-off between Robustness and Accuracy](https://arxiv.org/abs/1901.08573) — *ICLR*  
  → Fundamental limitation  
  **Status:** 🟢 Holds

---

## Certified Defenses

### 2018
- [Certified Defenses via Randomized Smoothing](https://arxiv.org/abs/1801.09344) — *ICLR*  
  → Provable robustness guarantees  
  **Status:** 🟢 Holds (limited scale)

---

## Efficient Training

### 2020
- [Adversarial Training for Free!](https://arxiv.org/abs/1904.12843) — *NeurIPS*  
  → Reduces cost of adversarial training  
  **Status:** 🟡 Partially Broken

---

# 🚨 Broken Defenses (Critical Reading)

These papers are **essential** — they explain why most defenses fail.

### 2018
- [Obfuscated Gradients Give False Sense of Security](https://arxiv.org/abs/1802.00420) — *ICML*  
  → Shows most defenses rely on gradient masking

---

## Examples of Broken Ideas

- Feature squeezing → 🔴 Broken  
- Randomization defenses → 🔴 Broken  
- Gradient masking → 🔴 Illusion of robustness  

---

# 🧠 Key Insights

### 1. Strong attacks are simple
- PGD ≈ worst-case first-order attack

### 2. Most defenses fail
- Especially under **adaptive attacks**

### 3. Only reliable defenses:
- Adversarial training (costly)
- Certified defenses (limited)

### 4. Evaluation matters more than method
- AutoAttack is standard

---

# 📊 Benchmarks

- CIFAR-10
- ImageNet
- RobustBench (leaderboard)

---

# 🏁 Takeaway

If you understand:
- **FGSM → PGD → C&W**
- **Transfer & query attacks**
- **Adversarial training**
- **Obfuscated gradients paper**

→ You understand **80% of the field**
