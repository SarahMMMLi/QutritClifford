# A Complete and Natural Rule Set for Multi-Qutrit Clifford Circuits

This repository contains detailed proofs as described in appendix E of the paper. More precisely, we show how to reduce 378 box relations to a much smaller, more canonical set of rewrites rules. In the end, we find that 17 gate relations, as presented in Figure 1 of our paper, suffice to prove these 378 box relations. In what follows, we explain the folder structure, notations, and the conventions of all proofs, as well as how they are mapped onto Appendix E of the paper.

## Folder Structure
Using the derived relations and the meta rules, we show that all the box relations in Appendix D are consequences of the reduced relations in Figure 1. We do this by first proving all single-qutrit derived relations and box relations so that we can claim we have completeness for single-qutrit Clifford circuits. We can then use this completeness as a lemma for proving results about two-qutrit circuits. After similarly showing completeness for two-qutrit circuits, we can then use this completeness as a lemma for proving results regarding the three-qutrit circuits. Hence the proofs are arranged in folders titled:

- Single-Qutrit
- Two-Qutrit
- Three-Qutrit
