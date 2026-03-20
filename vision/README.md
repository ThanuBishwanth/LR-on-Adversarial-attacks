# 🖼️ Adversarial Attacks in Computer Vision

Focus: Image classification, CNNs, ViTs, physical-world attacks

---

## ⚡ Quick Navigation
- White-box
- Black-box
- Transfer-based
- Query-based
- Physical attacks
- Universal perturbations

---

# ⚔️ White-box Attacks

## 2015
- [Explaining and Harnessing Adversarial Examples](https://arxiv.org/abs/1412.6572) — *ICLR*  
  `gradient-based`  
  → Introduces FGSM

## 2016
- [DeepFool](https://arxiv.org/abs/1511.04599) — *CVPR*  
  `minimal-perturbation`  
  → Finds smallest perturbation

## 2017
- [Towards Evaluating the Robustness of Neural Networks](https://arxiv.org/abs/1608.04644) — *ICLR*  
  `optimization-based`  
  → C&W attack (breaks many defenses)

## 2017
- [PGD Attack (Madry et al.)](https://arxiv.org/abs/1706.06083) — *ICLR*  
  `first-order`  
  → Strongest first-order adversary baseline

---

# ⚔️ Black-box Attacks

## 2017
- [Practical Black-Box Attacks](https://arxiv.org/abs/1602.02697) — *AsiaCCS*  
  `transfer-based`  
  → Uses surrogate models

## 2018
- [Boundary Attack](https://arxiv.org/abs/1712.04248) — *ICLR*  
  `decision-based`  
  → No gradients needed

---

# ⚔️ Query-based Attacks

## 2020
- [Square Attack](https://arxiv.org/abs/1912.00049) — *ECCV*  
  `score-based`  
  → Efficient query attack

---

# 🔁 Transfer-based Attacks

## 2017
- [Transferability of Adversarial Examples](https://arxiv.org/abs/1605.07277) — *arXiv*  
  → Enables black-box attacks

---

# 🌍 Universal Perturbations

## 2017
- [Universal Adversarial Perturbations](https://arxiv.org/abs/1610.08401) — *CVPR*  
  `input-agnostic`  
  → Single perturbation fools many inputs

---

# 🧱 Physical Attacks

## 2017
- [Adversarial Examples in the Physical World](https://arxiv.org/abs/1607.02533) — *ICLR Workshop*  
  → Real-world robustness failure

## 2018
- [Adversarial Patch](https://arxiv.org/abs/1712.09665) — *NeurIPS Workshop*  
  → Local patch attack

---

# 🧪 Benchmarks

- CIFAR-10
- ImageNet
- MNIST

---

# 🧠 Key Insight

Even simple methods like FGSM and PGD can drastically reduce model accuracy :contentReference[oaicite:0]{index=0}
