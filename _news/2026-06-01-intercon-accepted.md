---
layout: post
title: "Presentation of Research Paper at INTERCON 2026 (IEEE)"
date: 2026-08-13
inline: false
related_posts: false
description: "Presentation of our work on fine-tuning the 600M NLLB-200 model for low-resource Spanish-Quechua neural machine translation at INTERCON 2026, Trujillo, Peru."
tags: [Natural Language Processing, Machine Translation, Low-Resource Languages, Deep Learning]
---

<div class="row align-items-start my-4">
    <div class="col-12 col-md-4 text-center mb-3 mb-md-0">
        {% include figure.liquid path="assets/img/intercon_photo.jpg" class="img-fluid rounded z-depth-1 mx-auto d-block" style="max-width: 280px; width: 100%; height: auto;" zoomable=true %}
        <div class="caption font-italic mt-2">
            At the IEEE INTERCON 2026 conference venue in Trujillo, Peru.
        </div>
    </div>
    <div class="col-12 col-md-8">
        <p>On August 13, 2026, I presented our research paper titled <strong>"Fine-Tuning a 600M NLLB-200 Model for Low-Resource Spanish-Quechua Machine Translation"</strong> at the <strong>2026 IEEE International Conference on INTERCON (INTERCON 2026)</strong>, held in Trujillo, Peru.</p>
        <p>This research is joint work developed alongside <strong>Dr. Reucher Correa Morocho</strong> from the Department of Computer Science Engineering at the Universidad Nacional de Piura.</p>
        <p>The talk formed part of the main technical program, covering our empirical setup on the SomosNLP 2022 Spanish-Quechua corpus, cross-dataset evaluations on the AmericasNLP benchmark, and a detailed analysis of subword tokenization and corpus quality constraints in Quechua NMT.</p>
    </div>
</div>

### Abstract and Motivation

Quechua represents the most widely spoken indigenous language family in the Americas, with the Peruvian variety alone encompassing over three million speakers. Despite its profound sociolinguistic significance, it remains severely underrepresented in the field of Natural Language Processing (NLP), categorized as a low-resource language due to the extreme scarcity of clean, large-scale, and openly accessible parallel corpora.

This research investigates the efficacy of a reproducible, computationally efficient fine-tuning pipeline utilizing the distilled **600M-parameter variant of Meta's NLLB-200** model. Rather than depending on heavy, industrialized compute clusters, our objective was to rigorously evaluate the performance achievable by a mid-sized architecture when trained end-to-end on raw, uncurated community-generated data—specifically, the **102,000 sentence pairs derived from the SomosNLP 2022 Spanish-Quechua corpus**.

### Key Methodological Contributions and Results

- **In-Domain Evaluation:** When evaluated on the held-out test partition of the SomosNLP dataset, our fully fine-tuned 600M model achieved a **42.68 chrF++** score (and **17.67 BLEU**).
- **Cross-Dataset Generalization:** Evaluated without subsequent adaptation on the official **AmericasNLP 2024 development set**, the model attained **51.88 chrF++**. While numerically surpassing previous published benchmarks—including models scaled at 1.3B and 3.3B parameters—our qualitative error analysis and data provenance evaluation demonstrated that this outcome is substantially influenced by topical and stylistic overlap between datasets rather than pure architectural dominance.
- **Structural Bottlenecks:** The study explicitly underscores that subword tokenization granularity (which fails to align cleanly with Quechua's agglutinative and synthetic morphology) and unmitigated corpus noise constitute the primary bottlenecks restricting translation fidelity in low-resource environments.

<div class="row mt-4 justify-content-center gx-3">
    <div class="col-6 col-md-4 text-center px-2 mb-3 mb-md-0">
        {% include figure.liquid path="assets/img/certificate_receive.jpg" class="img-fluid rounded z-depth-1 mx-auto d-block" style="max-width: 250px; width: 100%; height: auto;" zoomable=true %}
    </div>
    <div class="col-6 col-md-4 text-center px-2">
        {% include figure.liquid path="assets/img/outside_intercon.jpg" class="img-fluid rounded z-depth-1 mx-auto d-block" style="max-width: 250px; width: 100%; height: auto;" zoomable=true %}
    </div>
</div>
<div class="caption text-center font-italic mt-2">
    Left: Receiving the presentation certificate.<br>    
    Right: Alongside Dr. Reucher Correa Morocho and academic peers at the conference.
</div>

### Access to the Manuscript

In compliance with academic publishing guidelines regarding author-hosted preprints and accepted manuscripts, the complete publication text is openly accessible for review:

- **[Download Full Research Paper (PDF)](../../assets/pdf/INTERCON.pdf)** _(Hosted via GitHub Pages)_

### Acknowledgments and Future Directions

I extend my appreciation to the organizing committee of INTERCON 2026, the session participants for their valuable academic inquiries, and my colleague for this successful collaborative effort. Future extensions of this research will focus on implementing rigorous data-cleaning protocols, developing morphology-aware subword tokenization strategies, and scaling evaluations toward truly out-of-domain conversational corpora.

---
