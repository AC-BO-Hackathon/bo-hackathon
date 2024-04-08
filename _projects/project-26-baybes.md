---
number: 26 # leave as-is, maintainers will adjust
title: Multiple-Context Bayesian Optimization
topic: general
team_leads:
  - Joscha Hoche (Merck KGaA / EMD group) @hochej
  - Viola Muning Li (Merck KGaA / EMD group) @vola-m-li
  - Marcel Mueller (Merck KGaA / EMD group and University of Bonn) @marcelmbn, @marcelmuellergdi
  - Rim Rihana (Merck KGaA / EMD group) @RimRihana
  - Tobias Ploetz (Merck KGaA / EMD group) @tobiasploetz

# Comment these lines by prepending the pound symbol (#) to each line to hide these elements
contributors:
  - Martin Fitzner (Merck KGaA / EMD group) @Scienfitz
  - Alexander Hopp (Merck KGaA / EMD group) @AVHopp

github: AC-BO-Hackathon/project-26-multiple-context-bo
youtube_video: <video-id>

---

Traditionally, Bayesian Optimization (BO) is performed for a specific optimization task, e.g., for optimizing a cell culture medium for a specific cell type. 
If the medium is to be optimized for a different cell type, a new, uncorrelated optimization campaign is started.
In multi-context BO (which could also be referred to as transfer learning), the information already available about the medium optimization campaign for the previous cell type is inherited into the new run.

In this project, we aim to investigate _(i)_ the multiple-context performance of BO frameworks on existing benchmarks, _(ii)_ develop new benchmarks for such tasks based on existing data, and _(iii)_ possibly also investigate different ways of incorporating prior knowledge into the model.

Check out our submission post at <url>!

References:
  - [https://github.com/emdgroup/baybe](https://github.com/emdgroup/baybe)

