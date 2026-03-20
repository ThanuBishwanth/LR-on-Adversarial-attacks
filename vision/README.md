# Adversarial Machine Learning in Vision

This list prioritizes:
- Top venues (ICLR, NeurIPS, ICML, CVPR, ICCV, S&P)
- High impact (widely cited / foundational)
- Conceptual importance (introduced new attack/defense classes)


- [White-box Attacks](#white-box-attacks)
- [Black-box Attacks](#black-box-attacks)
- [Universal & Physical Attacks](#universal--physical-attacks)
- [Evaluation](#evaluation)
- [Defenses](#defenses)
- [Broken Defenses (Critical Reading)](#broken-defenses-critical-reading)

# ⚔️ Attacks

## White-box Attacks
### 2015
- [Explaining and Harnessing Adversarial Examples](https://arxiv.org/abs/1412.6572) — *ICLR*  
  **FGSM**
### 2016
- [DeepFool](https://arxiv.org/abs/1511.04599) — *CVPR*
- [Adversarial Examples in the Physical World](https://arxiv.org/abs/1607.02533) — *ICLR Workshop*

### 2017
- [Towards Evaluating the Robustness of Neural Networks](https://arxiv.org/abs/1608.04644) — *ICLR*  
  **C&W Attack**
- [Towards Deep Learning Models Resistant to Adversarial Attacks](https://arxiv.org/abs/1706.06083) — *ICLR*  
  **PGD Attack**
- [Ensemble Adversarial Training](https://arxiv.org/abs/1705.07204) — *ICLR*

### 2018
- [Spatially Transformed Adversarial Examples](https://arxiv.org/abs/1801.02612) — *ICLR*
- [Synthesizing Robust Adversarial Examples](https://arxiv.org/abs/1707.07397) — *ICML*

### 2019
- [Adversarial Examples Are Not Bugs, They Are Features](https://arxiv.org/abs/1905.02175) — *NeurIPS*

## Black-box Attacks

### Transfer-based

### 2017
- [Practical Black-Box Attacks](https://arxiv.org/abs/1602.02697) — *AsiaCCS*
- [Transferability of Adversarial Examples](https://arxiv.org/abs/1605.07277) — *arXiv*

### 2019
- [Boosting Adversarial Attacks with Momentum](https://arxiv.org/abs/1710.06081) — *CVPR*

---

### Query-based Attacks

#### Score-based

### 2018
- [NES Attack](https://arxiv.org/abs/1703.03864) — *NeurIPS Workshop*
- [SPSA Attack](https://arxiv.org/abs/1802.05666) — *ICLR Workshop*

### 2020
- [Square Attack](https://arxiv.org/abs/1912.00049) — *ECCV*
- [Bandits with Priors](https://arxiv.org/abs/1807.07978) — *ICLR*


#### Decision-based

### 2018
- [Boundary Attack](https://arxiv.org/abs/1712.04248) — *ICLR*

### 2019
- [HopSkipJump Attack](https://arxiv.org/abs/1904.02144) — *IEEE S&P*


## Universal & Physical Attacks

### 2017
- [Universal Adversarial Perturbations](https://arxiv.org/abs/1610.08401) — *CVPR*

### 2018
- [Adversarial Patch](https://arxiv.org/abs/1712.09665) — *NeurIPS Workshop*
- [Robust Physical Perturbations](https://arxiv.org/abs/1707.08945) — *CVPR*

### 2019
- [Expectation Over Transformation (EOT)](https://arxiv.org/abs/1707.07397) — *ICML*


# Evaluation

### 2020
- [AutoAttack](https://arxiv.org/abs/2003.01690) — *ICML*

### 2021
- [RobustBench](https://arxiv.org/abs/2010.09670) — *NeurIPS*


# Defenses

## Adversarial Training (Core)

### 2017
- [Madry et al. (PGD Training)](https://arxiv.org/abs/1706.06083) — *ICLR*  
  **Status:** Partially Broken

### 2018
- [Ensemble Adversarial Training](https://arxiv.org/abs/1705.07204) — *ICLR*  
  **Status:** Partially Broken

## Robustness vs Accuracy

### 2019
- [Robustness vs Accuracy Tradeoff](https://arxiv.org/abs/1901.08573) — *ICLR*  
  **Status:**  Holds


## Certified Defenses

### 2018
- [Certified Defenses](https://arxiv.org/abs/1801.09344) — *ICLR*  
  **Status:** Holds

### 2019
- [Randomized Smoothing](https://arxiv.org/abs/1902.02918) — *ICML*  
  **Status:**  Holds


## Regularization / Training Tricks

### 2018
- [Label Smoothing & Robustness](https://arxiv.org/abs/1512.00567) — *CVPR*  
  **Status:** Broken

### 2019
- [Input Gradient Regularization](https://arxiv.org/abs/1711.09404) — *NeurIPS*  
  **Status:** Broken

## Efficient Robust Training

### 2020
- [Adversarial Training for Free!](https://arxiv.org/abs/1904.12843) — *NeurIPS*  
  **Status:**  Partially Broken
- [Fast is Better than Free](https://arxiv.org/abs/2001.03994) — *ICLR*  
  **Status:**  Partially Broken


#  Broken Defenses (Critical Reading)

### 2018
- [Obfuscated Gradients Give False Sense of Security](https://arxiv.org/abs/1802.00420) — *ICML*

### 2019
- [Evaluating Robustness Requires Strong Attacks](https://arxiv.org/abs/1902.06705) — *ICML*

## Classic Broken Ideas

- Feature squeezing  
- Randomization 
- Gradient masking  
- Defensive distillation   

# 🧠 Key Insights

### 1. PGD is the baseline adversary
- First-order worst-case attack

### 2. Transferability enables black-box attacks

### 3. Most defenses fail under adaptive attacks

### 4. Certified defenses are the only principled guarantees

### 5. Evaluation (AutoAttack) is critical


#  Benchmarks

- CIFAR-10  
- ImageNet  
- RobustBench  
