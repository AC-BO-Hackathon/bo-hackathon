---
number: 11 # leave as-is, maintainers will adjust
title: BlendDS - An intuitive specification of the design space for blends of components
topic: general
team_leads:
  - Daniele Ongari (SYENSQO)
  - Alessio Tamburro (SYENSQO)

github: [danieleongari/blends](https://github.com/danieleongari/blends)
youtube_video: [HASa3tFLZoI](https://www.youtube.com/watch?v=HASa3tFLZoI)

---

We will design "BlenDS" a framework for an intuitive specification of the design space for blends of components. 
The framework will be based on the following concepts: there are two entities, the "Component" and the "Blend"; 
they can be recursively combined in a tree-like structure to create the final tree branching from the root blend. 
The root blend will have all the constraints needed to generate trials of a design space. 
The scope of this project is to develop an API, use Large Language Models to traslate human written specifications 
into a root blend, and finally generate valid samples from the blend space that can be then used as a designed experiment.
We will compare this easy-to-use approach (whose generation of samples resembles a model-agnostic space filling design),
with the classical Mixture Design DOE. 

References:
- [NIST, Engineering Statistics Handbook: 5.5.4 What is a Mixture Design?](https://www.itl.nist.gov/div898/handbook/pri/section5/pri54.htm)
