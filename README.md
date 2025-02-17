# A Complete and Natural Rule Set for Multi-Qutrit Clifford Circuits

This repository contains technical proofs as described in Appendix E of the paper. More precisely, we show how to reduce 378 box relations to a much smaller, more canonical set of rewrites rules. In the end, we find that 17 gate relations, as presented in Figure 1 of our paper, suffice to prove these 378 box relations. 

In what follows, we explain the folder structure, notations, and the conventions of all proofs, as well as how they are mapped onto Appendix E of the paper.

![](https://github.com/SarahMMMLi/QutritClifford/blob/main/Figures/Figure1.png)

## Folder Structure
Using the derived relations and the meta rules, we show that all the box relations in Appendix D are consequences of the reduced relations in Figure 1. We do this by first proving all single-qutrit box relations are consequences of the single-qutrit reduced relations. Then we can claim that the 7 reduced relations in Figure 45 give the single-qutrit Clifford completeness. We can then use this completeness as a lemma for proving results about two-qutrit Clifford circuits. After similarly showing two-qutrit Clifford completeness, we can then use this as a lemma for proving results regarding the three-qutrit Clifford circuits. Hence the proofs are arranged in folders titled:

- [Single-Qutrit](https://github.com/SarahMMMLi/QutritClifford/tree/main/Single-Qutrit),
- [Two-Qutrit](https://github.com/SarahMMMLi/QutritClifford/tree/main/Two-Qutrit), and
- [Three-Qutrit](https://github.com/SarahMMMLi/QutritClifford/tree/main/Three-Qutrit).

In each folder, we proceed in two steps. Take proving single-qutrit Clifford completeness as an example. The proofs for two- and three-qutrit Clifford completeness are carried out analogously.

- We show that the set of 12 derived relations in Figure 46 are consequences of the 7 reduced relations in Figure 45. All proofs can be found in the folder titled [Derived2Reduced](https://github.com/SarahMMMLi/QutritClifford/tree/main/Single-Qutrit/Derived2Reduced).
- We show that the set of 34 box relations in Appendix D.2 are consequences of the 12 derived relations in Figure 46. All proofs can be found in the folder titled [Box2Derived](https://github.com/SarahMMMLi/QutritClifford/tree/main/Single-Qutrit/Box2Derived).

To simplify the relation reduction, we use meta rules to derive useful variants of rewrite rules in Figures 45 and 46. All proofs can be found in the document titled [Variants_single_qutrit.pdf](https://github.com/SarahMMMLi/QutritClifford/blob/main/Single-Qutrit/Variants_single_qutrit.pdf).

In the meantime, the correctness of all proofs and the soundness of all box relations were checked by verifying intermediate steps. Our Python codes can be found at [Verification.ipynb](https://github.com/SarahMMMLi/QutritClifford/blob/main/Verification.ipynb).

## Notations
We use a few abbreviations to simplify the discussions, as summarized below.

- **WTS** is short for 'Want To Show'.
- **LHS** is short for 'Lefthand Side'.
- **RHS** is short for 'Righthand Side'.
- Let R be a relation. **R.LHS** means the lefthand side of R. **R.RHS** means the righthand side of R. 
- **Proof cont.** is short for 'Proof Continued'.

## Conventions
On each page of the proof, there are three sections, separated by coloured horizontal lines.

- The top section contains all the rules used to reduce a relation.
- The middle section states the lemma for a relation reduction.
- The bottom section contains the proof.
- In the technical proof,
  - we use a square box to emphasize the local circuit where we apply the rewrite rules.
  - we use an equation with rewrite rules on top of or beneath it to indicate that these rules are applied at this step.
