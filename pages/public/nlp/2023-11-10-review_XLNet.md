---
# every file
# static
layout: categorized_post
sidebar: mydoc_sidebar
search: include

title: "Review - XLNet: Generalized Autoregressive Pretraining for Language Understanding."
date: "2023.11.09."
reference: "[link](https://arxiv.org/abs/1906.08237)"
published_year: "2019.01.00."

# variable
categories: ['nlp', 'architectures'] # must be length 2 list
sub_category: [''] # optional, must be a singleton list. if no subcategory filled, it will regareded in listed page in sidebar page
rank: "☆☆☆"
keywords: "generative AR, bidirectional AE, sampled permutation LM, sequence inductive bias, transformer-XL"
summary: "- 


- 
 

- 
"

author_brif: "Yang, z. Dai, Z. et al. "
author_full: "Yang, Z., Dai, Z., Yang, Y., Carbonell, J., Salakhutdinov, R., & Le, Q."
---

<br>

|-|-|
| Author | {{page.author_full}} |
| Published | {{page.published_year}} |
| Reference | {{page.reference}}|
| Keywords | {{page.keywords}} |
| Importance | {{page.rank}} |

---

# Summary

<br>

{{page.summary}}

---

# Background

<br>

- After emerging of BERT(2019) and GPT(2017), the Natural Language Processing(NLP) problem would be divided into two categories per the type of models, which are Natural Language Generation(NLG) with Autoregressive(AR, GPT style) models, and Natural Language Inference(NLI) with Autoencoder(AE, BERT style) models.

- AR model estimates next tokens given the sequences of previous tokens as inputs.

- AE model estimates the exact tokens given the full sequence of tokens except the one we estimate.

---

# Problems, Raising Issues, Clues and Hypothesis

<br>

- AR model cannot utilize the information of the following tokens(so 'unidirectional').

- AE model cannot consider independency between tokens, as it estimate the `[mask]`ed token parallelly.

  -> Moreover, the theoretical issues about how `[mask]`ed tokens affects in fine-tuning processes matters, as `[mask]`ed tokens does not appear in the processes.

- Any model should choose either one, but the authors tried to utilize the benefits of both.

  -> However, the authors thought a LM must use AR type, as sentences have 'inductive bias'. The inductive bias refers to 'the characteristics of sentences which are sequentially proposed', for short.

  -> An model named 'Orderless Nade', which in general is used in Sound Language Processing(SLP), becomes the idea of 'permuation LM'. it esitmate the original sounds with random permutation of input sources when the input is the harmony(or collection) of several sound sources.

---

# Statement

<br>

- So the answers they came out is the 'permutation', in that to perform AR estimation with permuted input tokens, and take average of them as the final results.

- To perform the permutation modeling, it adopts two-stream attention, (1) the query attention and (2) the content attention.

---

# Metrics and Verifications

<br>

here

---

# Discussions

<br>

here

---

# Takeaways
