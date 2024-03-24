---
number: 16 # leave as-is, maintainers will adjust
title: BOPE-GPT, Preference Exploration with the curious AI chemist
topic: general
team_leads:
  - Ricardo Valencia Albornoz (University of Edinburgh)

contributors:
  - Sabah Gaznaghi (University of Queensland)

# github: AC-BO-Hackathon/<your-repo-name>
# youtube_video: <your-video-id>

---

When facing a chemistry problem with many outputs, you might want to optimise one output first, like the yield of a reaction, or look for trade-offs for several outputs in a multi-objective fashion. In the latter, objectives/outputs may not be equally important (even across iterations) and very often, a human ranks these outputs to help with future experimentation. 

Here we will use Bayesian optimization with preference exploration, BOPE [1,2] (implemented in Botorch), to guide optimisation in a synthetic multi-output dataset, and we will apply it later to a Fischer-Tropsch synthesis dataset [3,4]. This algorithm selects importance (or utility) of the outputs based on pairwise comparison, and the small twist is that this comparison will be done by a large language model (LLM) instead of a defined utility function [5].

We welcome anyone that wants to contribute or know more about preferential Bayesian optimization, multi-input multi-output datasets and LLM prompting.

References:

1. [BoTorch tutorial for BOPE](https://botorch.org/tutorials/bope).
2. Lin ZJ, Astudillo R, Frazier P, Bakshy E. [Preference Exploration for Efficient Bayesian Optimization with Multiple Outcomes](https://proceedings.mlr.press/v151/jerry-lin22a). In: Proceedings of The 25th International Conference on Artificial Intelligence and Statistics. PMLR. pp. 4235–4258.
3. Lozano-Blanco G, Thybaut JW, Surla K, Galtier P, Marin GB. [Single-Event Microkinetic Model for Fischer−Tropsch Synthesis on Iron-Based Catalysts](https://pubs.acs.org/doi/10.1021/ie071587u). Ind Eng Chem Res 2008;47:5879–5891.
4. Chakkingal A, Janssens P, Poissonnier J, Virginie M, Khodakov AY, et al. [Multi-output machine learning models for kinetic data evaluation : A Fischer–Tropsch synthesis case study](https://www.sciencedirect.com/science/article/pii/S1385894722026754). Chemical Engineering Journal 2022;446:137186.
5. Qin Z, Jagerman R, Hui K, Zhuang H, Wu J, et al. [Large Language Models are Effective Text Rankers with Pairwise Ranking Prompting](https://arxiv.org/abs/2306.17563). DOI: 10.48550/arXiv.2306.17563.
