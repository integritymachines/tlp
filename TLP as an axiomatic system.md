# TLP as an axiomatic system

5 November 2026

## Abstract

The *Tractatus Logico-Philosophicus* [Witt1922d, Witt1922e] admits a self-consistent axiomatic system, *TLP*, under the *Least Inconsistent* (*LI*) criterion.

## TLP

*TLP* is a minimal spanning set of 13 independent axioms (A) and nine derivations (D) for the 526 propositions of the *Tractatus* under the *Least Inconsistent* criterion (*LI*).¹ It violates none of them, reads 14 narrowly, and adds one commitment without a textual source.² The adopted interpretive decisions leave no tie between inequivalent systems under *LI+*.³ A corrected model-existence proof establishes consistency for the adopted revision-58 system.⁴ There are infinitely many states of affairs, and the decidability of logic constrains their organization.⁵

### Signature

- O: objects. A: states of affairs, partial slot maps $\kappa(a)\colon P \to O$. $\Lambda = \{0,1\}^A$: worlds. χ\*: the actual world.
- Picture $P = (D, \rho, \tau)$: D finite and nonempty; ρ injective on names; τ bijective on forms and slots; $r\colon D \to A$ induced. Sense: $\sigma_{P,\chi} = (\chi \restriction D) \circ r^{-1}$.
- M+: the medium is the whole written sign. Fitting preserves atomic incidence and shared symbols; names are injective, and a binder avoids the same-sort free letters of its body and every name token of the checked sign. Sibling bound letters may share tokens where these lexical constraints permit. Series holes write their full interface images, with a separate state for each propositional letter. Logical signs add no projected states; defined signs are expanded before fitting.⁶
- C-nv: in Φ(x), x ranges over values o not named in its scope for which Φ(o) has sense in its own right. A general proposition must fit as a whole, with the adopted exposed-atom clause. N over an empty admitted range is true; N() may be a true component but is not a standalone sign. A vacuous value description is the singleton B: existential abstraction yields B, while N still yields ¬B.⁷
- N+: a quantifier excludes the values of the variables free in its scope and of the names in it.⁸
- Commitments: S1, fixed O and A; S3, every projection admissible unless A6s forbids it; S4, states are partial slot maps; K3, the three kinds of description in 5.501 are exhaustive.⁹

### Axioms and derivations

Sources are given in parentheses.¹⁰ "Completely general" means name-free; "singled out" means uniquely described by a formula whose uniqueness sentence also has sense.

- **D1** O is nonempty. ← A19 (2.026)¹¹
- **D2** Distinct states of affairs have distinct slot maps. ← A7, S3 (2.01, 2.03)¹²
- **D3** Every object occurs in some state of affairs. ← A13 (2.011)¹³
- **A4** States of affairs are independent: $\Lambda = \{0,1\}^A$. (2.061, 4.27, 6.37)¹⁴
- **A5** There is an actual world χ\*. (2.04, 2.06)¹⁵
- **A6a** A picture's medium is a fact of the world it depicts: its states are in A. (2.141, 3.14)¹⁶
- **A6s** No nonempty part D′ of a picture's medium has r(D′) = D′. (3.13; 4.024, 4.061, 2.161)¹⁷
- **A7** Every nonempty finite situation is the sense of some picture. (2.19, 4.5)¹⁸
- **A8** Definitions are well-founded and uniform, with one definition per sign; syntax is settled independently of meaning. (3.23, 3.33)¹⁹
- **D9** Every object has a name. ← D3, A7 (3.203)²⁰
- **D10** Every possible sign expresses a sense under some admissible projection. ← A7, A6s, S3, A6a, A4, A8 (4.5, 5.473)²¹
- **A11** In some adequate notation, whether a proposition is a tautology is decidable from its sign and definitions. (5.551, 6.126)²²
- **D12** Every world with the completely general truths of χ\* is isomorphic to χ\*. ← A17 (5.526)²³
- **A13** Every object occurs in some state of affairs with a different object. (2.0121)²⁴
- **A14** Every state of affairs combines at least two distinct objects. (2.03, 2.031, 2.032, 2.14, 2.15, 4.0311)²⁵
- **D15** Every object fixed by the automorphisms of the frame and χ\* is singled out by one completely general description. ← A16 (2.02331)²⁶
- **A16** Every object is singled out at χ\* by one completely general description. (5.526)²⁷
- **A17** Any two worlds with the same completely general truths are isomorphic. (5.5262, sentence 2)²⁸
- **A18** For every proposition p, every minimal alteration of χ\* that changes its truth value changes the completely general truths. (5.5262, sentence 1)²⁹
- **A19** In some world, there are distinct objects o, o′ that agree in sense and truth for every name-free formula Ψ(x). (5.5302)³⁰
- **D-S4** Every state of affairs is finite. ← A11, A7, S3 (4.2211, 4.04)³¹
- **D21** Every nonempty multiplicity class of A is infinite. ← A7, A6s, A6a, S3, D2 (3.13, 4.463)³²

### Restricted propositions

