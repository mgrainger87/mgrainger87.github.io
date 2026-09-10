---
title: "Research"
permalink: /research/
---

Learning from finite observations necessarily requires inductive inference: the data constrain the learned system, but do not uniquely determine how it should behave beyond the observations. Modern machine learning selects among these possibilities through powerful inductive biases in architecture, loss, regularization, and optimization, but those same choices also shape which possible explanations for the data appear simple, stable, or natural under the geometry induced by the learning procedure. In that sense, the learning procedure can “bend the ruler” by which its own generalization is evaluated: changing the representation can also change the geometry through which differences among possible generalizations are measured, so that improvement in the learned model space need not correspond to improvement in the semantic space we actually care about.

My research asks what learning could look like if that evaluative structure were made explicit and held fixed independently of the candidate model or representation. Given a geometry of admissible variation and a set of consequences that must be preserved, I am studying how a learner can construct an **effective theory** from finite evidence: one that preserves the distinctions needed for those consequences while allowing irrelevant distinctions to be forgotten.

This requires more than learning useful representations that make prediction or optimization easier. It involves learning **effective objects**: consequence-relative statistical interfaces that define boundaries across which fine-grained distinctions need no longer remain explicit to the rest of the system. An effective object identifies underlying possibilities that may safely be treated as equivalent for specified uses, while preserving both their outward responses and a conditional distribution over the unresolved possibilities beneath the interface. Its adequacy is therefore judged by what it allows the system to predict, how it responds to perturbations, which distributions it can generate, how it composes with other effective objects, and whether unresolved detail can be lawfully refined when needed—not simply by whether its coordinates are compact or its training loss is low.

I am especially interested in how such objects can be constructed from finite evidence, revised when new perturbations or uses expose missing structure, composed into larger effective theories, and recursively reused so that what has already been learned makes subsequent learning problems smaller.

My interests sit at the intersection of:

- **Generalization and inductive bias:** how finite observations constrain—but do not uniquely determine—behavior away from the observed data; how losses, architectures, regularization, optimization, and representation geometry shape that extension; and how the assumptions governing generalization can be kept distinct from the candidate representations judged under them.

- **Generative and probabilistic modeling:** conditional probability laws, diffusion and noising processes, energy-based descriptions, source-conditioned distributions, and sampling procedures, with particular interest in treating prediction, response, and generation as different operations of one coherent learned law.

- **Statistical mechanics and coarse-graining:** ensembles, entropy, free energy, source–response relations, effective interactions, coarse-graining, renormalization, and conditional refinement as mathematical tools for understanding what information an effective description should retain and what can be integrated out.
