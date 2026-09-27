# Theory of Computation Notes

These are my notes on the theory of computation: finite automata and regular languages, grammars and pushdown automata, Turing machines and decidability, and then time and space complexity. The first three chapters cover the discrete math that the rest of the book leans on (sets and proofs, graphs, counting).

The compiled book is [theory-of-computation-notes.pdf](theory-of-computation-notes.pdf), about 500 pages.

## What's in it

1. Sets, logic, and the language of proof: sets, functions and relations, strings and languages, quantifiers, proof techniques, induction.
2. Graph theory for computation: degrees, paths and connectivity, trees, matchings and coloring, and graphs as inputs to algorithms.
3. Counting and combinatorics: pigeonhole, permutations and binomial coefficients, inclusion-exclusion, recurrences and generating functions.
4. Finite automata: DFAs and NFAs, the subset construction, and closure under the regular operations.
5. Regular expressions and nonregularity: Kleene's theorem, the pumping lemma, Myhill-Nerode, minimization, and the syntactic monoid.
6. Context-free grammars: derivations, ambiguity, Chomsky normal form, closure properties, parsing.
7. Pushdown automata: equivalence with CFGs, the pumping lemma for context-free languages, deterministic PDAs.
8. Turing machines: the model, multitape and nondeterministic variants, enumerators, the Church-Turing thesis, and the universal machine.
9. Decidability: decidable problems about automata and grammars, diagonalization, and why the acceptance problem is undecidable.
10. Reducibility: mapping reductions, Rice's theorem, the Post correspondence problem.
11. Advanced computability: the recursion theorem, oracles and Turing reducibility, the arithmetic hierarchy, which logical theories are decidable, Kolmogorov complexity.
12. Time complexity: big-O, P and NP, verifiers, polynomial-time reductions.
13. NP-completeness: the Cook-Levin theorem, reductions from 3SAT to graph problems, and what to do about hard problems.
14. Space complexity: Savitch's theorem, PSPACE-completeness and TQBF, generalized geography, L and NL, and NL = coNL.
15. Intractability: hierarchy theorems, relativization, approximation algorithms, probabilistic computation, interactive proofs.
16. Algebraic and combinatorial methods: languages recognized by finite monoids, Burnside and Pólya counting, generating functions, expander and Cayley graphs.

Appendix A puts the three subjects side by side, with a concept map, a ten-week study plan, twenty problems that cross between them, and ten longer projects.

Each section gives the definitions and theorems with proofs and then works through examples. The worked examples start by saying how to recognize the kind of problem, and most of them end by checking the answer. Every section finishes with exercises.

## Building the PDF

The book is `theory-of-computation-notes.tex`, and the macros and the TikZ styles for the state diagrams are in `preamble.tex`. It builds with pdflatex on any recent TeX Live. Run it three times so the table of contents and the cross-references settle:

```bash
pdflatex theory-of-computation-notes.tex
pdflatex theory-of-computation-notes.tex
pdflatex theory-of-computation-notes.tex
```
