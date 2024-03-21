number: 1 # leave as-is, maintainers will adjust
title: Bayesian optimization of likely negative candidates in imbalanced biological datasets
topic: real-world
team_leads:
  - Mayk Caldas Ramos (University of Rochester) @maykcaldas
  - Mehrad Ansari (Acceleration Consortium)     @mehradans92
  - Shane Michtavy (University of Rochester)    @smichtavy

# Comment these lines by prepending the pound symbol (#) to each line to hide these elements
# contributors:
#   - Contributor 1 (Institution 1)
#   - Contributor 2 (Institution 2)

# github: maykcaldas/BO-PU
# youtube_video: <your-video-id>

---

Available peptide datasets often lack class balance due to experimental and technical challenges of the high-throughput screening methods in identifying negative examples, which limits the effectiveness of machine learning (ML) models trained on these datasets. A promising solution involves exclusively leveraging positive examples. This method, known as positive-unlabeled (PU) learning[1], treats all non-positive examples as "unlabeled". The classifier is trained by iteratively identifying likely negative candidates (reliable negatives) within the unlabeled data. In this project, we aim to enhance this approach by incorporating Bayesian Optimization (BO)[2,3] for a more strategic selection of likely negative peptide candidates for different biological tasks, including hemolysis and binding against SHP-2 protein target. Utilizing BO to optimize the peptide sequences selection could significantly improve the method's efficiency and accuracy. This is achieved by systematically exploring the example space to find the optimal PU split for training, offering a strategic advantage over traditional heuristic-based methods.[4]

References:
1- Ansari, Mehrad, and Andrew D. White. 2023. “Learning Peptide Properties with Positive Examples Only.” bioRxiv : The Preprint Server for Biology, June. https://doi.org/10.1101/2023.06.01.543289.
2- Frazier, Peter I. 2018. “A Tutorial on Bayesian Optimization.” arXiv [stat.ML]. arXiv. http://arxiv.org/abs/1807.02811.
3- Shahriari, Bobak, Kevin Swersky, Ziyu Wang, Ryan P. Adams, and Nando de Freitas. 2016. “Taking the Human out of the Loop: A Review of Bayesian Optimization.” Proceedings of the IEEE 104 (1): 148–75. https://doi.org/10.1109/JPROC.2015.2494218.
4- Wang, Ke, and Alexander W. Dowling. 2022. “Bayesian Optimization for Chemical Products and Functional Materials.” Current Opinion in Chemical Engineering 36 (100728): 100728. https://doi.org/10.1016/j.coche.2021.100728.