# 🖼️ Adversarial Machine Learning in Vision — Top Papers (~50 Core Works)

A **high-confidence, minimal-noise** collection of the most important papers in adversarial robustness.

---

## ⚡ Quick Jump
- White-box
- Black-box (Transfer + Query)
- Universal & Physical
- Evaluation
- Defenses
- Broken Defenses

---

# ⚔️ Attacks

---

## White-box Attacks

### 2015
- Explaining and Harnessing Adversarial Examples (FGSM) — ICLR  

### 2016
- DeepFool — CVPR  

### 2017
- Carlini & Wagner Attack — ICLR  
- PGD Attack (Madry et al.) — ICLR  

### 2018
- Basic Iterative Method (Kurakin et al.) — ICLR Workshop  
- Momentum Iterative FGSM (MI-FGSM) — CVPR  

### 2019
- Diverse Input Method (DIM) — CVPR  
- Translation-Invariant Attacks (TI-FGSM) — CVPR  

### 2020
- Expectation Over Transformation (EOT) — ICML  

---

## Black-box Attacks

### Transfer-based

#### 2017
- Practical Black-Box Attacks — AsiaCCS  

#### 2018–2020 (Transfer Improvements)
- MI-FGSM (transfer boost) — CVPR  
- DIM — CVPR  
- TI-FGSM — CVPR  

---

### Query-based

#### Score-based

### 2018
- NES Attack — NeurIPS Workshop  

### 2018
- SPSA Attack — ICML  

### 2020
- Square Attack — ECCV  

---

#### Decision-based

### 2018
- Boundary Attack — ICLR  

### 2019
- HopSkipJump Attack — IEEE S&P  

---

## Universal & Physical Attacks

### 2017
- Universal Adversarial Perturbations — CVPR  
- Physical World Attacks — ICLR Workshop  

### 2018
- Adversarial Patch — NeurIPS Workshop  
- Spatial Transform Attack — ICLR  

### 2019
- Expectation Over Transformation (physical robustness) — ICML  

---

## Advanced Attack Directions

### 2020–2022
- AutoAttack — ICML  
- Fast Adaptive Boundary Attack — CVPR  

---

# 🧪 Evaluation

### 2020
- AutoAttack — ICML  

### 2021
- RobustBench — NeurIPS  

---

# 🛡️ Defenses

---

## Adversarial Training (Core)

### 2017
- Madry et al. (PGD Training) — ICLR  
  **Status:** 🟡

### 2018
- Ensemble Adversarial Training — ICLR  

### 2019
- TRADES — ICML  
  **Status:** 🟡 (best trade-off method)

---

## Efficiency Improvements

### 2020
- Free Adversarial Training — NeurIPS  
- Fast Adversarial Training — ICLR  

---

## Certified Defenses

### 2018
- Certified Defenses (Kolter & Wong) — ICLR  
  **Status:** 🟢  

### 2019
- Randomized Smoothing — ICML  
  **Status:** 🟢  

---

## Preprocessing / Detection

### 2017
- Feature Squeezing — NDSS  
  **Status:** 🔴  

### 2018
- Input Transformations — ICLR  
  **Status:** 🔴  

---

# 🚨 Broken Defenses (Critical Reading)

### 2018
- Obfuscated Gradients — ICML  

### 2019
- Adaptive Attacks on Defenses — ICML  

---

## Commonly Broken

- Gradient masking → 🔴  
- Randomization → 🔴  
- Preprocessing → 🔴  

---

# 🧠 Key Insights

### 1. Attack hierarchy
FGSM → PGD → C&W → AutoAttack

### 2. Strongest attacks today
- PGD (training)
- AutoAttack (evaluation)

### 3. Only reliable defenses
- Adversarial training
- Certified defenses

### 4. Biggest mistake
- Not evaluating with adaptive attacks

---

# 📊 Benchmarks

- CIFAR-10  
- ImageNet  
- RobustBench  

---

# 🏁 Takeaway

If you understand:

- FGSM, PGD, C&W  
- Transfer + Query attacks  
- AutoAttack  
- TRADES  
- Obfuscated Gradients  

→ You understand **core adversarial ML in vision**
