---
layout: page
title: KronSAE: addressability and steering
description: Ongoing. Experiments largely done; write-up in progress.
importance: 2
category: interpretability
---

Can a Kronecker-factorized SAE place a concept in a predetermined branch (addressability), and does manipulating that branch change generation consistently (steerability)? Controlled experiments on Pythia-410M compare KronSAE with a flat TopK SAE, with and without concept supervision.

Current conclusions: supervision, not structure, produces placement, and placement does not imply steerability. The work also documents negative results and evaluation pitfalls, such as probe-based steering scores that need a fluency gate.
