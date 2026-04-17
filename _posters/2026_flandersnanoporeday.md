---
title: "Establishing a reproducible baseline for squiggle-space algorithm development"
excerpt: "Poster presented at the Flanders Nanopore Day 2026."
date: 2026-04-17
collection: posters
image: "<img src='/images/2026_flandersnanoporeday.jpg' style='width: 20vw; min-width: 100px; border: 1px solid grey;'>"
---

This poster will be presented at the [Flanders Nanopore Day](https://nanoporeflanders.be/).

<a href="/files/2026_flandersnanoporeday.pdf"><img src= "/images/2026_flandersnanoporeday.jpg" style="border: 1px solid grey;"></a>

## Abstract

Nanopore sequencing enables real-time, point-of-care diagnostics through continuous signal streaming and compact devices. However, the high computational cost of basecalling remains a major hurdle. Raw signal-based algorithms bypass this issue, but their progress is hindered by a fragmented research landscape, poor reproducibility, and outdated datasets. 

To address the data bottleneck, we built SquiDBase, a FAIR repository of raw microbial and viral signals with verified ground truth. Periodic updates using ONT’s latest SUP models keep raw signal research aligned with basecalling advancements. SquiDBase also enables microbial epigenetics research by providing the raw signal. 

To introduce systematic reproducibility, we built SquiDBench, a Nextflow-based benchmarking framework for squiggle-space methods. Initial results reveal a critical performance gap: many tools trained on legacy data underperform on modern R10 signals, underscoring the need for benchmarks to advance the field.

## Additional information

SquiDBase can be found at <a href="https://squidbase.org/">SquiDBase.org</a>. It was published in January 2026 in [NAR Genomics and Bioinformatics](https://academic.oup.com/nargab/article/8/1/lqaf213/8417709).