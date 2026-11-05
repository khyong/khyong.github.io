---
layout: page
title: Disentangled and object-centric representations
description: Consistent symmetry representations, layer-wise factor separation, and slot attention under continual learning.
importance: 4
category: current
related_publications: true
---

A second line of work, carried out with colleagues at the IRR Lab, asks how **factors of variation** should be organized inside a network so that representations generalize compositionally and survive sequential training.

- **Consistent representation of identical transformations.** Symmetry-based VAEs can encode the same semantic transformation differently depending on the sample pair. Mapping latent vectors to a bijective cyclic representation via the Cayley transform, with a fixed-grid codebook, restores this consistency and improves disentanglement and compositional generalization {% cite jung2026impact %}.
- **Layer-centric disentanglement.** Instead of constraining only the latent bottleneck, the Orthogonal Subspaces Projection layer separates factors inside intermediate layers and improves downstream generalization across vision and language tasks {% cite jung2026layercentric %}.
- **Factor-wise homogeneity in slot attention.** Slot Attention organizes its latent space into separated regions that preserve identical factor states across tasks, which is a key mechanism against forgetting in continual object-centric learning {% cite kang2026factorwise %}.

These projects connect to my Neural Collapse work through a shared question: what geometry should a representation space have, and how can training be steered toward it?
