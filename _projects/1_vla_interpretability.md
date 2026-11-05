---
layout: page
title: Mechanistic interpretability of VLA models
description: What do vision-language-action models represent, and how is their latent space organized?
img: assets/img/ri_neural_collapse.jpg
importance: 1
category: current
related_publications: false
---

Vision-Language-Action (VLA) models map images and instructions to robot actions, but we know little about how their internal representations are organized. I study the **latent space geometry** of VLA models with tools from mechanistic interpretability, such as sparse autoencoders and probing, to answer questions like:

- Which features drive an action decision, and are they grounded in the visual scene or the language instruction?
- How do vision, language, and action representations align, and where does that alignment break?
- Can collapse phenomena known from classification (Neural Collapse, minority collapse) explain failure modes of policies?

The goal is a geometric account of policy behavior that can be used to **diagnose** failures and **shape** representations during training.

<!-- TODO: add figures, project page links, or preprints when available -->
