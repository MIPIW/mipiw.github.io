---
layout: page
title: Language-specific neurons in translation (M.A. thesis)
description: Seoul National University, 2026. Completed.
importance: 1
category: interpretability
---

Does the language specificity found by LAPE matter causally for a task? On Europarl with Gemma-3-4B-IT, Qwen3-4B, and Llama-3.2-3B-Instruct, I compare neurons selected in place with those from a multi-layer SAE (MLSAE) and analyze sparsity, dimensionality, inter-feature interference, and reconstruction contribution across layers.

Under task-oriented prompts, language-agnostic neurons dominate; suppressing them consistently lowers BLEU in all three models, whereas suppressing language-specific neurons barely changes it. Layer-wise organization is architecture-dependent.