| Proposition | Reading kept |
|---|---|
| 4.128, 5.453³³ | No number is pre-eminent; ℵ0 bounds only what completely general signs can fix. |
| 4.243³⁴ | "fx" is schematic. |
| 4.461, 5.132, 5.1362, 5.5351³⁵ | "Sinnlos" is the null sense. |
| 5.47³⁶ | "fa" is schematic: R(a, b) as a function of a. |
| 5.53³⁷ | Exclusion is weak (N+). |
| 2.173³⁸ | No picture is its own object. |
| 2.224³⁹ | The type reading: no sense fixes its own truth value. |
| 5.5321⁴⁰ | "Only one" where the doubled instances fit. |
| 4.1272⁴¹ | "There are n objects which φ" is sayable where the n-fold instances fit. |
| 5.24 (X51) | Bases and result share the bases where the operation keeps them; under variabilization (4.1273's series) they share the base's form.⁴² |

## Notes

[1] The *Least Inconsistent* criterion (*LI*). Under their original readings [Witt1922d, Witt1922e] the 526 propositions are jointly inconsistent. A formalization seeks admissible readings under which they are consistent. Options are compared by violations (propositions left out), then by restrictions (narrower readings the wording admits). Marks are compared first by kind and then by level; at the first difference, the option with fewer marks wins.

- Kinds: definition (a unit with "heisst", "nenne ich", "Def.", "das heisst", "besteht darin, dass", or "X ist das, was ..." with X not fixed before) > limit (something cannot be said, expressed, asserted, thought or asked, or is nonsense) > assertion > notation and remark.
- A mark is weighted by the unit it narrows (sentence, gloss, parenthesis), once per proposition.
- Level: digits after the point; the figures "indicate the logical importance" (note to 1).
- Witnesses: the reading preferred by *LI* among those the printings admit.
- Ties (*LI+*): fewer commitments without textual source; fewer axioms; better witness alignment; the 1922 printing.

[2] Spanning and minimality. Spanning: every proposition of the 1922 printing [Witt1922d, Witt1922e, Witt1922pg] is an axiom source, derived, restricted or consistent with *TLP*; none is left out. Minimality: each axiom fails in a countermodel that satisfies the other twelve (Appendix B; X54–X57), so none is derivable from the rest. Ties go to fewer axioms (*LI+* 2). The commitment is K3 (note 9). No limit (4.1212, 4.122, 4.126–4.1274) is violated because the axioms are frame conditions, not propositions; frame facts show (6.12, 6.124). That is the question 6.54 raises. Seventeen readings rely on a textual witness for which the alternative witness admits only a weak reading or requires a special clause (grade V2); 5.152 follows Wittgenstein's correction [Lewy1967, Witt1933, Witt1961].

[3] *LI+* decided 5.526's second sentence (one axiom against two), the finiteness of states (derived: one commitment fewer) and an exception clause to 2.224 (same models). The sole tie between incongruent systems, over 2.02331, dissolved under A16 (X21–X22).

[4] Appendix A outlines the model-existence argument; Appendices C and D give the full proofs. The decision procedure uses a bound over the complete expanded input, ambient-aware fitting relations and complete substitution tables. Correctness on admitted inputs is proved before eventual periodicity is used; future map legality and grammar membership are not decided. The remaining axioms use explicit descriptions, world invariants and a simultaneous Baire-category construction. This is a proof for the adopted revision-58 system, whose computational-input requirement was changed in X49. The mathematical argument has been self-audited; no external independent certificate or full executable verification is claimed. Independence: Appendix B.

[5] D21 (note 32); cf. 4.463, "den ganzen—unendlichen—logischen Raum". Necessary conditions for A11 include (X27, X42): (a) for each arity, slot pair and pattern, the union of the forms' projections contains $K_{n,n}$ for finitely many n only; (b) the same for the incidence of forms and tuples; (c) the truth of fitting frame sentences is decidable. Failures of (a) or (b) encode finite graphs [Trak1950, Vau1960]. These conditions are necessary, not sufficient. No full frame with infinite O, or with finite O and finitely many arities, carries a model.

[6] 3.332's "das Satzzeichen", 3.14's "seine Elemente, die Wörter", 5.5261's "wie im unverallgemeinerten Satz" (X29, X41). No binder on a name's token: one element in two symbols is what 3.325 excludes (X43); the loose rule restricts 3.325 (definition), the strict one 4.1272 and 5.5321 (assertions). A defined sign signifies through its definiens (3.261) and is replaceable by it (4.241, 6.23): it fits as its translation (X47). Logical signs are "Interpunktionen" (5.4611); variables are signs (4.1271, 4.1272), and exempting their tokens restricts 3.14 (definition, level 2) and more (X48).

[7] Counting instances outside the frame as false violates 5.501 ("dessen Glieder Sätze sind"), 3.313 and 3.315; cf. 5.5351, "nicht falsch, sondern unsinnig" (X24).

[8] Strong exclusion contradicts 5.54 and A11 (X9). Excluding variables only contradicts 5.52's substitution reading: 7,152 random cases, 0 mismatches under N+, 59 without names (X35). [Hint1956, Wehm2004, RogW2012]

[9] S1: 2.012, 2.021–2.024, 2.027. S3: 5.473. S4: 2.01, 2.03, 2.031, 3.1432. K3: "Wir können drei Arten der Beschreibung unterscheiden" does not say "only these"; without K3, A11 fails for infinite A. Probability (5.15): the fair product measure on Λ [Carn1945].

[10] A: each is independent of the other twelve (Appendix B). D: follows from the premises after ←.

[11] A19 needs two objects. 2.026: "Nur wenn es Gegenstände gibt, kann es eine feste Form der Welt geben."

[12] If κ(a) = κ(a′) with a ≠ a′, no picture of {a ↦ 1} has a well-defined projection r, against A7.

[13] With A14, D3 and A13 are interderivable (X19).

[14] 2.061: "Die Sachverhalte sind von einander unabhängig." Cf. [Butt2017].

[15] 2.04: "Die Gesamtheit der bestehenden Sachverhalte ist die Welt."

[16] 2.141: "Das Bild ist eine Tatsache"; 3.14: "Das Satzzeichen ist eine Tatsache."

[17] 3.13: "aber nicht das Projizierte. Also die Möglichkeit des Projizierten, aber nicht dieses selbst." Hereditary, since parts of pictures are pictures (2.1513; X42); for finite D, r has no cycle. The rival system K, in which s := (∃φ)(∃x, y)φ(x, y) and p ∨ s lack sense, restricts 4.5(iii) (definition, level 1); *TLP*, on which they have sense, restricts 2.173 and 2.224 (assertion, level 3) (X41, X46). 3.332 gives containment by its reason clause, not A6d's support condition (3.24, 3.333; X40).

[18] 4.5(ii): "jeder mögliche Sinn durch ein Symbol ... ausgedrückt werden kann". A collective reading leaves out 4.5 (X1).

[19] Also 3.261, 5.451. Effective syntax is a strengthening, not a reading (X3); its corollary |A| = ℵ0 now follows from A11 (note 22).

[20] D3 puts o in some state a; A7 depicts {a ↦ 1}; ρ reaches every object of κ(a).

[21] A7 gives a cycle-free picture of the tokens of the sign's named parts; its inverse is an admissible projection (S3) that A6s does not bar. This requires hereditary A6s (X42).

[22] 5.551: "ohne weiteres"; 6.126: "kann man berechnen". Decidability requires a finite procedure on the whole sign (6.122, 6.1262). Names: an injective naming by finite strings in some adequate notation, "in einer entsprechenden Notation" (6.122). A name's symbol carries what all symbols for its object share (3.3411), so its finite type is too little: in Φ, "something has a state into c" is a tautology at o₁ and a contradiction at h (X49; provisional). Hence O and the forms are countable and |A| = ℵ0. Definitions are input (X47). A11 is a promise problem over admitted meaningful signs; the algorithm need not decide G\* membership. X49 changes the former finite-type input requirement.

[23] A17 at χ\*. Strictly weaker than A17 relative to the other axioms: in Appendix B's Ξ, D12 holds at χ\* and A17 fails (X57).

[24] 2.0121: "keinen Gegenstand ausserhalb der Möglichkeit seiner Verbindung mit anderen denken". The plural is number-neutral (X13).

[25] Reciprocal predicates need two objects: 2.031 "zueinander", 2.14 "zu einander", 4.0311 "untereinander". The rivals restrict the definitions 2.14 and 2.15; A14 restricts 4.24 and 5.47 (X18).

[26] Singled out: true of that object only, with a 5.5321 sentence that has sense (5.526; X42).

[27] 5.526: "Und dies x ist a." So every object is fixed by the automorphisms of χ\* and |O| ≤ ℵ0 (note 33).

[28] 5.5262, sentence 2: "der Spielraum ... welchen die ganz allgemeinen Sätze begrenzen": a range of possibilities (4.463; X25). A11 forces |A| = ℵ0 (note 22).

[29] 5.5262, sentence 1: "Es verändert ja die Wahr- oder Falschheit jedes Satzes etwas am allgemeinen Bau der Welt": minimal alterations (X25, X26).

[30] 5.5302: "(Selbst wenn dieser Satz nie richtig ist, hat er doch Sinn.)" Indiscernible by name-free formulas, not conjugate by automorphisms (4.122, 4.1241, 4.126; X34). Never at χ\*, by A16. Cf. [Weis2017].

[31] Finite signs (A11) depict each state with its multiplicity (A7; 4.04).

[32] For a finite class K, A7 for "all of K true" needs r(D) = K with D ⊆ K (A6a; r preserves multiplicity and is injective, D2), so r(D) = D, against A6s. Lokhorst stipulates infinitely many states [Lok1988].

[33] A16 caps |O|, and A11's finite names make O and the forms countable (X49). The plain reading would leave out 5.526, 5.551 and 6.126 (X22, X45, X49).

[34] Monadic elementary propositions would restrict the definitions 2.14 and 2.15.

[35] 4.461: "Tautologie und Kontradiktion sind sinnlos." "No sense at all" contradicts 4.5(iii); cf. 4.4611 (X4).

[36] "Denn 'fa' sagt dasselbe wie '(∃x).fx.x = a'"; read with 3.318.

[37] Note 8.

[38] s and p ∨ s have sense and are true wherever their sign exists, so the bipolar "darum" fails for them.

[39] Co-text 2.223 and 2.141 make it plainly about the token, which s settles; 6.113's "am Satz allein" takes the type.

[40] For f = Cyc("x lies in a 2-cycle") in Φ, the doubled existential is false even though a and b satisfy f: the required named instance does not fit (X42, X43).

[41] (∃x, y)(Cyc(x) ∧ Cyc(y)) is false in Φ even though a and b satisfy Cyc (X43). This has the same interpretive cost as note 40.

[42] Judgments. The outcome depends on the following interpretive judgments. Counting marks without first ranking their kinds would reverse X41, X43 and X47.

| Judgment | Ground | If it failed |
|---|---|---|
| Axioms are frame conditions (X18, X24) | 6.12, 6.124 | Every axiom says what shows (6.54) |
| Decidable = finite procedure (X24) | 6.126, 6.122, 6.1262 | Tie: infinite states admitted |
| Names in an adequate notation (X49; provisional) | 6.126, 3.3411, 6.122 | Tie with the finite type, if co-plain and it has a model |
| ℵ0 effects charged uniformly (X22) | No text separates caps | Ties over 5.526 |
| "mit anderen" number-neutral (X13) | Bare generic plural | Tie with strict A13, if it has a model |
| 5.526's descriptions name-free (X22) | "ohne irgend einen Namen" | Tie over 2.02331 |
| Singled out, with sense (X42) | 5.526 | A16 weaker |
| 5.5262: minimal change; Spielraum (X25) | 1.21; 4.463 | A18 or A17 changes |
| Name-free indiscernibility (X34) | 4.122, 4.1241, 4.126 | Tie with conjugacy (open) |
| Names excluded too (X35) | 5.52, 5.501 | Tie, if the rival unmarked |
| 3.332 as containment (X40) | Its reason clause | A restriction; strongly, HIGH ALERT #2 |
| 2.18 as scope; 3.13 as situation (X41) | "überhaupt"; "das Projizierte" | As for 3.332 |
| 3.04, 2.225 not diagonal (X41) | "Gedanke"; "a priori" | As for 3.332 |
| 2.224 token, 6.113 type (X41) | 2.223, 2.141 | Self-depiction admitted; D21 lost |
| Parts of pictures are pictures (X42) | 2.1513 | Tie with the whole-sign form |
| Sign = perceptible element (X43) | 3.14, 3.32 | Loose rule; 4.1272, 5.5321 lifted |
| 4.5's gloss defines; no route via 6 (X46) | "das heisst" | 2.18, 3.332 alert-relevant |
| Defined signs fit as translations (X47) | 3.261, 4.241, 3.34 | A second commitment possible |

## Appendix A: the model Φ and its corrected proof

The object domain is

$$O = \{h, h', a, b\} \cup \{o_i \mid i \in \mathbb{N}_{>0}\}.$$

The state space is exactly

$$A = \bigcup_{i \ge 1} \{R_i(a,b),\, R_i(b,a),\, R_i(h,o_i)\} \;\cup\; \bigcup_{i \ge 1} \{f_{i,j}(h', o_i) \mid 1 \le j \le i\}.$$

All objects and forms displayed with distinct symbols are distinct. The world space is $\Lambda = \{0,1\}^A$. Choose the actual world $\chi^* \in \Lambda$ by

$$\chi^*(R_i(a,b)) = 1_S(i),\quad \chi^*(R_i(b,a)) = 1_T(i),\quad \chi^*(R_i(h,o_i)) = 1,\quad \chi^*(f_{i,j}(h',o_i)) = 1,$$

where $1_S$ and $1_T$ are the indicator functions of sets $S, T \subseteq \mathbb{N}_{>0}$ selected by the simultaneous construction below. Writing F for the frame,

$$\mathrm{Aut}(F) \cong \langle (ab) \rangle \times \prod_{i \ge 1} \mathrm{Sym}\{f_{i,1}, \dots, f_{i,i}\}.$$

Thus the only object motion is the global transposition (ab); marker forms may be permuted independently within each unit.

### A11: exact claim and proof structure

Let e be a closed, meaningful, admitted G\* sign and let Δ be its finite well-founded definition data. There is an effective procedure D such that

$$D(\Delta, e)\downarrow, \qquad D(\Delta, e) = 1 \iff \forall \chi \in \Lambda\; V_{\Phi,\chi}(e) = 1.$$

Names use the stipulated injective effective notation. The procedure assumes the legality of successive series substitutions; it does not decide that promise.

Expand the complete input and compute every full hole-interface image. Let w be the maximum object/form variable-bag size over all written nodes, including ordinary wrappers and binder bodies, and let n count all original names. Set

$$Q = \max\{1, w + n\}, \qquad b = 4Q + 2n + 8.$$

Letterwise transport, full receiving interfaces and scope-preserving normalization bound every generated live bag by Q, even when term size and nesting depth grow without bound.

Two finite auxiliary constructions have different purposes. The uncoloured token structure $H_b$ computes ambient-aware fitting relations. Finite semantic representatives $M_P$ of exactly realizable b-profiles P compute truth. They retain exact named exceptions, capped marker supplies, orientation bits and correlations between selected units. Token placements are never equated with semantic referents. Fresh-unit relocation supplies admissible hereditary projections.

A finite record retains occurrence and exposed-atom information, root/component status, fitting relations under ambient reservations, and sense/truth tables under complete external substitutions. The compiler walks the fixed written expression and treats supplied filler records as opaque data. Descriptor closure and fitting are calculated separately from term values. Correctness is proved on safe observations of legal substitutions; no infinite-future legality flag is used.

For a series [B, x, C] in a filler environment Γ, define

$$k_0 = \mathrm{Compile}(B, \Gamma), \qquad F(k) = \mathrm{Compile}(C, \Gamma[x \mapsto k]), \qquad k_{m+1} = F(k_m),\ m \in \mathbb{N}.$$

Structural induction on the written expression, followed by induction on m, proves agreement with the normalized terms and admission under the own-instance rule. Only then does repetition in the finite record space justify replacing the infinite observation sequence by its preperiod and cycle. The same induction proves agreement between worlds and their profile representatives, including nested series. Acceptance at every realizable profile decides tautologyhood.

### A16–A18 and the actual world

Finite name-free formulas describe each leaf $o_i$ by the exact number i of distinct forms reaching it from a common source. A guarded disjoint-edge test distinguishes $R_i$ from markers. Four families of completely general sentences recover the h-edge bits, marker truth counts, orientation types and relative orientations of mixed units. Agreement on those families constructs a world isomorphism, proving A17. The argument includes the token placements and own-instance range checks required for these formulas.

For A16, explicit descriptions distinguish h and h′, and one asymmetrically oriented unit distinguishes a and b. Each description is true of exactly its intended object and has a fitting doubled uniqueness sentence. Rigidity alone is not substituted for this construction.

For A18, select the actual world within the Cantor space

$$X = \{\chi \in \Lambda \mid \chi(R_i(h,o_i)) = \chi(f_{i,j}(h',o_i)) = 1 \text{ for all } i \ge 1,\ 1 \le j \le i\}.$$

Each proposition p has a Borel truth set $B_p = \{\chi \in X \mid V_{\Phi,\chi}(p) = 1\}$, by well-founded countable Boolean semantics. A Baire-category argument supplies a common comeagre set $G \subseteq X$, invariant under finite coordinate flips and the global swap, on which each truth set is locally constant relative to G. Choose $\chi^* \in G$ with $|S \setminus T| = |T \setminus S| = \aleph_0$.

By A17, the only distinct world sharing χ\*'s completely general truths is $\chi^\dagger = (ab)\cdot\chi^*$. Its difference set $D = \{s \in A \mid \chi^\dagger(s) \ne \chi^*(s)\}$ is infinite. If χ† changes a proposition, relative local constancy and flip invariance supply a world χ′ changing that proposition with $\{s \in A \mid \chi'(s) \ne \chi^*(s)\} \subsetneq D$ finite. Thus χ† cannot be a minimal truth-changing alteration. This proves A18 at the same χ\* used for A16. The construction neither assumes a countable transitive model of all set theory nor restricts Λ. If a suitable countable forcing model is supplied, its generic set can also be included in the comeagre intersection.

### Axiom accounting and scope

| Axiom | Proof |
|---|---|
| A4, A5 | Full world space; actual world supplied by the simultaneous construction |
| A6a, A6s, A7 | Medium states in A; admissible projections exclude cycles; fresh finite copies represent every nonempty finite situation |
| A8 | Finite, well-founded, uniform definitions and hygienic expansion |
| A11 | Corrected whole-input finite-record procedure above |
| A13, A14 | Directly from the displayed binary frame |
| A16 | Explicit unique descriptions and meaningful uniqueness sentences |
| A17 | Verified invariant families construct an isomorphism |
| A18 | Invariant Baire construction and the proper-sub-alteration argument |
| A19 | At the all-false world, (ab) preserves every name-free sense and truth |

The resulting model establishes the consistency of the adopted thirteen-axiom system in the ordinary classical metatheory used by these proofs. The conclusion is accepted in the present mathematical self-audit. External independent verification is not claimed. Full proofs: Appendices C and D; independence: Appendix B.

## Appendix B: independence

**Standard.** A countermodel for Ak is a structure in which every axiom other than Ak holds by a proof and Ak fails. The structure consists of a frame F, a world space Λ, an actual world χ\* (where it has one), a medium, the admissible pictures Π, and a notation with its definitions. Full proofs are recorded in the ledger (X54–X57). The arguments below are complete at the standard of Appendices C and D.

| Axiom | Countermodel | Failure |
|---|---|---|
| A4 | Φ, with the worlds in which R_1(a, b) and R_1(b, a) are both true removed | Λ ⊊ {0,1}^A (B.4) |
| A5 | Φ's frame | No actual world (B.5) |
| A6a | An external medium: a disjoint copy of Φ's frame outside O and A | Medium states not in A (B.6) |
| A6s | Φ with every projection admissible | A picture depicts its own medium (B.7) |
| A7 | Φ + Q(h, h′, z), Q2(h′, h, z2) | No picture of {Q, Q2 true} (B.8) |
| A8 | A circular definition | Not well-founded (B.9) |
| A11 | Φ ⊔ directed paths with lengths in a non-recursive set L | Tautology undecidable (B.10) |
| A13 | Φ + an idle object | It occurs in no state (B.11) |
| A14 | Φ + unary states V_k(o_k) | One-object states (B.12) |
| A16 | Φ with S = T | a, b not singled out (B.13) |
| A17 | Ξ, a column frame | Non-isomorphic worlds with the same general truths (B.14) |
| A18 | Φ with S = ℕ>0, T = ∅ | The swap is a minimal alteration keeping the general truths (B.15) |
| A19 | ζ: forms f_{n,j}(h, o_n), j ≤ n | Rigid: every object described in every world (B.16) |

### B.1 Transfer

None of the following proofs uses χ\*:

- Appendix C (A11, which depends on the frame and the full world space, D.5);
- D.1's counting lemma, which is semantic but true at every world;
- D.2 (A17 and the automorphism calculation);
- the fitting witnesses of D.1 and D.4 (sense of the descriptions and of their 5.5321 sentences);
- D.5 for A4, A6a, A6s, A7, A8, A13, A14, A19.

They use only the frame, Λ = {0,1}^A, the notation with its definitions, and the fitting and sense rules. A structure that agrees with Φ in these respects satisfies those axioms by the same proofs. Only D.3 (A5, A18) and, in D.4, the descriptions D_a and D_b use χ\*. D_a and D_b depend on it through the choice of i_0 and the actual orientation; the descriptions of o_i, h and h′ are true at every world.

### B.2 Lemma G (A11 on unit frames)

A unit frame has:

- finitely many hub objects and hub forms, each hub form with finitely many states on hubs;
- units i ≥ 1 of one template: a leaf o_i; finitely many template forms, one copy per unit, each with a fixed finite set of states on hubs and o_i; and marker forms f_{i,j}, 1 ≤ j ≤ i, each with the one state f_{i,j}(s, o_i) for a fixed hub s.

Its world space is Λ = {0,1}^A.

Appendix C proves A11 on such a frame by the same procedure, with names extended to its hubs and forms. The frame enters only C.1 (names; arities), C.2 (its closing sentence on A6s relocation), C.4 (fitting tables) and C.5 (profiles). C.3 and C.6–C.8 do not depend on the frame.

- **Arities.** Atoms of any arity are incidence tests; C.3 counts letters, not arity.
- **C.4.** Ω_F has the hubs and infinitely many units with infinitely many markers; H_b has b units with b markers each, and the hubs exactly. Units are interchangeable and the marker supply is unbounded, so finite incidence-and-inequality witnesses transport to fresh units, and the back-and-forth property holds.
- **A6s.** Template forms relocate to fresh units as in Φ. Hub forms do not relocate, so hereditary A6s is checked in every own-instance check, as part of the acceptance relation with the hub-name tokens pinned. These are finitely many cases, kept exactly in H_b.
- **C.5.** An anonymous unit's type is its template bits and capped marker counts; hub bits are exact. Realizability is C.5's arithmetic.

Lemma G does not cover a constrained world space with co-possible tokens. A4's countermodel avoids that case (B.4).

In each countermodel below that changes Φ's propositions, χ\* is chosen by D.3 over that structure's own propositions. D.3 applies verbatim.

### B.3 Lemma G2 (A11 on column frames)

A column frame glues countably many unit frames at one hub (B.14): each column is a unit frame with hubs g and c_u. Appendix C applies with C.2, C.4 and C.5 nested one level. C.1, C.3 and C.6–C.8 are frame-independent.

- **C.2.** Move every used token column to a fresh column index, keeping levels. Incidences, inequalities and marker capacities survive, and token and target states are disjoint, so hereditary A6s never binds. g has no forms.
- **C.4.** Ω_Ξ has infinitely many columns, sub-units per column and markers per sub-unit; H_b has b of each. With fewer than b identities in play, a new column, a new sub-unit in a touched column, or a new marker in a touched sub-unit always has a mate. Finite witnesses move to fresh columns at large, distinct levels.
- **C.5, profiles.**
  - Pin every column and every sub-unit that contains a named item.
  - A pinned sub-unit records its B bit, its named markers' truth, and its residual true and false marker counts (capacity j minus named), capped at b.
  - A column records its pinned sub-units and the capped counts of its anonymous sub-unit types (B bit, capped true and false marker counts). An anonymous column's type is that record.
  - The profile is the pinned data plus the capped counts of anonymous column types.
  - Realizability is C.5's arithmetic at both levels. Within a column it runs over levels of capacity j, and each column needs a saturated sub-unit type; across columns, infinitely many columns need a saturated realizable column type.
  - The profile set is finite. M_P truncates saturated supplies to b copies at both levels.
- **Matching invariant (a b-pebble strategy).**
  - g is matched with g, and pinned items with themselves.
  - Each touched column is matched with a column of the same capped type.
  - Each touched sub-unit is matched with a sub-unit of the same (bit, t, f) type in the matched column.
  - Each marker is matched with a marker of the same truth in the matched sub-unit.
  - A B-form or marker touches its sub-unit and its column.

  Atoms hold exactly on (B_{u,j}, c_u, o_{u,j}) and on (a marker of (u, j), g, o_{u,j}). The matching preserves incidence, truth, equality, N+ and the atom clause on fully named atoms. Levels are not atomic: only counting tells them apart. Counting past the cap would need more live variables than the bag bound Q < b allows, so capped counts always leave a mate.
- **Same profile, same truth.** Two worlds with profile P both match M_P (C.5). C.8's world-profile adequacy carries every series term and each countable joint negation at one cap b, because series generate no names.

### B.4 A4

**Countermodel.** Φ with world space Λ_1 := {W : not (W(R_1(a, b)) = W(R_1(b, a)) = 1)}. The constraint is on unit 1 only. "Situation" is read as possible (2.202). A sign's tokens must be co-possible, i.e. jointly true in some world of Λ_1. χ\* makes unit 1 FF (both orientation states false). Every other unit, every marker and every R_i(h, o_i) is chosen as in D.3, over this structure's propositions, on the subspace X_1 with unit 1 FF. X_1 is a Cantor space.

- **A4 fails:** Λ_1 is a proper subset of {0,1}^A.
- **Fit is Φ's.** Co-possibility can bind only on unit 1's two orientation states. Tokens are never pinned (C.4). Units are interchangeable, and unit 1 has the fewest markers (c(1) = 1). So every fitting placement relocates to fresh units of index ≥ 2 (C.2, X50 Lemma 1), with hereditary A6s by the same move. Co-possibility never binds, and fit and sense are Φ's.
- **A11:** Appendix C with unit 1 pinned in every profile; its realizable types are FF, AB and BA. C.5's arithmetic and matching are unchanged.
- **A7:** a possible finite situation is copied by unit shift onto fresh units ≥ 2 (D.5). For example, {R_1(a, b) → 0, R_1(b, a) → 0} takes tokens on R_m(a, b) and R_m(b, a) with m ≥ 2. The witnessing world values the units ≥ 2 freely.
- **A16:** D.4, with i_0 ∈ S \ T and i_0 ≥ 2.
- **A17:** D.2. TT_1 is false at every world; swap(a, b) preserves Λ_1; Aut is Φ's.
- **A18:** Γ is generated by finite flips on units ≥ 2 and by the swap, and it preserves X_1. The isomorphs of χ\* are χ\* and χ†. D.3.3's variant χ′ lies in X_1 ⊆ Λ_1.
- **A19:** the all-false world lies in Λ_1; the swap is used as in D.5.
- **A5, A6a, A6s, A8, A13, A14:** as for Φ.

### B.5 A5

**Countermodel.** Φ's frame, with Λ = {0,1}^A and Φ's notation, and no actual world.

- **A5 fails** by construction.
- **A16, A18 (and D12, D15)** are conditionals ("if χ\* is the actual world, …"), so they hold vacuously.
- **Every other axiom** holds by B.1.

### B.6 A6a

**Countermodel.** Φ, with its actual world χ\* (D.3), and an external medium: M is a disjoint copy F′ of Φ's frame, outside O and A. Its objects are not objects of the world, carry no names and fall under no quantifier; otherwise A13, A16 and A11's naming would be affected. Every sign's tokens are states of F′, and projections map F′-tokens to A.

- **A6a fails:** M ∩ A = ∅.
- **Fitting in F′ coincides with fitting in Φ.** An isomorphism F → F′ carries token placements both ways, preserving incidence, St, N+ and name injectivity. The atom clause concerns the referents of names, which are objects of F, not tokens. So propositions, senses and truth values are Φ's, and Appendix C's procedure applies unchanged.
- **A6s:** r maps tokens in F′ into A, so no nonempty D′ has r(D′) = D′.
- **A7:** D.5's fresh-copy construction, carried out in F′.
- **Every other axiom:** as for Φ.

### B.7 A6s

**Countermodel.** Φ, with its actual world χ\* (D.3), and every projection admissible (Π unrestricted).

- **A6s fails:** the elementary sign R_1(a, b), with its token on the state R_1(a, b) itself, has r(D) = D.
- **Senses are unchanged.** Whenever a sign fits and meets the atom clause, an A6s-respecting placement exists, by fresh-unit relocation (X50 Lemma 1). So the propositions, their senses and their truth values at every world are Φ's.
- **A11, A16–A18 and the rest** hold by the proofs for Φ. A7 holds a fortiori, since there are more pictures.

### B.8 A7

**Countermodel.** Φ plus hubs z, z2 and ternary hub forms Q, Q2, with the one states Q(h, h′, z) and Q2(h′, h, z2). χ\* makes Q and Q2 true and f_{1,1}(h′, o_1) false. Everything else is chosen by D.3, over this structure's propositions, on the subspace with these values fixed; there, all other markers and every R_i(h, o_i) are true.

- **A7 fails.** Only Q's and Q2's states are ternary, so a picture of {Q → 1, Q2 → 1} has the projection identity or swap on them. Hereditary A6s forbids both: the identity has fixed points, and the swap is a 2-cycle.
- **A11:** Lemma G, with hub A6s checked in every own-instance check. The A6s swap: a fully named Q-atom takes Q2's state as its token and conversely. This puts the token of name h at h′ and the token of name h′ at h.
- **A16 for z, z2.** A frame test cannot fit at both h and h′, so the descriptions go through the actual world.
  - F(u) := (Ep)(Ey)(St(p, u, y) . ~p(u, y)), "u has a false out-edge". It fits at h and at h′. At χ\* it is true of h′ (f_{1,1} is false) and false of h.
  - D_z2(x) := (Eq)(Eu, v)(St3(q, u, v, x) . F(u)) and D_z(x) := (Eq)(Eu, v)(St3(q, u, v, x) . ~F(u)), with St3(q, u, v, x) := q(u, v, x) v ~q(u, v, x).
  - Only z and z2 are third objects of ternary states, with first objects h and h′ respectively. D_z is true of z only and D_z2 of z2 only.
  - Both have sense at every stage, including the fully named one, because F fits at either hub. Their 5.5321 sentences fit with the copies on Q's and Q2's states.
  - Φ's descriptions keep their objects, since z and z2 have no binary states.
- **A17.** D.2's families, plus:
  - QT := (Eq)(Eu, v, x)(q(u, v, x) . S(u)), with S(u) := ~(Ep)(Ey)(St(p, u, y) . (Eq′)(St(q′, u, y) . St(p, u, y))), "u has no two out-forms into one object". S fits only with u's token at h′ (f_{2,1}, f_{2,2} into o_2). It is true of h and false of h′.
  - At the fully named stage for (Q, h), the A6s swap puts h's token at h′, where S fits. In the Q2-branch, h′'s token is at h, where S does not fit. So QT reads Q(h, h′, z) at every world.
  - Q2T := (Eq)(Eu, v, x)(q(u, v, x) . T′(u)), with T(u) := (Ep)(Ey)(St(p, u, y) . Off(p, u, y)) and T′(u) := (Ep)(Ey)St(p, u, y) . ~T(u). At Q2T's fully named stage h′'s token is at h, where T′ fits, so it reads Q2's bit. Its Q-branch has no sense.
  - Q, Q2, z and z2 are fixed by every automorphism, so these families are complete.
- **A18:** D.3 on the fixed subspace. Marker permutations fix χ\*, since unit 1's single marker is false and all others are true. So the isomorphs are χ\* and swap(a, b)(χ\*), and D.3.3 applies.
- **A19:** swap(a, b) at the all-false world fixes the hub part.
- **A13** (z, z2 occur with h, h′), **A14** (three distinct objects), **A4, A5, A6a, A6s** (enforced) and **A8:** as for Φ.

### B.9 A8

**Countermodel.** Φ, with its actual world χ\* (D.3), its notation and definitions, plus one circular definition d := ~d, with d a propositional sign.

- **A8 fails:** the definition is not well-founded.
- **Propositions are Φ's.** A sign containing d has no finite translation, so it is no proposition (X47: a sign with defined signs has sense iff its translation fits). The propositions, senses and truth values are Φ's.
- **A11:** the naming is Φ's. Given a sign and its definitions, first check syntactically whether d occurs (a finite expansion graph). If it does, the sign is outside the promise. If not, its reachable definitions are well-founded and Appendix C decides tautologyhood.
- **A5, A16 and A18:** by D.3 and D.4.
- **Every other axiom:** by B.1.

### B.10 A11

**Countermodel.** Φ ⊔ P_L. P_L has one form Q and one directed path of each length n ∈ L, where L is infinite and non-recursive; χ\* is all true on P_L. Objects of Φ meet at least two forms, and path vertices meet exactly one.

- **A11 fails.** Let S_n := (Eφ)(Ex_0..x_n)(St(φ, x_0, x_1) … St(φ, x_{n−1}, x_n) . ~(Ez)St(φ, z, x_0) . ~(Ez)St(φ, x_n, z)).
  - S_n has sense: since L is infinite, it fits inside a longer path.
  - S_n is a tautology iff n ∈ L. So a decision procedure for tautologyhood would decide L.
- **The other axioms:** recorded in the ledger's Appendix B.

### B.11 A13

**Countermodel.** Φ plus one idle object z, a hub in no state.

- **A13 fails:** z occurs in no state.
- **A11:** Lemma G.
- **A16.** Φ's descriptions keep their unique objects, since each requires an edge at x.
  - z is described by Z(x) := ~((Ep)(Ey)St(p, x, y) v (Ep)(Ey)St(p, y, x)), true of z only. At z the y-ranges are empty; the p-ranges are not.
  - Z fits with x at a, and its doubled 5.5321 sentence fits with the copies at a and b.
- **A17:** z is fixed by every automorphism and carries no state, so D.2 applies.
- **A18:** D.3.
- **A19, A7, A14, A4, A5, A6a, A6s, A8:** as for Φ.

### B.12 A14

**Countermodel.** Φ plus, in each unit, a unary form V_k with the one state V_k(o_k). χ\* is chosen by D.3 on the subspace with every V-bit true.

- **A14 fails:** V_k(o_k) combines one object.
- **A11:** Lemma G.
- **A16:** D.1 counts binary forms only, so U_i and D.4's descriptions keep their objects.
- **A17:** add UT_i := (Ew)(U_i(w) . (Eq)(q(w) . (q(w) v ~q(w)))). It fits with w at o_m and q at V_m, and it reads V_i(o_i). With D.2's families, the invariants are complete.
- **A18:** D.3.
- **A7:** unit shift moves V_k with its unit; A6s as for Φ.
- **A13, A19, A4, A5, A6a, A8:** as for Φ.

### B.13 A16

**Countermodel.** Φ with χ\*\_=: every marker state and every R_i(h, o_i) true, and S = T (for definiteness, S = T = ∅).

- **A16 fails.** swap(a, b) is an automorphism of the frame and fixes χ\*\_=, since S = T. Name-free formulas are equivariant under such an automorphism (D.5, A19). So every completely general formula true of a at χ\*\_= is true of b, and no description singles out a.
- **A18 holds.** Let W have the completely general truths of χ\*\_=.
  - By A17, W = σ(χ\*\_=) for some σ ∈ Aut(F) (D.2).
  - Marker permutations fix χ\*\_=, since all markers are true; the swap fixes it, since S = T.
  - So W = χ\*\_=, which changes no proposition. No genericity is needed.
- **A5:** χ\*\_= exists.
- **Every other axiom:** by B.1.

### B.14 A17

**Why a new frame class.**

- In every unit frame of Lemma G, A17 holds: units are described, their finite types are read, and a finite hub symmetry is fixed by compactness over finite joint types (D.2's OR argument).
- Frames whose identical units each carry infinitely many unordered markers fail A17, but they fail A18 as well. Describable types differ by finitely many markers, so a finite alteration can swap two units.
- So failing A17 needs infinitely many interchangeable units whose types differ at infinitely many rigid positions.
- A11 needs those positions to be told apart only by counting, never by an incidence chain. A chain with series descriptors allows lockstep comparison, which makes tautology undecidable.

Ξ therefore has two levels: columns are interchangeable, and within a column, levels are fixed by marker count.

**Frame Ξ.**

- Objects: a hub g; column objects c_u (u ≥ 1); sub-leaves o_{u,j} (u, j ≥ 1).
- Forms: B_{u,j}, with the one state B_{u,j}(c_u, o_{u,j}); markers f_{u,j,k} (1 ≤ k ≤ j), with the one state f_{u,j,k}(g, o_{u,j}).
- Aut(Ξ) = Sym(columns) ⋉ ∏ Sym(markers of each sub-unit), a wreath-type product:
  - g is the only object with two out-forms into one object;
  - a sub-leaf's level is its marker count;
  - B_{u,j} ties o_{u,j} to c_u.
- The world space is {0,1}^A. A world gives each column the sequence β_u(j) := W(B_{u,j}), plus the marker bits.
- A11 holds by Lemma G2 (B.3). A proposition's truth at W depends only on its profile at W.

**Profiles with all markers true.**

- Sub-units of level j < b have type (bit, j, 0), one per level; levels ≥ b have type (bit, b, 0).
- So a column's unpinned type at cap b is (β|\_{b−1}, the capped count of 1s, the capped count of 0s at levels ≥ b).
- If β has infinitely many 0s and 1s, the type is β|\_{b−1} with tail (b, b).

**A17 fails.** Let D be the set of sequences w(01)^ω (w a finite word), and γ := 1 0 1 00 1 000 1 … . γ is not eventually periodic, so γ ∉ D.

- W_1: all markers true, with columns carrying D bijectively. W_2: the same with D ∪ {γ}.
- Every finite word is a prefix of infinitely many members of D. So at every cap b, both worlds have every prefix type saturated, with tail (b, b), and no other type.
- Their profiles agree, so every name-free sentence with sense has the same truth at W_1 and W_2.
- An isomorphism of worlds is a frame automorphism, hence a column permutation that keeps levels. It would have to biject columns preserving sequences, but γ ∉ D. So W_1 and W_2 are not isomorphic.

**Actual world.** χ\*: all markers true; β_u := 1^u 0 τ_u with τ_u := (0^u 1)^ω.

- The minimal eventual periods u + 1 are distinct, so |β_u Δ β_v| is infinite for u ≠ v.
- Every β_u has infinitely many 0s and 1s.

**Tests** (name-free; the abbreviations are D.1's).

- Counting. M_k(o_{u,j}) holds iff k ≤ j: the sources are g, with j forms, and c_u, with one. g and c_u have no in-edges. So U_j is true exactly of the level-j sub-leaves. It fits with y at a fresh o_{m,J}, J > j; name reservation forces its counting source to g.
- Bit_n(x) := (Ey)(U_n(y) . (Ep)p(x, y)) and NBit_n(x) := (Ey)(U_n(y) . (Ep)(St(p, x, y) . ~p(x, y))). Both fit with x at c_m (p at B_{m,J}) or at g (p at a marker). At a named c_u they read β_u(n), because the atom clause admits only p = B_{u,n}.
- DS(x) := (Ep, q)(Ey)(St(p, x, y) . St(q, x, y)) fits only at g and is true only of g.

**A16 at χ\*.**

- g: D_g(x) := (Ep)(Ey)St(p, x, y) . ~(Ep)(Ey)(St(p, x, y) . ~p(x, y)), "an out-edge and no false out-edge".
- c_u: D_u(x) := ⋀_{j≤u} Bit_j(x) . NBit_{u+1}(x). The prefix 1^u 0 is unique to β_u; g has no false out-edge; leaves have no out-edge.
- o_{u,j}: D_{u,j}(y) := U_j(y) . (Ex)(D_u(x) . (Ep)St(p, x, y)).
- Sense at every stage.
  - The x tokens sit at fresh column objects.
  - The inner y-binders avoid the name tokens by taking other levels of the token column.
  - Counting sources sit at g.
  - At the fully named stage of D_{u,j}, St(B_{u,j}, c_u, o_{u,j}) is a state.
- Doubled 5.5321 sentences.
  - D_g's copies sit at g and c_m.
  - D_u's copies sit at c_m and c_m′.
  - D_{u,j}'s copies sit at sub-leaves of two fresh columns.
  - DS is not a description: its doubled sentence cannot fit, since only g has double out-forms.

**D12 at χ\*.** Suppose CGT(W) = CGT(χ\*). The following sentences have sense and hold at χ\*, hence at W:

- "no false marker": ~(Ex)(DS(x) . (Ep)(Ey)(St(p, x, y) . ~p(x, y))), with x at g;
- ~(Ex)NBit_1(x);
- the 5.5321 sentences of D_g and of each D_u;
- for each u and n, (Ex)(D_u(x) . Bit_n(x)) or its NBit counterpart, according to β_u(n).

At W, it follows in order that:

1. all markers are true;
2. g satisfies D_g, so by uniqueness every column has a 0;
3. since no column has a 0 at level 1, every column has the prefix 1^u 0 for exactly one u ≥ 1;
4. each D_u has exactly one realizer, which bijects columns with the indices u;
5. the Bit_n sentences fix every bit.

Hence W = π(χ\*) for a permutation π of columns.

**A18 at χ\*,** by profile replacement; no genericity is needed. Let p change truth between χ\* and W, with CGT(W) = CGT(χ\*). By D12, W = π(χ\*). If π = id, W = χ\*. Otherwise:

- Let b be p's cap. Let J be the pinned columns, the columns v < b − 1, and their π-preimages; J is finite.
- Define W″: on each v ∈ J, β_v reset to β_{π(v)} at levels < b and at named levels; χ\* off J; all markers true.
- P(W″) = P(W).
  - On J, the first b − 1 bits and the named levels are W's, and both tails are (b, b).
  - Off J, both worlds have only the type (1^{b−1}, (b, b)), infinitely often.
- So p(W″) = p(W).
- Δ(W″) is finite and contained in Δ(W), since every changed coordinate takes W's value. Δ(W) is infinite, because some v has π(v) ≠ v and |β_v Δ β_{π(v)}| is infinite. So the inclusion is proper.
- Hence W is not a minimal p-changing alteration, and A18 holds. This covers every proposition, series included (B.3).

**The remaining axioms.**

- **A7:** a finite situation is copied onto fresh columns at the same levels; the name g keeps its token at g. Token and target states are disjoint (hereditary A6s), and ρ is injective.
- **A19:** swapping columns 1 and 2 is an automorphism fixing the all-false world, so c_1 and c_2 are indiscernible.
- **A13:** g and c_u each occur with o_{u,j}.
- **A14:** every state is binary on distinct objects.
- **A6s:** by relocation (B.3).
- **A4, A5, A6a, A8:** as for Φ.

**By-product.** D12 holds at Ξ's χ\* while A17 fails, so A17 is strictly stronger than D12 relative to the other axioms.

### B.15 A18

**Countermodel.** Φ with χ\*\_→: every marker state and every R_i(h, o_i) true; S = ℕ>0 and T = ∅.

- **A16 holds.** D.4's descriptions need only some i_0 ∈ S \ T; take i_0 = 1.
- **A5:** χ\*\_→ exists.
- **Every other axiom except A18:** by B.1.
- **A18 fails.**
  - Let q := (p)(p(b, a) . ~p(a, b)), that is, ~(Ep)~(p(b, a) . ~p(a, b)).
  - **Sense.** The named atoms stand under the non-vacuous form binder p, so the atom clause does not apply to the written sign. The tokens p at R_m, a at a and b at b fit, and p's token avoids the name tokens, which are of a different sort.
  - **Range.** At every world, p ranges over the forms f for which f(b, a) . ~f(a, b) has sense. Those are exactly the R_i, since the only two-way object pair is {a, b} and markers have one state.
  - So q is true at W iff W(R_i(b, a)) = 1 and W(R_i(a, b)) = 0 for every i.
  - Let χ† := swap(a, b)(χ\*\_→). q is false at χ\*\_→ and true at χ†. Δ(χ†) is the set of all orientation atoms.
  - **Minimality.** If Δ(W) ⊊ Δ(χ†), some orientation atom keeps its value at χ\*\_→, so q(W) = false. So χ† is a minimal q-changing alteration.
  - χ† has the completely general truths of χ\*\_→, by equivariance.
  - Hence a minimal alteration changes q without changing the completely general truths: A18 fails.

### B.16 A19

**Countermodel.** ζ: objects h and o_n (n ≥ 1); forms f_{n,j} (1 ≤ j ≤ n), each with the one state f_{n,j}(h, o_n); χ\* all true.

- **A19 fails.** At every world, U_n has sense at every object and is true of o_n only, by D.1's counting lemma with h the only source. So no two distinct objects are indiscernible.
- **A11:** Lemma G.
- **A16:** U_n describes o_n. h is described by H(x) := ~(Ep)(Ey)St(p, y, x), which fits with x at a leaf and is true of h only. The doubled sentences fit on distinct units, and H's at two leaves.
- **A17:** MC′\_{i,k} := (Ew)(U_i(w) . (Eu)(Ep_1 … p_k) ⋀_j (St(p_j, u, w) . p_j(u, w))). Aut(ζ) = ∏_i Sym(f_{i,1..i}), and equal counts give an automorphism.
- **A18:** marker permutations fix χ\* (all true), so the only world with the completely general truths of χ\* is χ\*.
- **A13, A14, A4, A5, A6a, A6s** (relocation), **A7** (unit shift) and **A8:** as for Φ.

## Appendix C: formal-series decidability

This appendix gives the definitions and argument needed for the A11 theorem stated in Appendix A. All bounds refer to one complete finite input. No finite quotient uniform over contexts with arbitrarily many additional names is asserted.

### C.1 Syntax, inputs and normalization

There are object letters, form letters of specified arity, and propositional hole letters. Names for the displayed frame are a,b,h,h',o_i,R_i,f_{i,j}, written with effective decimal indices; f_{i,j} requires 1≤j≤i. Distinct names have distinct referents. A name's referent is not its token location.

Atomic expressions are f(t_1,...,t_k), with the declared sorts. Ordinary expressions are finite joint negations N(E_1,...,E_m) and N over a one-letter abstraction z.B, for an object or form letter z. The standard finite Boolean connectives and existential notation abbreviate these operations. A series descriptor [B,x,C] describes the sequence whose base is B and whose successor is the fixed context C with its x-holes filled. Joint negation of that described family is an expression. B has no occurrence of the local x; enclosing propositional holes may occur in B or C when the descriptor is nested. An operation may have zero, one or several local hole occurrences. There are no tuple-series or unrestricted syntax-inspecting operations.

For a descriptor, form its finite least word closure L: include the free letters and names of B and C outside its local holes, the images contributed by holes of enclosing series, and close under the declared maps. Its exposed interface consists of the external free letters V and names N_br; locally bound targets are not external interface letters. Each hole j carries a sort-preserving map

    mu_j : V ∪ N_br -> V ∪ bnd(j) ∪ N_br,

where bnd(j) contains the letters bound above that hole. It writes the full image mu_j(V ∪ N_br), identities included. Map-source spellings are scope-inert. There is no name generation or shadowing of a binder on a path to a hole. Enclosing-hole images in an inner descriptor must respect its interface or the intervening binders.

Set T_0=B. To form T_(m+1), freshen T_m's private binders, apply the appropriate map at each hole, substitute the copies into C, and normalize. Normalization recomputes inner closures and hole images from inside out, deletes idle declaration units, then deletes newly vacuous abstractions with their enclosing truth operation retained. It does not move a surviving scope, merge prefixes or inspect other syntactic features of a filler. A map identifying two inner closure sources with incompatible images is undefined. Admission of a series requires every stipulated successive step, including nested steps, to be defined. This is the syntactic promise, not a test assumed available to the algorithm.

Definitions are finite, uniform and well founded; expand them hygienically before performing these operations. Form arities other than two have no atomic state in Φ. Empty ordinary N has value true as a permitted component, but no standalone state-bearing sign. A vacuous abstraction has the singleton value B; N over it is N(B), not B.

### C.2 Fitting, sense and value

Token fitting is existential and independent of semantic reference. Every atom must be placed on a frame state, with repeated letters and atoms sharing their assignments. Names are injective. At a binder, its token differs from the tokens of the other same-sort letters free in its body and every same-sort name of the whole sign being checked. Sibling internal binders may share tokens where those constraints permit. A series' written tokens are those of B and C, including its H1 words, plus a distinct state per propositional letter; its descriptor is not replaced by a union of its term tokens.

Sense combines this fitting requirement with the literal exposed-atom condition: fully named atoms outside non-vacuous binding must denote states. Apply the component convention and vacuous transparency just specified. For applicable finite named projections require hereditary A6s. It causes no further existential obstruction in Φ: move every used token unit to a distinct sufficiently large fresh index beyond the finitely many named target indices. All incidence and inequalities survive, and token and target forms are disjoint, so no projection cycle remains.

For N over z.B at parameters alpha, a candidate d is admitted exactly when it has the right sort, satisfies N+ against the names and other free parameter values in that body, and the named instance B[d,alpha] has its own sense. Equal referents are represented by the same name. The value is true exactly when every admitted instance is false. A series at parameters alpha uses exactly the instances T_m[alpha] having their own sense, and likewise takes their joint negation. Empty admitted families give true. Ambient reservations from one token check are not automatically imported into the next body's own-instance check. Sense and map admission do not depend on the world's truth valuation.

### C.3 The whole-input width bound

In the fully expanded written input, include every node, ordinary wrappers as well as all series bases, operations and full hole images. At a binder include its body bag together with the binder letter. Let w be the largest object/form free-variable bag and let n count all original names, including declaration names. Put Q=max(1,w+n) and b=4Q+2n+8.

Every augmented live bag in any legal finite unfolding has size at most Q, counting its free letters and names. Proof: a copied node's exposed letters have a single image and its private binders are freshly renamed; a name turned into a variable was already charged. At a receiving node every external word brought by a hole is in its full written image, including the union over multiple holes. A legal map transports an existing closure, and recomputing a receiving closure cannot escape its declared pool. Normalization deletes units and never moves retained scopes. Induction over any finite unfolding sequence proves the assertion. The original nodes include the ordinary wrapper, so the bound applies to the entire input.

A checked named instance promotes at most Q active free identities to names. Its own name set, original names, live boundary and auxiliary boundary-role charts fit within 3Q+n identities, below b. This does not count every ancestor binder as a new permanent reservation. The budget bounds local interfaces, not total syntax size, binder count or generated nesting depth.

### C.4 Finite fitting relations

Let Ω be the uncoloured version of the frame with infinitely many units and infinitely many markers in each. Let H_b have b units and b markers per unit, with the same hubs and R incidences. Φ embeds in Ω. Conversely every finite positive incidence-and-inequality witness in Ω transports to distinct sufficiently large Φ units. Thus they agree on existential whole-sign fitting.

Selected tuples of at most b identities in Ω and H_b are matched by exact hubs, object/form roles, touched-unit partition, and marker equality. With fewer than b identities retained, a new unit or a new marker in a touched unit always has a mate; the leaf and R-form of a touched unit have unique corresponding mates. This is a back-and-forth extension property for incidence and equality.

The lexical constraints form a tree recursion with the live boundary and all reserved names in each bag. An atom tests incidence; a finite N-node combines its child relations at the same boundary assignment; a binder existentially extends by a token satisfying the exclusions. Internal siblings are independent only after that common boundary is fixed. Induction through this recursion transfers acceptance exactly between Ω and H_b. It preserves repeated atoms and shared tokens, rather than reducing them to atom counts. Additional propositional-letter states are chosen afterwards on fresh units; their unbounded possible number is not forced into H_b.

These tables describe unanchored existential fitting. They do not assert equivalence when a token is externally pinned to a small-capacity Φ unit. Semantic names do not impose such pinning.

### C.5 Finite world profiles and their realizability

At cap b, pin every unit containing an original named leaf, R-form or marker. Record its three R truth bits, each named marker's truth, and residual true/false marker counts capped at b. An anonymous unit's type is its three R bits and its capped true/false marker counts. Record the number of anonymous units of each type, again capped at b. The original constant interpretations and named-unit identities remain exact.

Realizability is decidable by a finite search and arithmetic. At each pinned unit, the residual capacity is its known index minus the number of named markers. A count below b is exact; count b means at least b. Check that the two count intervals can sum to that capacity. Enumerate the finitely many assignments for unpinned indices below 2b. For every remaining index the possible capped pairs are exactly (r,b), (b,s), r,s<b, and (b,b), with arbitrary R bits. Meet each remaining finite quota with distinct tail indices; a type not permitted in the tail must already have its quota met. Infinitely many residual indices can be assigned if and only if some tail-permitted type has saturated quota. Assign the rest to that type. This proves necessity and sufficiency and constructs a world, rather than inferring realizability from symmetry.

For each realizable profile P, form M_P by retaining named units and named markers and replacing every saturated residual marker supply and anonymous unit supply by exactly b copies. This is a semantic structure, not a token structure or necessarily a literal cut of Φ. Match selected tuples to any world of profile P, keeping pinned units and named markers fixed, matching touched anonymous units injectively, and retaining marker truth/equality and unit correlations. A form value touches its unit even when its leaf has not been selected. With fewer than b selected values a new required unit or marker has a mate because supplies are either exactly equal below b or both at least b.

Induction proves agreement for the required bounded-variable observations at arbitrary quantifier depth. The sense tests use equality, sorts, frame incidence and the separate syntactic fitting tables, all preserved by this matching. They require no extra unidentified world-dependent colour. Later series induction will extend this result; no assumption about infinite-world finite-state periodicity is made here.

### C.6 The finite records and ordinary operations

Use finite sorted pools for the at most Q exposed variable identities, original names, active parameter-name roles and local boundary charts. Private binders are represented at their local boundary and canonically reindexed; their fresh printed spellings are not ever-growing carrier elements. For every external role/word substitution, including identifications, retain:

1. Exact occurring free-letter and name sets, exposed-atom sets, and the root/component state-presence and sense flags.
2. The acceptance relation for every ambient name-presence pattern and boundary token assignment in H_b.
3. Sense and truth observations for every realizable profile, relevant tuple in M_P, and named-instance role pattern. A component truth entry is distinct from a standalone value-admission entry.

This is a finite product K. All original names are parameterized, including names which move only after several substitutions. Ambient names absent from the filler still have reservation rows. A larger input with more context names requires a new K.

An atom fills the indicated incidence and truth tables. Ordinary Boolean constructors combine truth entries and boundary acceptance relations. A binder chooses token extensions in H_b and, separately, loops over semantic candidates in M_P, applying N+ and the body's own-instance sense before truth lookup. Occurrence data decide vacuity and exposure. These are explicit finite operations on the record arrays.

For a hole mapped by mu, operate on the complete array by

    A_mu(k)[rho] = k[rho composed with mu],

with the necessary finite port reindexing. Do not discard the entire array because its identity row fails. In particular, a direct composite may be defined when a different intermediate quotient is not. That observation does not authorize using the illegal intermediate as a sign.

There is no field deciding whether infinitely many future transformations will be defined. Complete elementary operations deterministically on all finite records, assigning arbitrary fixed results to locally detected failures. No semantic correctness is claimed for unsafe entries or records without legal representatives.

### C.7 Descriptor calculation and safe observations

Call an observation safe when the directly transformed expression, including any named-instance equality pattern, is map-admissible. Safety is a proof predicate, not a computed oracle. A safe output observation of a legal composite asks only for safe filler observations: a mapped request is the corresponding transformed component of that composite. Actual parameter instances passing N+ are injective on their co-occurring interface and avoid the relevant existing names, so they preserve closure, normalization and map admissibility after freshening. Noninjective series maps are justified instead by the admitted G\* promise.

A separate finite written-descriptor procedure computes occurrence sets, closures, vacuity and fitting. Own holes supply their full H1 word images and propositional state slots, not an invented term value. Enclosing holes contribute their actual finite occurrence records. Recompute receiving closures from these generators, processing inner descriptors first; then normalize. This consists of finite unions, map images, least closures, equality tests and the ordinary fitting operations.

For an existing copied descriptor, legal closure transport is exact. If rho f = f_bar rho on the relevant map domains, every finite path from a generator maps to a quotient path, and every quotient path lifts step by step from a chosen reached preimage. Thus rho(Cl_f(S)) = Cl_fbar(rho(S)). Hygiene prevents a private terminal target from being merged with an external source. Duplicate external entries can disappear, but surviving private binder occurrences cannot disappear by external renaming. Newly receiving descriptors must nevertheless recompute their own generators; they are not treated as unchanged copies.

These facts prove the safe dependency invariant for descriptor construction as well as ordinary syntax. An undefined map cannot be executed and then repaired by arbitrary image selection. Display-only placeholders never become semantic fillers, and individual alternative rows are never passed as if they were complete semantic records.

### C.8 Structural compiler, termination and correctness

Define Compile(E,Γ) on the original finite written expression E, with complete records for its propositional holes in Γ. The preceding operations handle atoms, ordinary constructors and holes. At a series [B,x,C], set

    k_0 = Compile(B,Gamma),
    F(k) = Compile(C,Gamma[x:=k]), with stipulated normalization.

Iterate F until a whole record repeats. Compute the descriptor's written observations separately. At each semantic index the series value is the joint negation of the truth entries of terms admitted by their own sense, over the recorded preperiod and cycle.

Termination is structural induction on E. B and C are proper written subexpressions, so their calls terminate for every finite environment. The loop ranges over fixed finite K and repeats within |K|+1 visited positions. A supplied record is never expanded back into the syntax it represents. This is why increasing generated nesting depth does not invalidate termination.

For correctness, strengthen the structural induction to arbitrary legal fillers and supplied records accurate on their safe observations. Holes use direct-composite lookup; ordinary nodes use C.6 and the safe dependency invariant. At a bracket the actual finite terms T_m are map-admissible by the input promise, even if some lack sense. The smaller-expression hypothesis for B gives accuracy of k_0. Its hypothesis for C applies to any current legal filler T_m and gives accuracy at m+1. Natural-number induction therefore establishes the demanded observation accuracy at every finite m, before periodicity is invoked.

Legal closure and instance commutation identify each transformed bracket term with the appropriate direct transformed T_m. The separate descriptor calculation gives its written sense. The infinite semantic value is consequently the joint negation of exactly the admitted term observations represented by the code sequence. Whole-record repetition now allows truncation. Arbitrary unused entries can delay repetition but cannot change the demanded observations already proved correct at every index.

For world-profile adequacy, apply the same structural and finite-index inductions to corresponding observations in a world and M_P. Ordinary steps use C.5; series steps preserve every term's admission and truth and hence their countable joint negation. Periodicity is needed only to compute that common result on the finite representative side.

The reference semantics is well founded independently of this computation. Assign atoms rank 1, ordinary constructors maximum child rank plus 1, and holes ordinal rank parameters. For a bracket, iterate the structurally defined rank function of C from that of B and take an ordinal strictly greater than the supremum of all resulting ranks. These functions are monotone and have countable values on countable parameters. Hygienic substitution respects the bounds and normalization does not increase them. Every operational term has lower rank than its bracket, so transfinite recursion defines its truth without circularly choosing the compiler's fixed point.

Finally, expand the input, compute Q,b, construct all realizable profiles and finite records, and compile the closed sign with empty hole environment. Return 1 if and only if its truth entry is true at every profile. Termination and correctness above prove A11 on the stated promise. Equal complete codes induce equal outputs in every admitted use of a fixed context; no stronger claim that they classify arbitrary future syntax legality is required.

## Appendix D: the remaining axioms and a simultaneous actual world

The frame, world space and axioms are those stated in the paper. This appendix supplies the finite descriptions, fitting witnesses and actual-world proof used in Appendix A. No decidability oracle or separate process document is a premise.

### D.1 Finite descriptions: semantic calculations and fitting

Expand the following abbreviations hygienically:

    St(p,u,v) = p(u,v) or not p(u,v)
    Off(p,u,v) = exists s,t (St(p,s,t) and St(p,u,v))
    M_k(x) = exists y,p_1,...,p_k AND_j St(p_j,y,x)
    U_i(x) = M_i(x) and not M_(i+1)(x)
    Rf(p,w) = exists u (St(p,u,w) and Off(p,u,w))
    Unit_i(w,p) = U_i(w) and Rf(p,w).

All are name-free formulas, with object/form sorts as indicated in the definitions stated here. The indices i and k specify finite formula lengths; they are not hidden object names in the formulas.

St is true on meaningful atomic instances. Off includes its second St conjunct so that u,v occur in the scopes of s,t. N+ then requires a disjoint object pair; omitting that guard changes the formula under this semantics.

Counting lemma. At o_i, M_k holds exactly when k<=i. Into o_i, h supplies one R-form and h' supplies i marker forms. N+ forces the k selected form values to be distinct and their common source to differ from x. Into a and b, infinitely many R-forms are available, so every finite M_k holds. No state ends at h or h'. Thus U_i is true exactly of o_i. Also Rf(p,o_i) holds exactly when p=R_i: R_i has a disjoint common-pair state, whereas a marker has only one state.

These are conclusions about admitted quantifier chains, not just ordinary first-order readings. The fitting witnesses needed to justify those chains are as follows. All fresh token-unit indices can be chosen beyond the finitely many semantic form indices in the instance.

| Checked pattern | Compatible tokens |
|---|---|
| Counting at named x | x at a fresh leaf o_m; source at h'; bound forms at enough distinct markers of unit m |
| Rf at named p,w | p at R_m, w at o_m, u at h; Off's s,t at a,b |
| Unit_i and a cycle test | Same p,w placement; counting uses h' and markers, Rf uses h plus the common pair, cycle test uses a,b in its separate scope |
| Two units with a shared orientation test | Distinct leaf units for w,w' and distinct R-form tokens for p,q; a,b shared in the orientation block |
| Marker-count test with u,w and selected forms named | u,w at a,b; selected form names at distinct R-form tokens; each Off block uses h and that R-form's leaf |

The last row is essential. A semantic marker form need not have a marker-form token. Its negative Off subformula must fit even though its semantic witness range is empty. Using R-form tokens gives both the named (a,b) edge and a separate possible off-edge in the token pattern. At the semantic level the named marker has no disjoint edge, so Off is false. Confusing token roles with referents would break this argument.

For the marker-count formula's outer w-instance, U_i(w) also fits with w at b and its counting source at a using sufficiently many R-form tokens. At that stage u is still bound. When the u-body is subsequently checked as its own named instance, the U_i sibling is no longer in that body. This is exactly the adopted own-instance C-nv rule, not a waiver of ambient reservations within a single check.

Nested binder exclusions and global name reservations are respected in these placements. Separate sibling binders share tokens only where the final lexical rule permits it. Move all used token forms to fresh units disjoint from the named target forms; the applicable projection graph then has no directed cycle. False negative branches need a fitting sign, not a successful semantic witness. Consequently the displayed frame calculations survive C-nv, N+ and hereditary A6s.

### D.2 A17: completely general truths determine the world up to isomorphism

Define the following name-free sentences, with i≠j in OR and positive integers k:

    HT_i = exists w,p (Unit_i(w,p) and exists u (St(p,u,w) and p(u,w)))
    MC_(i,k) = exists w (U_i(w) and exists u,p_1,...,p_k
                  AND_j (St(p_j,u,w) and not Off(p_j,u,w) and p_j(u,w)))
    TT_i = exists w,p (Unit_i(w,p) and exists x,y (p(x,y) and p(y,x)))
    FF_i = exists w,p (Unit_i(w,p) and exists x,y (not p(x,y) and not p(y,x)))
    MIX_i = exists w,p (Unit_i(w,p) and exists x,y (p(x,y) and not p(y,x)))
    OR_(i,j) = exists w,w',p,q (Unit_i(w,p) and Unit_j(w',q)
                  and exists x,y (p(x,y) and not p(y,x) and q(x,y) and not q(y,x))).

Their roles are:

* HT_i selects Unit_i(w,p) and a true p-edge into w.
* MC_(i,k) selects U_i(w), a common incoming source, and k distinct true forms whose Off condition is false.
* TT_i, FF_i and MIX_i select Unit_i and respectively two true, two false, or one true/one false orientations of a two-way pair.
* OR_(i,j), i!=j, selects both units and uses the same ordered pair to test that both are mixed in the same direction.

The preceding placements verify sense and the successful named prefixes. Their exact readings at every world are:

    HT_i: truth of R_i(h,o_i);
    MC_(i,k): at least k true marker states in unit i;
    TT_i / FF_i / MIX_i: the unordered pair of orientation bits;
    OR_(i,j): the two mixed units have matching orientation.

For MC, the guarded negative Off condition excludes the R_i edge and keeps the markers. For the orientation families, both directed instances must be frame states, so their pair is {a,b}. OR does not choose separate orientations independently for the two units.

Suppose W and W' agree on all completely general truths. The HT family fixes every h-edge bit. All MC thresholds fix each finite number of true markers. The orientation families fix each unit's orientation type. If there are mixed units, choose one i_0: its two worlds' orientation determines a single global choice of identity or swap(a,b). OR_(i_0,j) forces that same choice to match every other mixed unit. Nonmixed pairs are already invariant. Within each unit choose a marker permutation carrying its true subset to the other true subset, possible because the finite cardinalities agree. These permutations, together with the one global swap, give an isomorphism W -> W'. This proves A17.

For later use, these are all the frame automorphisms. The only two-way object pair is {a,b}; h is the remaining source of R-form states, and h' is the source of one-state marker forms. Leaves have no outgoing states. Leaf o_i is fixed by its distinct finite number i of incoming marker forms. Thus each R_i is fixed, and only marker permutations within each unit and the global swap remain. This is a frame argument, independent of the truth-world invariant families.

### D.3 One actual world for A5, A16 and A18

#### D.3.1 Borel semantics, without an A11 oracle

Restrict attention temporarily to the closed subspace X of worlds in which every marker state and every R_i(h,o_i) is true. The two orientation bits per unit vary freely, so X is a Cantor space. This restriction is for choosing χ\*, not a restriction of Λ.

There are countably many finite signs with finite definition data and countably many named parameter tuples. For every meaningful proposition p, its truth set B_p within X is Borel. Atoms are clopen; Boolean operations preserve Borelness; object/form value ranges are countable and world-independent; series ranges are their countably many finite-index operational terms, filtered by world-independent sense. The nested operational dependencies are well founded by the structural ordinal-rank construction in Appendix C.8. Hence transfinite induction builds each truth set using countable Boolean operations. This is a semantic regularity proof, not an inference from the presumed decidability of tautologyhood.

#### D.3.2 A simultaneous invariant good set

For each B_p choose an open U_p with B_p symmetric-difference U_p meagre. Borel sets have this property: the sets approximable by open sets modulo meagre sets form a sigma algebra containing the open sets. Include the boundary of U_p in the exceptional set. Let Γ be the countable group generated by finite flips of orientation coordinates and the global swap of the two orientations.

Remove all Γ-translates of all these exceptional sets from X. Also remove the worlds for which either S minus T or T minus S is finite, where S,T are the two orientation supports. The latter condition is meagre: beyond any finite coordinate prescription one can prescribe another difference in either direction. Its complement is Γ-invariant.

The resulting G is comeagre, nonempty by the Baire theorem, and Γ-invariant. At every z in G, each B_p is constant on some neighborhood of z relative to G: outside the exceptional set membership agrees with U_p, and z is not on its boundary. This does not assert local constancy on all worlds.

Choose χ\* in G. This proves A5 and ensures both orientation differences are infinite. The choice satisfies all propositions' regularity requirements simultaneously, not one newly selected actual world per proposition.

#### D.3.3 A18: no truth-changing minimal alteration preserves general truths

Write Δ(W)={s∈A : W(s)≠χ(s)}. A truth-changing alteration W is minimal when no W′ with Δ(W′) a proper subset of Δ(W) changes the same proposition from its value at χ. Minimality here is by inclusion, not by numerical cardinality.

Let p change truth between χ and W, and suppose W has the same completely general truths as χ. By A17 and the frame automorphism calculation, W is either χ or χ†=swap(a,b)(χ): all markers are true, so marker permutations make no difference. The first possibility cannot change p. The difference D between χ\* and χ† is infinite.

Both worlds lie in G. At χ† choose a basic finite-coordinate neighborhood on which p has the same truth value relative to G. Flip χ only on the finitely many coordinates of D needed to enter that neighborhood. The result χ' is in G by invariance, and p at χ' equals p at χ†, differing from p at χ. Its change set is a finite proper subset of D. Therefore χ† was not an inclusion-minimal alteration changing p. This proves A18 in its MC-all sense (the definitions stated here and the proper-subset argument as defined here).

The argument does not assume minimal alterations always exist. It proves the required statement for every alteration that is minimal. It also does not infer finite sensitivity of a Borel function at arbitrary points.

#### D.3.4 Optional forcing presentation

The forcing presentation specifies a pair Cohen-generic over a countable transitive M coding the signs. If such an M is supplied with the relevant Borel codes, its generic points form a comeagre subset of X. Intersecting that set with G still gives a permissible χ\*. This is an optional presentation of the actual-world choice; the Baire proof above already establishes existence.

The model-existence proof above does not require a countable transitive model of all ZFC to exist. A claim that one exists is a distinct foundational assumption and is not proved here. The Baire construction supplies directly the actual-world property for which genericity was used. No axiom requires a particular forcing presentation of χ\*; its two supports were never specified by a fixed concrete bit sequence. Choosing them by this existence construction does not change the frame, world space or truth semantics.

### D.4 A16: descriptions and their uniqueness sentences

For o_i use U_i. For h use

    (exists p,y (St(p,x,y) and Off(p,x,y)))
    and not (exists p,y St(p,y,x)).

For h' use

    (exists p,y St(p,x,y))
    and not (exists p,y (St(p,x,y) and Off(p,x,y))).

The first selects the source of multi-state forms without an incoming edge; the second selects a source of only one-state forms. At a,b the incoming edges defeat the h-description and the available off-states defeat the h'-description. Leaves have no outgoing edge. Thus these descriptions have the asserted unique truth values.

Their named x-instances fit with x tokened at a, outgoing edges on (a,b), off-edges on (h,o_m), and incoming edges on (b,a), with compatible R-form tokens. Inner object binders avoid the named x-token. These are token placements, irrespective of x's semantic referent.

Choose i_0 in S minus T, which exists for the selected χ\*. Use these descriptions:

    D_a(x) = exists w,p (
        U_i0(w)
        and exists u St(p,u,w)
        and exists y (p(x,y) and not p(y,x))).

For D_b reverse the final two orientations. The two-way pair forces an R-form; U_i0 and the incoming edge then force R_i0. Its actual orientation selects a for D_a and b for D_b. Crucially, there is no Rf conjunct here: reinstating it would reintroduce the earlier token obstruction.

At the named satisfying instance place x at a, w at a fresh o_m, p at R_m, the incoming-edge binder at h, the counting blocks at h' and markers, and the reverse-edge binder at b. The D_b case uses the same fitting pattern. All named successful prefixes can be realized with fresh target-disjoint forms. Thus the descriptions really admit their unique intended objects; they are not merely first-order formulas that become empty under C-nv.

A16 also demands sense of the 5.5321 uniqueness sentence, not just unique truth. For a description φ, the sentence is (exists x φ(x)) and not (exists x,y (φ(x) and φ(y))), with the stipulated exclusive quantifiers. For U_i the two copies can use distinct fresh leaf units. For h,h' and D_a,D_b place the two outer argument binders at a and b. Each copy's inner reverse-edge binder can use the other token because the other outer argument is absent from that inner binder's local body. Counting and off-edge blocks use fresh units as above. At this written stage the outer arguments are bound letters, not two global name reservations. Hence the doubled sign fits.

Existence holds by the successful single instance. The doubled existential cannot have an admitted true witness with two distinct object values: each component can be true only of the one selected object, and N+ excludes equal values. Some instantiated doubled ranges can be empty, but that does not invalidate the meaningful written uniqueness sentence or its true negation. This verifies both unique truth and sense of the uniqueness sentence. Therefore A16 holds at the same χ\* used for A18.

### D.5 The remaining axioms

A4: Λ is stipulated to be all of 2^A. Selecting χ\* inside X does not remove any other worlds.

A6a: Under the adopted formulation as defined here, M=A: all sign-medium states are frame states by fitting, including written descriptor tokens. This is not replaced by a new requirement that every medium state be true in the selected actual valuation. Logical operation signs have no additional projected state as specified in the signature.

A6s: The picture class excludes any nonempty invariant subset of the finite token medium under its projection. For finite D this is the no-directed-cycle condition. It is enforced in admissibility, rather than deduced for every arbitrary projection. The fresh-copy construction below shows it does not block A7. The finiteness premise is explicit in the picture definition as defined here and 7624.

A7: Let s be a nonempty finite situation. It uses finitely many units and finitely many markers in each. Choose distinct fresh unit indices large enough to accommodate those markers. Keep a,b,h,h' fixed, transport leaves and R-forms to those units, and transport markers injectively. This gives a token copy of the situation's finite state support, preserving every shared object/form and incidence. Name it and use the conjunction of the literals required by s. Projection from the copy onto the original support is well defined and bijective there; its token forms and target forms are disjoint, so it satisfies hereditary A6s. The literal signs have exactly s as their represented situation. If medium valuation at a witnessing world is required, A4 permits the required finite valuation. No unproved disjoint-copy property for arbitrary frames is assumed.

A8: Choose the stipulated finite, uniform, well-founded definition discipline and hygienic notation; expand definitions under X47. The grammar's future map-legality promise is syntactic and world-independent. A8 does not supply, and this proof does not claim, an algorithm deciding that infinite promise. Definitions do not depend on the truth of the expressions being defined.

A13: a,b occur together; h occurs with each o_i; h' occurs with each o_i through its nonempty marker set; every o_i therefore occurs with another object.

A14: Every displayed state has exactly two distinct object entries.

A19: At the all-false world the global swap(a,b) is an automorphism of both frame and valuation. Name-free formulas are equivariant: atomic incidence and truth, token fitting, N+, own-instance filtering, legal substitutions and normalization all transport under this automorphism. Structural induction and the finite-index series induction preserve sense and truth. Thus a and b have matching sense and truth for every name-free one-object formula. Their difference in the actual world is irrelevant: A19 asks for some world.

A11: Use the theorem of Appendix C. It depends on the frame and full world space, not on computing the selected χ\*. No actual-world oracle enters the decision procedure.

## Bibliography

- [Butt2017] Button, T. "Exclusion Problems and the Cardinality of Logical Space." *Journal of Philosophical Logic* 46 (2017): 611–623.
- [Carn1945] Carnap, R. "On Inductive Logic." *Philosophy of Science* 12 (1945): 72–97.
- [Coh1963] Cohen, P. J. "The Independence of the Continuum Hypothesis." *Proceedings of the National Academy of Sciences* 50 (1963): 1143–1148.
- [Ehr1961] Ehrenfeucht, A. "An Application of Games to the Completeness Problem for Formalized Theories." *Fundamenta Mathematicae* 49 (1961): 129–141.
- [Hint1956] Hintikka, J. "Identity, Variables, and Impredicative Definitions." *Journal of Symbolic Logic* 21 (1956): 225–245.
- [Lewy1967] Lewy, C. "A Note on the Text of the Tractatus." *Mind* 76 (1967): 416–423.
- [Lok1988] Lokhorst, G.-J. C. "Ontology, Semantics and Philosophy of Mind in Wittgenstein's Tractatus: A Formal Reconstruction." *Erkenntnis* 29 (1988): 35–75.
- [RogW2012] Rogers, B., and K. F. Wehmeier. "Tractarian First-Order Logic: Identity and the N-Operator." *Review of Symbolic Logic* 5 (2012): 538–573.
- [Trak1950] Trakhtenbrot, B. A. "Impossibility of an Algorithm for the Decision Problem in Finite Classes." *Doklady Akademii Nauk SSSR* 70 (1950): 569–572.
- [Vau1960] Vaught, R. L. "Sentences True in All Constructive Models." *Journal of Symbolic Logic* 25 (1960): 39–53.
- [Wehm2004] Wehmeier, K. F. "Wittgensteinian Predicate Logic." *Notre Dame Journal of Formal Logic* 45 (2004): 1–11.
- [Weis2017] Weiss, M. "Logic in the Tractatus." *Review of Symbolic Logic* 10 (2017): 1–50.
- [Witt1922d] Wittgenstein, L. *Logisch-philosophische Abhandlung*. German text in *Tractatus Logico-Philosophicus*, London: Kegan Paul, Trench, Trubner, 1922.
- [Witt1922e] Wittgenstein, L. *Tractatus Logico-Philosophicus*. Trans. C. K. Ogden. London: Kegan Paul, Trench, Trubner, 1922.
- [Witt1922pg] Wittgenstein, L. *Tractatus Logico-Philosophicus*, Project Gutenberg EBook 5740: Distributed Proofreaders' transcription of the 1922 printing, German and English, with page scans.
- [Witt1933] Wittgenstein, L. *Tractatus Logico-Philosophicus*. Reprint with corrections. London: Kegan Paul, 1933.
- [Witt1961] Wittgenstein, L. *Tractatus Logico-Philosophicus*. Trans. D. F. Pears and B. F. McGuinness. London: Routledge & Kegan Paul, 1961 (1963 impression).
- [Witt1973] Wittgenstein, L. *Letters to C. K. Ogden*. Ed. G. H. von Wright. Oxford: Blackwell; London: Routledge & Kegan Paul, 1973.
