---
layout: page
title: Imbalanced and continual learning
description: Margin balancing, stable replay, and class-wise interference in the last layer.
importance: 5
category: past
related_publications: true
---

Two settings where representation collapse shows up in practice:

- **Imbalanced learning.** Minority classes suffer from collapsed margins. Asymptotic Midpoint Mixup {% cite kim2024asymptotic %} balances margins while only moderately broadening the feature distribution, and the mixed-label analysis in {% cite kim2026mixedlabel %} explains why Mixup itself can hurt minority classes.
- **Continual learning.** Replay-based methods are unstable when masked logits leak gradients. Revisiting softmax masking with stop-gradient {% cite kim2024revisiting %} reduces class-wise interference in the last-layer features and classifier, mitigating catastrophic forgetting.

Earlier, I also worked on out-of-distribution detection with distance metric learning {% cite yang2020ood %} and dynamic activation functions {% cite maingoc2020dprelu %}.
