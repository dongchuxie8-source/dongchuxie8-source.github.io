---
title: 'Emo-LiPO: Listwise Preference Optimization for Fine-Grained Emotion Intensity Control in LLM-based Text-to-Speech'
authors:
  - Yihang Lin
  - Li Zhou
  - Congwei Cao
  - me
  - Xiaoxue Gao
  - Chen Zhang
  - Haizhou Li
date: '2026-05-01T00:00:00Z'
publication_types: ['paper-conference']
publication:
  name: 'Proceedings of the Thirty-Fifth International Joint Conference on Artificial Intelligence'
  short_name: 'IJCAI 2026'
peer_reviewed: true
open_access: true
abstract: >-
  Large language model (LLM)-based text-to-speech (TTS) systems enable prompt-conditioned emotional control but struggle with fine-grained emotion intensity due to the semantic--acoustic gap between text and speech. To address this challenge, we formulate emotion intensity control in LLM-based TTS as a learning-to-rank problem and propose Emo-LiPO, a listwise preference optimization framework that aligns prompt-conditioned speech generation with relative emotion intensity expressed in text. Emo-LiPO explicitly models global intensity ordering within each emotion under fixed transcripts, enabling more faithful and continuous emotional expression. We further construct ESD-plus, a multi-speaker dataset with explicit emotion intensity variations, to support fine-grained emotion modeling and evaluation. Experiments on ESD-plus demonstrate that Emo-LiPO significantly improves emotion accuracy and intensity controllability over both supervised- and DPO-based LLM TTS baselines, with particularly pronounced gains at high intensity levels.
tags:
  - Text-to-Speech
  - Preference Optimization
  - Affective Computing
featured: true
links:
  - type: preprint
    url: https://arxiv.org/abs/2606.13006
hugoblox:
  ids:
    doi: 10.48550/arXiv.2606.13006
image:
  caption: ''
  focal_point: ''
  preview_only: false
---