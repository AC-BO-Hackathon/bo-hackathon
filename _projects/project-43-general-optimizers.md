---
number: 43 # leave as-is, maintainers will adjust
title: Bayesian Optimization for Generality
topic: benchmark-dev
team_leads:
  - Felix Strieth-Kalthoff (University of Toronto) @felix-s-k
  - Mohammad Haddadnia (Harvard University) @mohaddadnia
  - Ella Rajaonson (University of Toronto) @rajaonsonella
  - Stefan Schmid (ETH Zürich) @stefanpschmid
  - Sean Park (University of Toronto) @seanhspark
  - Yeonghun Kang (University of Toronto) @yeonghun1675

# contributors:
#  - 

github: <your-github-repository>
# youtube_video: <your-video-id>

---

This project focuses on benchmarks and algorithms for "generality-oriented" Bayesian Optimization (BO). Usually, BO works by identifying those parameters x that optimize a single objective $f(\textbf{x})$. However, in the natural sciences, problems often involve several related objectives {f<sub>i</sub>(<b>x</b>)}<sub>i=1</sub><sup>n</sup>. Here, the aim is to find parameters $\textbf{x}$ that do well across all these objective functions, without evaluating each f<sub>i</sub>(<b>x</b>) in every iteration. A particularly important example of this is chemical reaction optimization, where the goal is to find reaction conditions that work well across a broad range of substrates. While recent years have seen early examples of generality-oriented BO, our goal is to establish benchmark tasks for generality-oriented BO, evaluate existing strategies, and develop new algorithms for generality-oriented BO (building on ideas from multi-fidelity optimization). 


References:

1. N. H. Angello et al. Science 2022, 378, 399. [https://doi.org/10.1126/science.adc8743](https://doi.org/10.1126/science.adc8743)
2. J. Y. Wang et al. Nature 2024, 626, 1025. [https://doi.org/10.1126/science.adc8743](https://doi.org/10.1038/s41586-024-07021-y)
