---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Protein Secretion"
summary: "Our studies of protein secretion began when we turned our attention to the effects of cellular stress and protein misfolding on cellular secretion of critical paracrine proteins, and discovered a unique mechanism of secretion of MANF, a novel ER stress response protein. This study led the way to our research into a more global view of proteins secreted from cardiac myocytes, wherein we examined the cardiac myocyte secretome in response to protein folding stresses."
authors: 
tags: 
categories: 
date: 2011-03-30T17:33:48+02:00
weight: 2

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Smart"
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:

- name: Ischemic Stress-induced Protein Secretion in the Heart 
  url: https://doi.org/10.1016/j.molmed.2010.12.003
  icon_pack: fas
  icon: file-alt 

- name: Mechanism of MANF Secretion
  url: https://doi.org/10.1074/jbc.m112.356345
  icon_pack: fas
  icon: file-alt 

- name: Proteomic Analysis of the Cardiac Myocyte Secretome
  url: https://doi.org/10.1016/j.yjmcc.2020.04.012
  icon_pack: fas
  icon: file-alt 

- name: ER Stress-Induced Secretion of Proteins
  url: https://doi.org/10.3390/cells9092066
  icon_pack: fas
  icon: file-alt


#  icon_pack: fab
#  icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

slides: "/test"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Using GPU programming for short read mapping.

Since the introduction of next generation sequencing technologies like Solexa,
454, and SOLiD the amount of generated data rises with each new technology
upgrade. As the application scenarios especially of the short read techniques
include the re-sequencing of known genomes or sequencing of closely related
strains, new software tools are needed for the fast mapping of sequencing reads
against a reference genome.

Currently, there are several tools available, but most of them are limited
either in speed or accuracy. Limitations in accuracy lead to non detected
mappings, which could become important in post processing steps like SNP
calling. Because of those limitations our goal was to develop an exact and
complete mapping algorithm with equivalent running time compared to available
heuristic implementations.

The result is SARUMAN (Semiglobal Alignment of Short Reads using CUDA and
Needleman-Wunsch). SARUMAN uses a qgram index based filter algorithm followed by
a modified Needleman-Wunsch alignment. To speed up he normally time-consuming
alignment step all alignments are processed on a NVIDIA graphics card to exploit
the massive parallel architecture of new graphics processing units (GPUs). Based
on this technique, depending on the input read length, SARUMAN is able to
process hundreds of thousands of alignments in just a few seconds. As a result
of this alignment strategy SARUMAN not only detects mismatches, but also allows
to detect and handle all insertions and deletions correctly. The mapping
algorithm is exact and complete, it identifies all possible matching positions
for a given error threshold and always returns the optimal local alignment.
