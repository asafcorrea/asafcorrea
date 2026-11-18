---
layout: page
title: "Runasimi-MT: Spanish–Quechua NMT"
description: "Fine-tuning NLLB-200 for low-resource Andean languages."
# img: assets/img/runasimi-preview.jpg
redirect: https://github.com/asafcorrea/Runasimi-MT
github: https://github.com/asafcorrea/Runasimi-MT
importance: 1
category: work
related_publications: true
---

This project explores fine-tuning the NLLB-200-distilled-600M model for Spanish–Quechua machine translation, addressing the lack of accessible MT tools for low-resource Andean languages. The work was published at IEEE INTERCON 2026 and presented orally.

The code and results reported in the paper are available in the GitHub repository. The current repository contains the Spanish–Quechua branch of the broader project, which also explores Spanish–Aymara translation.

**Reported results (paper):** chrF++ = 42.68 for Spanish → Quechua.

**Reproducibility note:** Re-running the pipeline yields slightly different numbers due to non-determinism (fp16, CUDA, library versions) and checkpoint selection. These variations are documented in the repository README.