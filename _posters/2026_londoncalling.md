---
title: "Establishing a reproducible baseline for squiggle-space algorithm development"
excerpt: "Poster presented at Oxford Nanopore Technologies' London Calling 2026."
date: 2026-05-19
collection: posters
image: "<img src='/images/2026_flandersnanoporeday.jpg' style='width: 20vw; min-width: 100px; border: 1px solid grey;'>"
---

<div class="notice--warning" markdown="1">
**August 2026:** the R10 results on this poster are not correct due to a configuration error on my side, the corrected results are considerably better. Final numbers will be in the upcoming paper.
</div>

This poster was presented at Oxford Nanopore Technologies' [London Calling 2026](https://nanoporetech.com/about/events/conferences/lc26).

<a href="/files/2026_flandersnanoporeday.pdf"><img src= "/images/2026_flandersnanoporeday.jpg" style="border: 1px solid grey;"></a>

## Abstract

Nanopore sequencing is uniquely positioned for real-time diagnostics at the point-of-care, thanks to continuous signal streaming and compact hardware. Direct analysis of raw ionic current (“squiggles”) preserves the data-rich signal while bypassing the conversion to nucleotide sequences, reducing compute to levels suited for miniaturized devices and enabling portable pathogen detection. Despite this potential, algorithmic development is hindered by a fragmented research landscape, suffering from a lack of reproducibility and a reliance on outdated datasets. 

To address the data bottleneck, we built SquiDBase, a centralized FAIR repository of raw microbial and viral signals with verified ground truth. Ground truth labels are periodically updated using ONT’s latest SUP basecalling models. This ensures that raw signal research remains synchronized with basecalling advancements, allowing the community to leverage accuracy gains immediately. By providing the raw signal, SquiDBase also enables research into microbial epigenetics and methylation dynamics that are otherwise impossible with public data. 

To transition the field from ad-hoc testing to systematic reproducibility, we developed SquiDBench, a Nextflow-based framework for the systematic benchmarking of squiggle-space classification and mapping algorithms. We are currently using this framework to establish a unified baseline by evaluating performance across a broad spectrum of biological complexities to ensure benchmarking is robust and representative of real-world challenges. Our preliminary results highlight a critical performance gap: many tools developed on legacy data underperform on modern R10 signals, indicating that algorithms have not yet adapted to the latest flow cells. Post-publication, SquiDBench will be periodically rerun to monitor the state of the art.

## Additional information

SquiDBase can be found at <a href="https://squidbase.org/">SquiDBase.org</a>. It was published in January 2026 in [NAR Genomics and Bioinformatics](https://academic.oup.com/nargab/article/8/1/lqaf213/8417709).
