---
title: "Same Chart, Different Story: Bias in Vision-Language Chart Interpretation"
collection: publications
category: conferences
permalink: /publication/2026-same-chart-different-story
authors: 'Mizanur Rahman, Huan Wu, Arash Asgari, Enamul Hoque, Laleh Seyyed-Kalantari'
# Date added to the website; the exact proceedings publication date was not supplied.
date: 2026-09-04
venue: 'EMNLP 2026 (Long Paper)'
paperurl: 'https://openreview.net/forum?id=Cb5E3ntNQW'
excerpt: 'ChartBias evaluates bias in vision-language chart interpretation through narrative shift, group hallucination, and preference polarity.'
citation: 'Rahman, M., Wu, H., Asgari, A., Hoque, E., &amp; Seyyed-Kalantari, L. (2026). Same Chart, Different Story: Bias in Vision-Language Chart Interpretation. <i>EMNLP 2026</i>.'
---

Vision-language models (VLMs) are increasingly used to interpret charts and generate natural-language explanations for socially consequential data. However, they may produce different narratives for the same chart when only the referenced social group changes, reinforcing stereotypes and misleading decisions. Despite these risks, no benchmark exists for systematically evaluating bias in chart interpretation across social dimensions.

We introduce **ChartBias**, the first benchmark for auditing bias in VLM-based chart interpretation. ChartBias contains 820 manually curated real-world charts spanning six attributes—race, income, age, religion, immigration status, and gender—yielding 4,319 valid chart–attribute instances and 8,638 paired generations where the chart is fixed and only the group term is swapped.

Across 12 proprietary and open-source VLMs, totaling 155,484 model responses, we find three widespread failure modes: **narrative shift** (same chart, different narratives), **group hallucination** (assigning a chart to a group without evidence), and **preference polarity** (favourable trends often linked to one group).

We further propose a multi-agent mitigation framework that serves as a strong baseline by separating chart-grounded evidence extraction from group-conditioned generation and using a counterfactual judge to verify that group-driven differences are supported by the chart. The framework substantially reduces narrative shift while preserving chart-grounded reasoning. Our findings show that evaluating chart understanding requires measuring not only accuracy, but also fairness and consistency across social groups.
