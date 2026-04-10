---
title: "Establishing a reproducible baseline for squiggle-space algorithm development"
excerpt: "Poster presented at London Calling 2026."
date: 2026-05-19
collection: posters
---

This poster will be presented at London Calling 2026.

## Abstract

Nanopore sequencing is uniquely positioned for real-time diagnostics at the point-of-care, thanks to continuous signal streaming and compact hardware. Direct analysis of raw ionic current (“squiggles”) preserves the data-rich signal while bypassing the conversion to nucleotide sequences, reducing compute to levels suited for miniaturized devices and enabling portable pathogen detection. Despite this potential, algorithmic development is hindered by a fragmented research landscape, suffering from a lack of reproducibility and a reliance on outdated datasets. 

To address the data bottleneck, we built SquiDBase, a centralized FAIR repository of raw microbial and viral signals with verified ground truth. Ground truth labels are periodically updated using ONT’s latest SUP basecalling models. This ensures that raw signal research remains synchronized with basecalling advancements, allowing the community to leverage accuracy gains immediately. By providing the raw signal, SquiDBase also enables research into microbial epigenetics and methylation dynamics that are otherwise impossible with public data. 

To transition the field from ad-hoc testing to systematic reproducibility, we developed SquiDBench, a Nextflow-based framework for the systematic benchmarking of squiggle-space classification and mapping algorithms. We are currently using this framework to establish a unified baseline by evaluating performance across a broad spectrum of biological complexities to ensure benchmarking is robust and representative of real-world challenges. Our preliminary results highlight a critical performance gap: many tools developed on legacy data underperform on modern R10 signals, indicating that algorithms have not yet adapted to the latest flow cells. Post-publication, SquiDBench will be periodically rerun to monitor the state of the art.