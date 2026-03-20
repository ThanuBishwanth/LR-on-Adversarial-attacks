# 🛡️ Adversarial Defenses

Focus:
- Robust training
- Detection
- Certified defenses
- LLM alignment defenses

---

## ⚡ Status Legend

- 🔴 Broken → bypassed by adaptive attacks
- 🟡 Partially Broken → works but limited
- 🟢 Holds → still valid (with assumptions)

---

# 🏋️ Adversarial Training

## 2017
- [Towards Deep Learning Models Resistant to Adversarial Attacks](https://arxiv.org/abs/1706.06083) — *ICLR*  
  → PGD-based training  
  **Status:** 🟡 Partially Broken  
  → Strong but expensive, not fully robust

## 2020
- [Adversarial Training for Free!](https://arxiv.org/abs/1904.12843) — *NeurIPS*  
  → Faster adversarial training  
  **Status:** 🟡 Partially Broken  

---

# 🔍 Detection-based Defenses

## 2017
- [Feature Squeezing](https://arxiv.org/abs/1704.01155) — *NDSS*  
  → Input preprocessing  
  **Status:** 🔴 Broken

---

# 🎭 Gradient Masking

## 2018
- [Obfuscated Gradients Give False Sense of Security](https://arxiv.org/abs/1802.00420) — *ICML*  
  → Breaks many defenses  
  **Status:** ✅ Canonical critique

---

# 📜 Certified Defenses

## 2018
- [Certified Defenses](https://arxiv.org/abs/1801.09344) — *ICLR*  
  → Provable robustness guarantees  
  **Status:** 🟢 Holds (limited scalability)

---

# 🎲 Randomization Defenses

## 2018
- [Mitigating Adversarial Effects via Randomization](https://arxiv.org/abs/1711.01991) — *ICLR*  
  → Random transformations  
  **Status:** 🔴 Broken

---

# 🧠 Preprocessing Defenses

## 2021
- [Pre-processing Defenses for Adversarial Attacks](https://arxiv.org/abs/2101.08909) — *arXiv*  
  → Noise filtering + transformations  
  **Status:** 🟡 Partially Broken  

---

# 🧠 Key Insights

- Most defenses fail under **adaptive attacks**
- Adversarial training remains strongest baseline
- Certified defenses are promising but not scalable
- LLM defenses are still immature
