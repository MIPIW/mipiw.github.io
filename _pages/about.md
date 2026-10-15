---
layout: about
title: about
permalink: /
subtitle: Ph.D. student, Department of Linguistics, Seoul National University

profile:
  align: right
  more_info: >
    <p>Computational Linguistics (CL_NLP) Lab</p>
    <p>Seoul National University</p>
    <p>Seoul, South Korea</p>

selected_papers: true
social: true

announcements:
  enabled: true
  scrollable: true
  limit: 5
---

I am a Ph.D. student in Linguistics at Seoul National University, advised by [Prof. Hyopil Shin](https://nlp.snu.ac.kr). I work on the interpretability of language models, with a focus on multilingual representations, sparse autoencoders (SAEs), and evaluation. My stance is to use interpretability results to *optimize* models, not only to describe them, and to bring problems from linguistics into the model's interior.

**Master's thesis.** *Investigating the Contribution of Language-Specific Neurons to the Translation Task* (M.A., SNU, 2026). LAPE-identified language-specific neurons are widely assumed to matter for multilingual ability, but it is unclear whether they contribute causally to a downstream task. Using task-oriented translation prompts and a multi-layer sparse autoencoder on Gemma-3-4B-IT, Qwen3-4B, and Llama-3.2-3B-Instruct, I find that language-agnostic neurons dominate the detected feature space and suppressing them consistently degrades translation, while suppressing language-specific neurons has little effect. The layer-wise organization depends on the architecture.

**Current directions.** (1) Structured sparse autoencoders (KronSAE) as an interface for locating and steering concepts; (2) how language-specific neurons map onto SAE latents, and how layer-wise information storage relates to layer importance; (3) English-centered intermediate representations in multilingual LLMs and what they lose; (4) memorization versus generalization; (5) evaluation of LLMs, including verbosity, confidence, and feedback on L2 writing. See [research](/projects/) for details.
