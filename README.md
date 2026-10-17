<img src="assets/banner.svg" alt="Xiaoyu (Tom) Chen. CS at the University of Michigan. ML safety and reliability research, computer vision, full-stack." width="100%">

I'm a CS junior at the University of Michigan, transferred from the University of Florida, and I work on making machine learning systems behave predictably when they are put under pressure.
Most of my time goes to research on LLM agent safety and reliability; the rest goes to building and shipping things end to end.

**Open to Summer 2027 software engineering and ML internships.** BS Computer Science, May 2028.

---

## Now

- **LLM agent safety benchmarking** at the TEA Lab, University of Florida ECE, an industry-sponsored collaboration. I own the data pipeline: large-scale evaluation runs on multi-GPU HPC under SLURM, and uncertainty signals (token log-probabilities and entropy) extracted from open-weight models in a single pass.
- **Reliability of coding agents** at OrderLab, University of Michigan EECS. I build the evaluation harness for sandbox policies, testing what a policy actually permits and blocks across matched scenario pairs.
- **Medical dialogue generation**, independent research: discrete latent encoding for more controllable and interpretable generation. Presented at AICCONF 2026.

---

## Featured work

<table>
<tr>
<td width="50%" valign="top">

<a href="https://github.com/Xiaoyu-Ch/hoopalytics"><img src="assets/card-hoopalytics.png" alt="Hoopalytics: a chart of median sort time against record count, showing hand-written merge sort running consistently faster than hand-written heap sort." width="100%"></a>

### [Hoopalytics](https://github.com/Xiaoyu-Ch/hoopalytics)

Merge sort and heap sort, both written from scratch, race each other over a season of NBA box scores, and the app reports who won. A Django backend aggregates per-player averages with pandas and times both sorts on every request; a React front end lets you pick the stat to rank by.

`Python` `Django` `React` `pandas`

</td>
<td width="50%" valign="top">

<a href="https://xiaoyu-ch.github.io"><img src="assets/card-site.png" alt="A wireframe of a personal site with a heading, body text, and three project tiles." width="100%"></a>

### [xiaoyu-ch.github.io](https://xiaoyu-ch.github.io)

My site: research, CV, publications, and project write-ups. Each project page carries a small interactive demo of the idea inside it, including a live merge-sort versus heap-sort race and an Elo-scoring widget, all written by hand in vanilla JS.

`Jekyll` `GitHub Pages` `vanilla JS`

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a href="https://xiaoyu-ch.github.io/projects/muted/"><img src="assets/card-muted.png" alt="A speech bubble showing a learner sentence struck through, and below it the corrected sentence." width="100%"></a>

### [Muted](https://xiaoyu-ch.github.io/projects/muted/)

An AI-first English speaking-practice app, designed, built, and shipped solo, currently in a small beta. The first voice pipeline was too expensive per minute to work for students, so I re-architected it around browser-native speech recognition plus a text model and cut the cost per minute by over 95%. I also found and closed a permission gap that let a client bypass the paid checkout flow.

`Next.js` `Supabase` `Stripe` `Web Speech API`

</td>
<td width="50%" valign="top">

<a href="https://github.com/Xiaoyu-Ch/CLI-image-processing"><img src="assets/card-imaging.png" alt="A strip of images: a source image, then the multiply, overlay, screen, and channel-scaled versions produced by this project." width="100%"></a>

### [TGA image processing](https://github.com/Xiaoyu-Ch/CLI-image-processing)

A small imaging library in C++11 with no dependencies: it parses the TGA binary format by hand, then implements Photoshop-style blend modes, channel arithmetic, and channel split and combine as per-pixel math. The images on that card are its actual output.

`C++11` `binary file I/O` `no dependencies`

</td>
</tr>
<tr>
<td colspan="2" valign="top">

<a href="https://github.com/Xiaoyu-Ch/Minesweepers"><img src="assets/card-minesweeper.png" alt="Two Minesweeper boards: one showing the region opened by a single click, one showing the order the queue opened those tiles." width="49%" align="left"></a>

### [Minesweeper](https://github.com/Xiaoyu-Ch/Minesweepers)

Minesweeper in C++ and SFML, with the classic extras: timer, leaderboard, debug mode, and a configurable board.

The interesting part is the reveal. One click on an empty tile runs a queue-driven flood fill that opens the whole safe region, counting each tile's neighbouring mines as it goes rather than precomputing the board. The right-hand board above shows the order the queue reaches each tile.

`C++` `SFML` `BFS`

</td>
</tr>
</table>

---

## Research

**Research Assistant**, TEA Lab, University of Florida ECE (industry-sponsored collaboration), May 2026 to present
Own the data pipeline for an LLM agent-safety benchmark: single-pass log-probability and entropy extraction from an open-weight model, executed at scale on dual-GPU HPC under SLURM. Tracked down silent GPU memory corruption, a floating-point overflow, and a label-leakage flaw in the data, and built the diagnostics that tell genuine detection apart from a model exploiting how the data was split.

**Undergraduate Researcher**, OrderLab, University of Michigan EECS, July 2026 to present
Evaluation of sandbox policies for coding agents. Built the harness that runs matched pairs of legitimate and cheating scenarios against policies at several strictness levels, so a policy can be judged on what it actually permits and blocks rather than on how it is described.

**Undergraduate Research Assistant**, Computer Vision and Sensing Lab, University of Florida ABE, February to August 2026
Perception pipeline for an autonomous harvesting robot: depth estimation, object detection, and segmentation over field footage, trained and run on university HPC.

**Independent Researcher**, Zhongbo Zhichuang Technologies, September 2025 to present
Discrete latent encoding (VQ-VAE) applied to doctor-patient dialogue for more controllable and interpretable medical dialogue generation.

---

## Publications

- **A Doctor Dialogue Model Based on Vector Quantisation.** AICCONF 2026 (IEEE SMC). Oral presentation.
- **CRetor: A Mandarin Counter-Speech Dataset.** Submitted to ACL Rolling Review, 2025.
- **From Theory to Reality: The Quest for Gravitational Waves.** CONF-CIAP 2024.

Two further papers are in progress, aimed at ACL and OSDI.

---

## Tech

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![vLLM](https://img.shields.io/badge/vLLM-30A14E?style=flat-square) ![YOLO](https://img.shields.io/badge/YOLO-00B8D4?style=flat-square) ![SLURM](https://img.shields.io/badge/SLURM%20%2F%20HPC-4D4D4D?style=flat-square)

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white) ![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)

---

## Elsewhere

[**Website**](https://xiaoyu-ch.github.io) · [**LinkedIn**](https://www.linkedin.com/in/xiaoyu-tom-chen-658251335) · **Email** xiaoyc@umich.edu
