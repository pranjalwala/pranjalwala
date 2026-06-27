<div align="center">

<img src="https://avatars.githubusercontent.com/u/203400440?v=4" width="110" style="border-radius: 50%;" />

# Pranjal Wala

[pranjalwala@gmail.com](mailto:pranjalwala@gmail.com) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/pranjal-wala-189470272/) &nbsp;·&nbsp; [Portfolio](https://pranjalwala.github.io) &nbsp;·&nbsp; Miranda House, University of Delhi

</div>

<br>

I'm a mathematics undergraduate. Most of my time lately has gone into evaluation work — building measurement pipelines and benchmark infrastructure around computer vision and print imaging systems.

Two things are running in parallel. At the **CIS Lab** (Columbus, Ohio), I'm finishing ablation and evaluation work for RobustSep, a color separation system built to stay usable when press conditions drift. The manuscript is being prepared with my co-authors. At **DSKC**, I'm building a multilingual retrieval system for Indian government welfare scheme documents — the challenge there is inconsistent source structure, multi-language queries, and clauses where a retrieval error has direct downstream consequences.

---

## Research

**RobustSep** &nbsp;·&nbsp; CIS Lab &nbsp;·&nbsp; *Manuscript in preparation*

Color separation models are calibrated to a specific press state. In production, that state drifts — and most pipelines have no answer for what happens next. The work at CIS Lab was about generating separations that remain feasible across a range of drift conditions rather than just at the calibration point.

I worked on the feasibility projection layer, designed the ablation protocol isolating the stochastic proposer and forward surrogate, and built the stratified evaluation pipeline. I also co-authored the Halftoning Benchmark Specification — the measurement methodology that the two repositories below implement.

> Srivastava†, Ahuja†, Wala†, Lodha. *RobustSep: A Stochastic Candidate-Generation Architecture for Robust, Drift-Aware Expanded-Gamut Color Separation.* &nbsp;(†equal contribution)

---

## Repositories

### [tvi-benchmark](https://github.com/pranjalwala/tvi---benchmark)

TVI — tone value increase — is the tendency of printed dots to reproduce larger than their digital specification. Measuring it accurately is a prerequisite for evaluating any halftoning or separation pipeline; without it, you can't tell whether a method is working or whether the press is just behaving differently than expected.

This package implements the print-and-scan evaluation layer from the Halftoning Benchmark Specification: calibration target generation, scan validation, Murray-Davies and Yule-Nielsen TVI curves, printer transfer function estimation, and confidence intervals across 3 sheets × 3 scans. Hardware-agnostic.

`Python` &nbsp;·&nbsp; `OpenCV` &nbsp;·&nbsp; `CIEDE2000`

---

### [misregistration](https://github.com/pranjalwala/misregistration)

CMYK channel misregistration — where individual ink channels land at slightly different positions on press — degrades both color accuracy and sharpness, and the effect compounds across overprints. Quantifying it requires a dedicated measurement pipeline.

This is Phase 2 of the halftoning benchmark: per-channel displacement estimation, ΔE maps, vector field visualizations, and Pareto analysis tables. It works alongside the TVI module; together they cover the two main process-control failure modes the benchmark specification targets.

`Python` &nbsp;·&nbsp; `OpenCV` &nbsp;·&nbsp; `image processing`

---

### [intel-scene-classification](https://github.com/pranjalwala/intel-scene-classification)

Six-class scene recognition on the Intel dataset. The training is standard. What I was actually trying to answer was whether the GradCAM outputs reflect what a person would identify as discriminative — or whether the model has learned to respond to texture patterns and compression artifacts that happen to correlate with class labels. The answer varies by class, and not always in predictable ways.

`Python` &nbsp;·&nbsp; `TensorFlow` &nbsp;·&nbsp; `GradCAM`

---

### [air-canvas-intent-aware](https://github.com/pranjalwala/air-canvas-intent-aware)

Gesture-based drawing using MediaPipe hand landmark tracking. The non-trivial part is separating intentional drawing strokes from repositioning movements — without that distinction, marks appear on every hand movement and the system stops being usable. The intent segmentation logic is what the "intent-aware" in the name refers to.

`Python` &nbsp;·&nbsp; `OpenCV` &nbsp;·&nbsp; `MediaPipe`

---

### [pranjalwala.github.io](https://pranjalwala.github.io)

Personal site.

---

## Work

| | |
|---|---|
| Research Assistant &nbsp;·&nbsp; CIS Lab, Columbus OH | Aug 2025 – present |
| Research Intern (NLP / RAG) &nbsp;·&nbsp; DSKC | Jun 2026 – present |
| Research Intern &nbsp;·&nbsp; Excelerate | Jul – Aug 2025 |

The Excelerate work involved systematic prompt perturbation — varying instruction structure, few-shot ordering, and constraint phrasing to map where model outputs degrade. The goal was characterizing failure modes rather than improving outputs.

---

## Tools

**Vision / imaging** &nbsp;·&nbsp; Python, OpenCV, MediaPipe, TensorFlow, Keras, NumPy, SciPy, Matplotlib

**Color science** &nbsp;·&nbsp; CIEDE2000, Murray-Davies, Yule-Nielsen, TAC feasibility, halftone dot gain

**NLP / retrieval** &nbsp;·&nbsp; DPR, IndicTrans2, RAG pipeline design

**Other** &nbsp;·&nbsp; Git, LaTeX, Jupyter, MATLAB

---

## Stats

<div align="center">

<img height="150" src="https://github-readme-stats.vercel.app/api?username=pranjalwala&show_icons=true&hide_border=true&count_private=true&theme=default&hide=contribs" />
&nbsp;
<img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=pranjalwala&layout=compact&hide_border=true&theme=default" />

</div>

---

<sub>B.Sc. Mathematics (Honours) · Miranda House, University of Delhi &nbsp;·&nbsp; Editor in Chief, *Mathletics* (2025–26)</sub>

<br>

<div align="center">

[pranjalwala@gmail.com](mailto:pranjalwala@gmail.com) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/pranjal-wala-189470272/)

</div>