---
layout: page
title: Neural Collapse and representation geometry
description: How last-layer features and classifier weights organize, and what breaks when idealized assumptions fail.
img: assets/img/ri_imbalanced.png
importance: 3
category: current
related_publications: true
---

**Neural Collapse** describes how, at the end of training, last-layer features of each class concentrate around their class mean, and the class means together with the classifier weights form a simplex equiangular tight frame (ETF). My Ph.D. work asks what happens to this geometry when idealized training assumptions are broken, and how to repair it.

- **Angle-only representations.** The Spherization Layer {% cite kim2022spherization %} represents features using only angles so that norms carry no information, making angular similarity the sole carrier of information.
- **Non-simplex fixed classifiers.** The Fixed Non-negative Orthogonal Classifier {% cite kim2024fixed %} induces zero-mean Neural Collapse and feature dimension separation, which helps continual and imbalanced learning.
- **Mixed labels and minority collapse.** Mixup under class imbalance causes minority collapse not only through imbalanced singleton labels but also through mixed labels; balancing mixed labels alleviates it {% cite kim2026mixedlabel %}.

My approach follows three steps: identify a model's failure from the perspective of representation learning, verify it theoretically and empirically, and propose a theory-grounded remedy.
