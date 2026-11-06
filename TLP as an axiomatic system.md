# TLP as an axiomatic system

5 November 2026

## Abstract

The *Tractatus Logico-Philosophicus* [Witt1922d, Witt1922e] admits a self-consistent axiomatic system, *TLP*, under the *Least Inconsistent* (*LI*) criterion.

## TLP

*TLP* is a minimal spanning set of 13 independent axioms (A) and nine derivations (D) for the 526 propositions of the *Tractatus* under the *Least Inconsistent* criterion (*LI*).¹ It violates none of them, reads 14 narrowly, and adds one commitment without a textual source.² The adopted interpretive decisions leave no tie between inequivalent systems under *LI+*.³ The model Φ establishes consistency.⁴ There are infinitely many states of affairs, and the decidability of logic constrains their organization.⁵

### Basic notions

- **Frame.** A frame F has objects O, forms, and states of affairs 𝔸. Each state a ∈ 𝔸 belongs to one form and has a slot map κ(a), a partial map from that form's slots P to O (S4). An automorphism of F permutes objects, forms, slots and states, preserving κ. Aut(F) is the group of automorphisms.
- **Situations and worlds.** A situation is a map s: E → {0,1} on a set E ⊆ 𝔸 of states; it is finite when E is. A world is a situation on all of 𝔸. Two worlds χ, χ′ are isomorphic when χ′ = g·χ for some g ∈ Aut(F).
- **Multiplicity.** Two states have the same multiplicity when some bijection of slots and objects carries the slot map of one onto that of the other (4.04). A multiplicity class is an equivalence class of 𝔸 under this relation.
- **Signs and tokens.** A sign is a written expression of the language of Appendix C.1. It is built from names (of objects and of forms), variables of both sorts, atomic formulas, the joint-negation operator N, and series descriptors. A placement assigns each letter of a sign a token: an object or a form of the frame. It must assign each atomic formula the state its tokens form, the formula's token state. The medium of a sign is the set of its token states. A sign *fits* when some placement obeys M+ below; a sign that fits is *possible*. C.2 gives the full rules.
- **N and series.** N(ξ̄) is the joint negation of a range ξ̄ of propositions (5.502). A range is given by enumeration, by the values of a propositional function, or by a formal series (5.501). A formal series [B, x, C] has terms T₀ = B and T_{m+1} = C[T_m]. Quantifiers and truth-functions are defined from N.
- **Formula notation.** The main part writes ∃, ∧ and ¬. The appendices write the Principia-style (Ex), ., ~ and v, or spell out exists, and, not and or. All of these abbreviate N (C.1).
- **Sense of a sign.** A sign has sense when it fits and passes C-nv's value rule (C.2). A proposition is a sign with sense. Its sense is the set of worlds at which it is true. It is a tautology when it is true at every world of Λ.
- **Alterations.** For a world χ ≠ χ\*, let Δ(χ) = {s ∈ 𝔸 : χ(s) ≠ χ\*(s)}. χ is a minimal alteration changing p when p's truth value differs at χ and χ\*, but not at any χ′ with Δ(χ′) ⊊ Δ(χ).
- **Structures.** A structure S = (F, Λ, χ\*, M, μ, Π, 𝒩) consists of:
  - a frame F;
  - a world space Λ ⊆ {0,1}^𝔸;
  - an actual world χ\* ∈ Λ, which may be absent;
  - a medium M, the set of states that carry sign tokens, with a valuation μ: Λ → {0,1}^M, where μ(χ) = χ↾M when M ⊆ 𝔸;
  - a class Π of admissible pictures;
  - a notation 𝒩 with its definitions.

  The axioms and the commitments are conditions on S. A model satisfies all thirteen axioms. A countermodel for an axiom satisfies the other twelve and fails it (Appendix B).

### Signature

- O: objects. 𝔸: states of affairs, with slot maps $\kappa(a)\colon P \rightharpoonup O$. Λ ⊆ {0,1}^𝔸: worlds. χ\* ∈ Λ: the actual world, if there is one.
- Picture $P = (D, \rho, \tau)$:
  - D ⊆ M is a finite, nonempty set of token states;
  - ρ is an injective map from D's token objects (the name tokens) to O;
  - τ is a bijection from D's token forms and their slots to forms and slots.

  The projection $r\colon D \to \mathbb{A}$ sends each token state to the state that has the τ-images as form and slots and the ρ-images as objects. The sense of P at χ is the situation $\sigma_{P,\chi} = (\mu(\chi) \restriction D) \circ r^{-1}$ on r(D).
- M+, the medium rule: the medium is the whole written sign. Fitting preserves atomic incidence and shared symbols. Names are injective, and a binder avoids the same-sort free letters of its body and every same-sort name token of the checked sign. Sibling bound letters may share tokens where these lexical constraints permit. Series holes write their full interface images, with a separate state for each propositional letter. Logical signs add no projected states; defined signs are expanded before fitting.⁶
- C-nv, the value rule: in Φ(x), x ranges over values o not named in its scope for which Φ(o) has sense in its own right. A general proposition must fit as a whole, with the exposed-atom clause (C.2). N over an empty admitted range is true; N() may be a true component but is not a standalone sign. A vacuous value description is the singleton B: existential abstraction yields B, while N still yields ¬B.⁷
- N+, the exclusion rule: a quantifier excludes the values of the same-sort variables free in its scope and of the same-sort names in it.⁸
- Commitments:⁹
  - S1: O and 𝔸 are fixed across worlds;
  - S3: every projection is admissible unless A6s forbids it, so a projection is any map that ρ and τ induce;
  - S4: each state's slot map is a partial map from slots to objects;
  - K3: the three kinds of description in 5.501 are exhaustive.

### Axioms and derivations

Sources are given in parentheses.¹⁰ "Completely general" means name-free. "Singled out" means uniquely described by a formula whose uniqueness sentence also has sense.

- **D1** O is nonempty. ← A19 (2.026)¹¹
- **D2** Distinct states of affairs have distinct slot maps. ← A7, S3 (2.01, 2.03)¹²
- **D3** Every object occurs in some state of affairs. ← A13 (2.011)¹³
- **A4** States of affairs are independent: Λ = {0,1}^𝔸. (2.061, 4.27, 6.37)¹⁴
- **A5** There is an actual world χ\* ∈ Λ. (2.04, 2.06)¹⁵
- **A6a** A picture's medium is a fact of the world it depicts: its states are in 𝔸 (M ⊆ 𝔸). (2.141, 3.14)¹⁶
- **A6s** For every picture, no nonempty part D′ of its medium has r(D′) = D′. (3.13; 4.024, 4.061, 2.161)¹⁷
- **A7** Every nonempty finite situation s is the sense of some picture: σ_{P,χ} = s for some P ∈ Π and χ ∈ Λ. (2.19, 4.5)¹⁸
- **A8** Definitions are well-founded and uniform, with one definition per sign; syntax is settled independently of meaning. (3.23, 3.33)¹⁹
- **D9** Every object has a name. ← D3, A7 (3.203)²⁰
- **D10** Every possible sign expresses a sense under some admissible projection. ← A7, A6s, S3, A6a, A4, A8 (4.5, 5.473)²¹
- **A11** There is an adequate notation in which it is decidable, from a proposition's sign and its definitions, whether the proposition is a tautology. This is a promise problem: the input is promised to be a meaningful admitted sign (note 22). (5.551, 6.126)²²
- **D12** If χ\* is the actual world, every world with the completely general truths of χ\* is isomorphic to χ\*. ← A17 (5.526)²³
- **A13** Every object occurs in some state of affairs with a different object. (2.0121)²⁴
- **A14** Every state of affairs combines at least two distinct objects. (2.03, 2.031, 2.032, 2.14, 2.15, 4.0311)²⁵
- **D15** If χ\* is the actual world, every object fixed by the automorphisms of the frame and χ\* is singled out by one completely general description. ← A16 (2.02331)²⁶
- **A16** If χ\* is the actual world, every object is singled out at χ\* by one completely general description. (5.526)²⁷
- **A17** Any two worlds with the same completely general truths are isomorphic. (5.5262, sentence 2)²⁸
- **A18** If χ\* is the actual world, then for every proposition p, every minimal alteration of χ\* that changes p's truth value changes the completely general truths. (5.5262, sentence 1)²⁹
- **A19** In some world, there are distinct objects o, o′ that agree in sense and truth for every name-free formula Ψ(x). (5.5302)³⁰
- **D-S4** Every state of affairs is finite. ← A11, A7, S3 (4.2211, 4.04)³¹
- **D21** Every nonempty multiplicity class of 𝔸 is infinite. ← A7, A6s, A6a, S3, D2 (3.13, 4.463)³²

### Restricted propositions

| Proposition | Reading kept |
|---|---|
| 4.128, 5.453³³ | No number is pre-eminent; ℵ0 bounds only what completely general signs can fix. |
| 4.24³⁴ | "fx" is schematic. |
| 4.461, 5.132, 5.1362, 5.5351³⁵ | "Sinnlos" is the null sense. |
| 5.47³⁶ | "fa" is schematic: R(a, b) as a function of a. |
| 5.53³⁷ | Exclusion is weak (N+). |
| 2.173³⁸ | No picture is its own object. |
| 2.224³⁹ | The type reading: no sense fixes its own truth value. |
| 5.5321⁴⁰ | "Only one" where the doubled instances fit. |
| 4.1272⁴¹ | "There are n objects which φ" is sayable where the n-fold instances fit. |
| 5.24 (X51) | Bases and result share the bases where the operation keeps them; under variabilization (4.1273's series) they share the base's form.⁴² |

The outcome rests on the interpretive judgments of note 43.⁴³

## Notes

[1] The *Least Inconsistent* criterion (*LI*). Under their original readings [Witt1922d, Witt1922e] the 526 propositions are jointly inconsistent. A formalization seeks admissible readings under which they are consistent. Options are compared by violations (propositions left out), then by restrictions (narrower readings the wording admits). Marks are compared first by kind and then by level; at the first difference, the option with fewer marks wins.

- Kinds: definition (a unit with "heisst", "nenne ich", "Def.", "das heisst", "besteht darin, dass", or "X ist das, was ..." with X not fixed before) > limit (something cannot be said, expressed, asserted, thought or asked, or is nonsense) > assertion > notation and remark. This ordering is an interpretive commitment of *LI*, not a consequence of the *Tractatus*.
- A mark is weighted by the unit it narrows (sentence, gloss, parenthesis), once per proposition.
- Level: digits after the point; the figures "indicate the logical importance" (note to 1).
- Witnesses: the reading preferred by *LI* among those the printings admit.
- Ties (*LI+*): fewer commitments without textual source; fewer axioms; better witness alignment; the 1922 printing.

[2] Spanning and minimality. Spanning: every proposition of the 1922 printing [Witt1922d, Witt1922e, Witt1922pg] is an axiom source, derived, restricted or consistent with *TLP*; none is left out. Minimality: each axiom fails in a countermodel that satisfies the other twelve (Appendix B; X54–X57), so none is derivable from the rest. Ties go to fewer axioms (*LI+* 2). The commitment is K3 (note 9). No limit (4.1212, 4.122, 4.126–4.1274) is violated because the axioms are frame conditions, not propositions; frame facts show (6.12, 6.124). That is the question 6.54 raises. Seventeen readings rely on a textual witness for which the alternative witness admits only a weak reading or requires a special clause (grade V2), marked in Appendix E; 5.152 follows Wittgenstein's correction [Lewy1967, Witt1933, Witt1961].

[3] *LI+* decided 5.526's second sentence (one axiom against two), the finiteness of states (derived: one commitment fewer) and an exception clause to 2.224 (same models). The sole tie between incongruent systems, over 2.02331, dissolved under A16 (X21–X22). These comparisons are recorded in the ledger; this paper does not repeat them.

[4] Appendix A outlines the model-existence argument; Appendices C and D give the full proofs. The decision procedure uses a bound over the complete expanded input, ambient-aware fitting relations and complete substitution tables. Correctness on admitted inputs is proved before eventual periodicity is used; future map legality and grammar membership are not decided. The remaining axioms use explicit descriptions, world invariants and a simultaneous Baire-category construction. The mathematical argument has been self-audited; no external independent certificate or full executable verification is claimed. Independence: Appendix B.

[5] D21 (note 32); cf. 4.463, "den ganzen—unendlichen—logischen Raum". Necessary conditions for A11 include (X27, X42): (a) for each arity, slot pair and pattern, the union of the forms' projections contains $K_{n,n}$ for finitely many n only; (b) the same for the incidence of forms and tuples; (c) the truth of fitting frame sentences is decidable. Failures of (a) or (b) encode finite graphs [Trak1950, Vau1960]. These conditions are necessary, not sufficient; they are recorded in the ledger and not proved here. A full frame is one in which every form applies to every tuple of distinct objects. No full frame with infinite O, or with finite O and finitely many arities, carries a model.

[6] 3.332's "das Satzzeichen", 3.14's "seine Elemente, die Wörter", 5.5261's "wie im unverallgemeinerten Satz" (X29, X41). No binder on a name's token: one element in two symbols is what 3.325 excludes (X43); the loose rule restricts 3.325 (definition), the strict one 4.1272 and 5.5321 (assertions). A defined sign signifies through its definiens (3.261) and is replaceable by it (4.241, 6.23): it fits as its translation (X47). Logical signs are "Interpunktionen" (5.4611); variables are signs (4.1271, 4.1272), and exempting their tokens restricts 3.14 (definition, level 2) and more (X48).

[7] Counting instances outside the frame as false violates 5.501 ("dessen Glieder Sätze sind"), 3.313 and 3.315; cf. 5.5351, "nicht falsch, sondern unsinnig" (X24).

[8] Strong exclusion contradicts 5.54 and A11 (X9). Excluding variables only contradicts 5.52's substitution reading: 7,152 random cases, 0 mismatches under N+, 59 without names (X35; recorded in the ledger, not re-run here). [Hint1956, Wehm2004, RogW2012]

[9] S1: 2.012, 2.021–2.024, 2.027. S3: 5.473. S4: 2.01, 2.03, 2.031, 3.1432. K3: "Wir können drei Arten der Beschreibung unterscheiden" does not say "only these"; without K3, A11 fails for infinite 𝔸 (recorded in the ledger, not proved here). S2, a finitary constraint on worlds, was dropped: A4 gives Λ = {0,1}^𝔸. Probability (5.15): the fair product measure on Λ [Carn1945].

[10] A: each is independent of the other twelve (Appendix B). D: follows from the premises after ←.

[11] A19 needs two objects. 2.026: "Nur wenn es Gegenstände gibt, kann es eine feste Form der Welt geben."

[12] If κ(a) = κ(a′) with a ≠ a′, no picture of {a ↦ 1} has a well-defined projection r, against A7: by S3, r is the map that ρ and τ induce, and it cannot separate a from a′.

[13] A13 gives each object a state that contains it. With A14, D3 and A13 are interderivable (X19).

[14] 2.061: "Die Sachverhalte sind von einander unabhängig." Cf. [Butt2017].

[15] 2.04: "Die Gesamtheit der bestehenden Sachverhalte ist die Welt."

[16] 2.141: "Das Bild ist eine Tatsache"; 3.14: "Das Satzzeichen ist eine Tatsache."

[17] 3.13: "aber nicht das Projizierte. Also die Möglichkeit des Projizierten, aber nicht dieses selbst." Hereditary, since parts of pictures are pictures (2.1513; X42); for finite D, r has no cycle. The rival system K, in which s := (∃φ)(∃x, y)φ(x, y) and p ∨ s lack sense, restricts 4.5(iii) (definition, level 1); *TLP*, on which they have sense, restricts 2.173 and 2.224 (assertion, level 3) (X41, X46). 3.332 gives containment by its reason clause, not by the support condition of the retired axiom A6d (3.24, 3.333; X40). Hereditary: A6s binds the projection of every part of a sign, including each named instance checked under C-nv.

[18] 4.5(ii): "jeder mögliche Sinn durch ein Symbol ... ausgedrückt werden kann". A collective reading leaves out 4.5 (X1).

[19] Also 3.261, 5.451. Effective syntax is a strengthening, not a reading (X3); its corollary |𝔸| = ℵ0 now follows from A11 (note 22).

[20] D3 puts o in some state a; A7 depicts {a ↦ 1}; ρ reaches every object of κ(a).

[21] A6a puts a possible sign's tokens in 𝔸, so they form a situation of the frame. A4 makes that situation possible. A8 lets defined signs be read through their definientia. A7 gives a cycle-free picture of the tokens of the sign's named parts; its inverse is an admissible projection (S3) that A6s does not bar. This requires hereditary A6s (X42).

[22] 5.551: "ohne weiteres"; 6.126: "kann man berechnen". Decidability requires a finite procedure on the whole sign (6.122, 6.1262). Names: an injective naming by finite strings in some adequate notation, "in einer entsprechenden Notation" (6.122). A name's symbol carries what all symbols for its object share (3.3411), so its finite type is too little: in Φ, "something has a state into c" is a tautology at o_1 and a contradiction at h (X49; provisional). Hence O and the forms are countable and |𝔸| = ℵ0. Definitions are input (X47). A11 is a promise problem over admitted meaningful signs; the algorithm need not decide G\* membership. X49 changes the former finite-type input requirement.

[23] A17 at χ\*. Strictly weaker than A17 relative to the other axioms: in Appendix B's Ξ, D12 holds at χ\* and A17 fails (X57).

[24] 2.0121: "keinen Gegenstand ausserhalb der Möglichkeit seiner Verbindung mit anderen denken". The plural is number-neutral (X13).

[25] Reciprocal predicates need two objects: 2.031 "zueinander", 2.14 "zu einander", 4.0311 "untereinander". The rivals restrict the definitions 2.14 and 2.15; A14 restricts 4.24 and 5.47 (X18).

[26] Singled out: true of that object only, with a 5.5321 sentence that has sense (5.526; X42).

[27] 5.526: "Und dies x ist a." So every object is fixed by the automorphisms of χ\* and |O| ≤ ℵ0 (note 33).

[28] 5.5262, sentence 2: "der Spielraum ... welchen die ganz allgemeinen Sätze begrenzen": a range of possibilities (4.463; X25). A11 forces |𝔸| = ℵ0 (note 22).

[29] 5.5262, sentence 1: "Es verändert ja die Wahr- oder Falschheit jedes Satzes etwas am allgemeinen Bau der Welt": minimal alterations (X25, X26).

[30] 5.5302: "(Selbst wenn dieser Satz nie richtig ist, hat er doch Sinn.)" Indiscernible by name-free formulas, not conjugate by automorphisms (4.122, 4.1241, 4.126; X34). Never at χ\*, by A16. Cf. [Weis2017].

[31] Finite signs (A11) depict each state with its multiplicity (A7; 4.04): the projection, which ρ and τ induce (S3), maps the token state's slots bijectively onto the depicted state's, so the latter is finite. D-S4 derives the finiteness that a former commitment stipulated (note 3).

[32] For a finite class K, A7 for "all of K true" needs r(D) = K with D ⊆ K (A6a; r, induced by ρ and τ (S3), preserves multiplicity and is injective, D2), so r(D) = D, against A6s. Lokhorst stipulates infinitely many states [Lok1988].

[33] A16 caps |O|, and A11's finite names make O and the forms countable (X49). The plain reading would leave out 5.526, 5.551 and 6.126 (X22, X45, X49).

[34] Monadic elementary propositions would restrict the definitions 2.14 and 2.15.

[35] 4.461: "Tautologie und Kontradiktion sind sinnlos." "No sense at all" contradicts 4.5(iii); cf. 4.4611 (X4).

[36] "Denn 'fa' sagt dasselbe wie '(∃x).fx.x = a'"; read with 3.318.

[37] Note 8.

[38] s and p ∨ s have sense and are true wherever their sign exists, so the bipolar "darum" fails for them.

[39] Co-text 2.223 and 2.141 make it plainly about the token, which s settles; 6.113's "am Satz allein" takes the type.

[40] For f = Cyc("x lies in a 2-cycle") in Φ, the doubled existential is false even though a and b satisfy f: the required named instance does not fit (X42, X43).

[41] (∃x, y)(Cyc(x) ∧ Cyc(y)) is false in Φ even though a and b satisfy Cyc (X43). This has the same interpretive cost as note 40.

[42] 5.24's parenthesis, "das Gemeinsame zwischen den Basen und dem Resultat der Operation sind eben die Basen", is kept for operations that keep their bases. A series term comes from an operation on a variabilized base (4.1273), so base and result share only the base's form. The cost is one assertion mark at level 2 (X51).

[43] Judgments. The outcome depends on the following interpretive judgments. Counting marks without first ranking their kinds would reverse X41, X43 and X47.

| Judgment | Ground | If it failed |
|---|---|---|
| Axioms are frame conditions (X18, X24) | 6.12, 6.124 | Every axiom says what shows (6.54) |
| Decidable = finite procedure (X24) | 6.126, 6.122, 6.1262 | Tie: infinite states admitted |
| Names in an adequate notation (X49; provisional) | 6.126, 3.3411, 6.122 | Tie with the finite type, if equally plain and it has a model |
| ℵ0 effects charged uniformly (X22) | No text separates caps | Ties over 5.526 |
| "mit anderen" number-neutral (X13) | Bare generic plural | Tie with strict A13, if it has a model |
| 5.526's descriptions name-free (X22) | "ohne irgend einen Namen" | Tie over 2.02331 |
| Singled out, with sense (X42) | 5.526 | A16 weaker |
| 5.5262: minimal change; Spielraum (X25) | 1.21; 4.463 | A18 or A17 changes |
| Name-free indiscernibility (X34) | 4.122, 4.1241, 4.126 | Tie with conjugacy (open) |
| Names excluded too (X35) | 5.52, 5.501 | Tie, if the rival unmarked |
| 3.332 as containment (X40) | Its reason clause | A restriction; strongly, a conflict between an axiom and D10 |
| 2.18 as scope; 3.13 as situation (X41) | "überhaupt"; "das Projizierte" | As for 3.332 |
| 3.04, 2.225 not diagonal (X41) | "Gedanke"; "a priori" | As for 3.332 |
| 2.224 token, 6.113 type (X41) | 2.223, 2.141 | Self-depiction admitted; D21 lost |
| Parts of pictures are pictures (X42) | 2.1513 | Tie with the whole-sign form |
| Sign = perceptible element (X43) | 3.14, 3.32 | Loose rule; 4.1272, 5.5321 lifted |
| 4.5's gloss defines; no route via 6 (X46) | "das heisst" | 2.18, 3.332 would reopen that conflict |
| Defined signs fit as translations (X47) | 3.261, 4.241, 3.34 | A second commitment possible |

## Appendix A: the model Φ and its corrected proof

The object domain is

$$O = \{h, h', a, b\} \cup \{o_i \mid i \in \mathbb{N}_{>0}\}.$$

The state space is exactly

$$\mathbb{A} = \bigcup_{i \ge 1} \{R_i(a,b),\, R_i(b,a),\, R_i(h,o_i)\} \;\cup\; \bigcup_{i \ge 1} \{f_{i,j}(h', o_i) \mid 1 \le j \le i\}.$$

All objects and forms displayed with distinct symbols are distinct. The world space is $\Lambda = \{0,1\}^{\mathbb{A}}$. Choose the actual world $\chi^* \in \Lambda$ by

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

By A17, the only distinct world sharing χ\*'s completely general truths is $\chi^\dagger = (ab)\cdot\chi^*$. Its difference set $D = \{s \in \mathbb{A} \mid \chi^\dagger(s) \ne \chi^*(s)\}$ is infinite. If χ† changes a proposition, relative local constancy and flip invariance supply a world χ′ changing that proposition with $\{s \in \mathbb{A} \mid \chi'(s) \ne \chi^*(s)\} \subsetneq D$ finite. Thus χ† cannot be a minimal truth-changing alteration. This proves A18 at the same χ\* used for A16. The construction neither assumes a countable transitive model of all set theory nor restricts Λ. If a suitable countable forcing model is supplied, its generic set can also be included in the comeagre intersection.

### Axiom accounting and scope

| Axiom | Proof |
|---|---|
| A4, A5 | Full world space; actual world supplied by the simultaneous construction |
| A6a, A6s, A7 | Medium states in 𝔸; admissible projections exclude cycles; fresh finite copies represent every nonempty finite situation |
| A8 | Finite, well-founded, uniform definitions and hygienic expansion |
| A11 | Corrected whole-input finite-record procedure above |
| A13, A14 | Directly from the displayed binary frame |
| A16 | Explicit unique descriptions and meaningful uniqueness sentences |
| A17 | Verified invariant families construct an isomorphism |
| A18 | Invariant Baire construction and the proper-sub-alteration argument |
| A19 | At the all-false world, (ab) preserves every name-free sense and truth |

The resulting model establishes the consistency of the adopted thirteen-axiom system in the ordinary classical metatheory used by these proofs. The conclusion is accepted in the present mathematical self-audit. External independent verification is not claimed. Full proofs: Appendices C and D; independence: Appendix B.

## Appendix B: independence

**Standard.** A countermodel for Ak is a structure in which every axiom other than Ak holds by a proof and Ak fails. The structure consists of a frame F, a world space Λ, an actual world χ\* (where it has one), a medium, the admissible pictures Π, and a notation with its definitions. Full proofs are recorded in the ledger (X54–X57). The arguments below are complete at the standard of Appendices C and D. Each countermodel keeps the commitments S1, S3, S4 and K3 and the rules M+, C-nv and N+, except where its section says otherwise: B.4 reads "situation" as possible and adds co-possibility (the reading of A6a under a constrained Λ), and B.7 admits every projection.

| Axiom | Countermodel | Failure |
|---|---|---|
| A4 | Φ, with the worlds in which R_1(a, b) and R_1(b, a) are both true removed | Λ ⊊ {0,1}^𝔸 (B.4) |
| A5 | Φ's frame | No actual world (B.5) |
| A6a | An external medium: a disjoint copy of Φ's frame outside O and 𝔸 | Medium states not in 𝔸 (B.6) |
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

They use only the frame, Λ = {0,1}^𝔸, the notation with its definitions, and the fitting and sense rules. A structure that agrees with Φ in these respects satisfies those axioms by the same proofs. Only D.3 (A5, A18) and, in D.4, the descriptions D_a and D_b use χ\*. D_a and D_b depend on it through the choice of i_0 and the actual orientation; the descriptions of o_i, h and h′ are true at every world.

### B.2 Lemma G (A11 on unit frames)

A unit frame has:

- finitely many hub objects and hub forms, each hub form with finitely many states on hubs;
- units i ≥ 1 of one template: a leaf o_i; finitely many template forms, one copy per unit, each with a fixed finite set of states on hubs and o_i; and marker forms f_{i,j}, 1 ≤ j ≤ i, each with the one state f_{i,j}(s, o_i) for a fixed hub s.

Its world space is Λ = {0,1}^𝔸.

Appendix C proves A11 on such a frame by the same procedure, with names extended to its hubs and forms. The frame enters only C.1 (names; arities), C.2 (its second paragraph, on A6s relocation), C.4 (fitting tables) and C.5 (profiles). C.3 and C.6–C.8 do not depend on the frame.

- **Arities.** Atoms of any arity are incidence tests; C.3 counts letters, not arity.
- **C.4.** Ω_F has the hubs and infinitely many units with infinitely many markers; H_b has b units with b markers each, and the hubs exactly. Units are interchangeable and the marker supply is unbounded, so finite incidence-and-inequality witnesses transport to fresh units, and the back-and-forth property holds.
- **A6s.** Template forms relocate to fresh units as in Φ. Hub forms do not relocate, so hereditary A6s is checked in every own-instance check, as part of the acceptance relation with the hub-name tokens fixed. These are finitely many cases, kept exactly in H_b.
- **C.5.** An anonymous unit's type is its template bits and capped marker counts; hub bits are exact. Realizability is C.5's arithmetic.

Lemma G does not cover a constrained world space with co-possible tokens. A4's countermodel avoids that case (B.4).

In each countermodel below that changes Φ's propositions, χ\* is chosen by D.3 over that structure's own propositions. D.3 applies verbatim.

### B.3 Lemma G2 (A11 on Ξ)

**The frame Ξ** (the countermodel of B.14).

- Objects: a hub g; column objects c_u (u ≥ 1); sub-leaves o_{u,j} (u, j ≥ 1).
- Forms: B_{u,j}, with the one state B_{u,j}(c_u, o_{u,j}); markers f_{u,j,k} (1 ≤ k ≤ j), with the one state f_{u,j,k}(g, o_{u,j}).
- Names: g, c_u, o_{u,j}, B_{u,j} and f_{u,j,k}, written with decimal indices; f_{u,j,k} requires 1 ≤ k ≤ j. All forms are binary.
- Aut(Ξ) = Sym(columns) ⋉ ∏ Sym(markers of each sub-unit), a wreath-type product:
  - g is the only object with two out-forms into one object;
  - a sub-leaf's level is its marker count;
  - B_{u,j} ties o_{u,j} to c_u.
- The world space is {0,1}^𝔸. A world gives each column the sequence β_u(j) := W(B_{u,j}), plus the marker bits.

Each column is a unit frame (B.2) with hubs g and c_u, the template form B, and markers from g. Ξ glues countably many copies at g.

**Lemma G2.** Appendix C proves A11 on Ξ by the same procedure. As in B.2, the frame enters C.1 only through its names, listed above; C.3 and C.6–C.8 do not depend on the frame. C.2, C.4 and C.5 nest one level:

- **C.2.** Move every used token column to a fresh column index, keeping levels. Incidences, inequalities and marker capacities survive, and token and target states are disjoint, so hereditary A6s never binds. g has no forms.
- **C.4.** Ω_Ξ has infinitely many columns, sub-units per column and markers per sub-unit; H_b has b of each. With fewer than b identities in play, a new column, a new sub-unit in a touched column, or a new marker in a touched sub-unit always has a mate. Finite witnesses move to fresh columns at large, distinct levels.
- **C.5, profiles.**
  - Pin every column and every sub-unit that contains a named item.
  - A pinned sub-unit records its B bit, its named markers' truth, and its residual true and false marker counts (capacity j minus named), capped at b.
  - A column records its pinned sub-units and the capped counts of its anonymous sub-unit types (B bit, capped true and false marker counts). An anonymous column's type is that record.
  - The profile is the pinned data plus the capped counts of anonymous column types.
  - Realizability is C.5's arithmetic at both levels. Within a column, it runs over the levels j with capacity j, and the column's infinitely many residual levels need a saturated sub-unit type. Across columns, the infinitely many anonymous columns need a saturated realizable column type.
  - The profile set is finite. M_P truncates saturated supplies to b copies at both levels.
- **Matching invariant (a b-pebble strategy [Ehr1961]).**
  - g is matched with g, and pinned items with themselves.
  - Each touched column is matched with a column of the same capped type.
  - Each touched sub-unit is matched with a sub-unit of the same (bit, t, f) type in the matched column.
  - Each marker is matched with a marker of the same truth in the matched sub-unit.
  - A B-form or marker touches its sub-unit and its column.
  - Residual counts: for every matched pair of columns, and of sub-units, the untouched sub-units of each type (respectively the untouched markers of each truth value) have equal counts, capped at b minus the number of pebbles in play. Placing a pebble removes one item of one type from both sides. Lifting one returns it to both. Fewer than b pebbles are ever in play, so a required mate always exists.

  Atoms hold exactly on (B_{u,j}, c_u, o_{u,j}) and on (a marker of (u, j), g, o_{u,j}). The matching preserves incidence, truth, equality, N+ and the atom clause on fully named atoms. Levels are not atomic: only counting tells them apart. Counting past the cap would need more live variables than the bag bound Q < b allows.
- **Same profile, same truth.** Two worlds with profile P both match M_P (C.5). C.8's world-profile adequacy carries every series term and each countable joint negation at one cap b, because series generate no names.

### B.4 A4

**Countermodel.** Φ with world space Λ_1 := {W : not (W(R_1(a, b)) = W(R_1(b, a)) = 1)}. The constraint is on unit 1 only. "Situation" is read as possible (2.202). A sign's tokens must be co-possible, i.e. jointly true in some world of Λ_1. χ\* makes unit 1 FF (both orientation states false). Every other unit, every marker and every R_i(h, o_i) is chosen as in D.3, over this structure's propositions, on the subspace X_1 with unit 1 FF. X_1 is a Cantor space.

- **A4 fails:** Λ_1 is a proper subset of {0,1}^𝔸.
- **Fit is Φ's.** Co-possibility can bind only on unit 1's two orientation states. Tokens are never fixed by names (C.4). Units are interchangeable, and unit 1 has the fewest markers (one). So every fitting placement relocates to fresh units of index ≥ 2 (C.2), with hereditary A6s by the same move. Co-possibility never binds, and fit and sense are Φ's.
- **A11:** Appendix C with unit 1 pinned in every profile; its realizable types are FF, AB and BA. C.5's arithmetic and matching are unchanged.
- **A7:** a possible finite situation is copied by unit shift onto fresh units ≥ 2 (D.5). For example, {R_1(a, b) → 0, R_1(b, a) → 0} takes tokens on R_m(a, b) and R_m(b, a) with m ≥ 2. The witnessing world values the units ≥ 2 freely.
- **A16:** D.4, with i_0 ∈ S \ T and i_0 ≥ 2.
- **A17:** D.2. TT_1 is false at every world; swap(a, b) preserves Λ_1; Aut is Φ's.
- **A18:** Γ is generated by finite flips on units ≥ 2 and by the swap, and it preserves X_1. The isomorphs of χ\* are χ\* and χ†. D.3.3's variant χ′ lies in X_1 ⊆ Λ_1.
- **A19:** the all-false world lies in Λ_1; the swap is used as in D.5.
- **A5, A6a, A6s, A8, A13, A14:** as for Φ.

### B.5 A5

**Countermodel.** Φ's frame, with Λ = {0,1}^𝔸 and Φ's notation, and no actual world.

- **A5 fails** by construction.
- **A16, A18 (and D12, D15)** are conditionals ("if χ\* is the actual world, …"), so they hold vacuously.
- **Every other axiom** holds by B.1.

### B.6 A6a

**Countermodel.** Φ, with its actual world χ\* (D.3), and an external medium.

- M is a disjoint copy F′ of Φ's frame, outside O and 𝔸. Its objects are not objects of the world: they carry no names and fall under no quantifier. Otherwise A13, A16 and A11's naming would be affected.
- Every sign's tokens are states of F′, and projections map F′-tokens to 𝔸.
- The medium is valued through the copy: μ(χ)(s′) := χ(s) for the copy s′ of a state s.

Then:

- **A6a fails:** M ∩ 𝔸 = ∅.
- **Fitting in F′ coincides with fitting in Φ.** An isomorphism F → F′ carries token placements both ways, preserving incidence, St, N+ and name injectivity. The atom clause concerns the referents of names, which are objects of F, not tokens. So propositions, senses and truth values are Φ's, and Appendix C's procedure applies unchanged.
- **A6s:** r maps tokens in F′ into 𝔸, so no nonempty D′ has r(D′) = D′.
- **A7:** D.5's fresh-copy construction, carried out in F′. Let s be a finite situation. Its tokens are the copies s′ of states on fresh units, and those fresh states are distinct from s's support. Take χ with χ(s) equal to the value s assigns to r(s′) (A4). Then μ(χ) gives the tokens exactly those values, so σ_{P,χ} = s.
- **Every other axiom:** as for Φ.

### B.7 A6s

**Countermodel.** Φ, with its actual world χ\* (D.3), and every projection admissible (Π unrestricted).

- **A6s fails:** the elementary sign R_1(a, b), with its token on the state R_1(a, b) itself, has r(D) = D.
- **Senses are unchanged.** Whenever a sign fits and meets the atom clause, an A6s-respecting placement exists, by fresh-unit relocation (C.2). So the propositions, their senses and their truth values at every world are Φ's.
- **A11, A16–A18 and the rest** hold by the proofs for Φ. A7 holds a fortiori, since there are more pictures.

### B.8 A7

**Countermodel.** Φ plus hubs z, z2 and ternary hub forms Q, Q2, with the one states Q(h, h′, z) and Q2(h′, h, z2). χ\* makes Q and Q2 true and f_{1,1}(h′, o_1) false. Everything else is chosen by D.3, over this structure's propositions, on the subspace with these values fixed; there, all other markers and every R_i(h, o_i) are true.

- **A7 fails.** Only Q's and Q2's states are ternary, so a picture of {Q → 1, Q2 → 1} has the projection identity or swap on them. Hereditary A6s forbids both: the identity has fixed points, and the swap is a 2-cycle.
- **A11:** Lemma G, with hub A6s checked in every own-instance check. The A6s swap: a fully named Q-atom takes Q2's state as its token and conversely. This puts the token of name h at h′ and the token of name h′ at h.
- **A16 for z, z2.** A frame test cannot fit at both h and h′, so the descriptions go through the actual world.
  - F(u) := (Ep)(Ey)(St(p, u, y) . ~p(u, y)), "u has a false out-edge". It fits at h and at h′. At χ\* it is true of h′ (f_{1,1} is false) and false of h.
  - D_z2(x) := (Eq)(Eu, w)(St3(q, u, w, x) . F(u)) and D_z(x) := (Eq)(Eu, w)(St3(q, u, w, x) . ~F(u)), with St3(q, u, w, x) := q(u, w, x) v ~q(u, w, x).
  - Only z and z2 are third objects of ternary states, with first objects h and h′ respectively. D_z is true of z only and D_z2 of z2 only.
  - Both have sense at every stage, including the fully named one, because F fits at either hub. Their 5.5321 sentences fit with the copies on Q's and Q2's states.
  - Φ's descriptions keep their objects, since z and z2 have no binary states.
- **A17.** D.2's families, plus:
  - QT := (Eq)(Eu, v, x)(q(u, v, x) . S(u)), with S(u) := ~(Ep)(Ey)(St(p, u, y) . (Eq′)(St(q′, u, y) . St(p, u, y))), "u has no two out-forms into one object". Of h and h′, S fits only at h′ (f_{2,1}, f_{2,2} into o_2). It is true of h and false of h′.
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

**Countermodel.** Φ ⊔ P_L, where L ⊆ ℕ≥2 is infinite and non-recursive.

- For each n ∈ L, P_L adds a directed path with vertices v_{n,0}, …, v_{n,n}. One form Q carries the states Q(v_{n,k}, v_{n,k+1}), k < n.
- The world space is {0,1}^𝔸.
- χ\* is all true on P_L. On Φ's part it is chosen by D.3, over this structure's propositions, on the subspace with every P_L bit true.

**The separator.** Sep(x) := (Ep)(Eq)((Ey)Inc(p, x, y) . (Ez)Inc(q, x, z)), with Inc(p, x, y) := St(p, x, y) v St(p, y, x), reads "x meets two forms".

- y and z are sibling binders and may coincide.
- Every object of Φ meets two forms: a and b (R_1, R_2), h (R_1, R_2), h′ (f_{1,1}, f_{2,1}), o_i (R_i, f_{i,1}). A path vertex meets only Q.
- Sep fits with x at any Φ object, and so its instances have sense at every object.

**A11 fails.** For n ≥ 2, let

S_n := (Eφ)(Ex_0 … x_n)(St(φ, x_0, x_1) . … . St(φ, x_{n−1}, x_n) . ~(Ez)St(φ, z, x_0) . ~(Ez)St(φ, x_n, z)).

- N+ makes x_0, …, x_n distinct. No form of Φ has two states chaining three distinct objects: R_i's states (a, b), (b, a) return to a, and markers have one state. So a witness lies in P_L, and it is a maximal Q-chain of length n, i.e. the path of length n. (S_1 is witnessed in Φ itself, by h → o_i, so n = 1 is excluded.)
- S_n fits: L is infinite, so its tokens fit inside a longer path, with room for z at both ends.
- S_n does not depend on the world. It is a tautology if n ∈ L and a contradiction otherwise. So a decision procedure for tautologyhood would decide L.

**Relativization.** In Φ's descriptions (D.4) and D.2's families, relativize every object quantifier and every described object to Sep: (Ey)(…) becomes (Ey)(Sep(y) . …), and D(x) becomes D(x) . Sep(x).

- Without this, U_1 would also hold of every path vertex that has an in-edge.
- With it, every object variable ranges over Φ's objects. A form variable in an atom with a Φ object never admits Q, because the instance has no sense.
- So these formulas read Φ's part exactly as in Φ. Their fitting placements are Φ's, with the Sep conjuncts placed at the same tokens.

**Path vertices.** Let Chain_n(φ; x_0, …, x_n) be the matrix of S_n. Then P_{n,k}(x) := (Eφ)(Ex_0 … x_{k−1}, x_{k+1} … x_n)Chain_n(φ; x_0, …, x_{k−1}, x, x_{k+1}, …, x_n).

- P_{n,k} is true exactly of v_{n,k}, because one path has each length and paths are rigid.
- It fits on a longer path. Its doubled 5.5321 sentence fits with the copies on two distinct longer paths, and its fully named instances fit because tokens are not fixed by names (C.4).

**The other twelve axioms.**

- **A4:** {0,1}^𝔸.
- **A5:** χ\* exists.
- **A16:** Φ's relativized descriptions and the P_{n,k}.
- **A17:** D.2's relativized families, plus the edge bits E_{n,k} := (Eφ)(Ex)(Ey)(P_{n,k}(x) . P_{n,k+1}(y) . φ(x, y)). Only Q admits φ, so E_{n,k} reads Q(v_{n,k}, v_{n,k+1}).
  - Aut(Φ ⊔ P_L) = Aut(Φ), because Sep separates the parts and the paths are rigid with distinct lengths.
  - Equal invariants therefore give an isomorphism, as in D.2.
- **A18:** D.3 on the subspace with every P_L bit true. The isomorphs of χ\* are χ\* and χ†, since the swap acts on Φ's part only. D.3.3 applies.
- **A7:** a finite situation's states on P_L are copied onto longer paths, one distinct path per depicted path and at the same offsets. Those on Φ are copied onto fresh units (D.5). Names stay injective, and token and target states are disjoint, so hereditary A6s holds.
- **A6a, A6s, A8:** as for Φ: tokens are frame states, relocation is as in A7, and the definitions are unchanged.
- **A13:** v_{n,k} occurs with its neighbours on the path.
- **A14:** every state is binary on distinct objects.
- **A19:** at the all-false world, swap(a, b) is an automorphism that fixes the world.

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

**Why a new frame class** (heuristic; these observations are not used in the proofs below).

- In every unit frame of Lemma G, A17 holds: units are described, their finite types are read, and a finite hub symmetry is fixed by compactness over finite joint types (D.2's OR argument).
- Frames whose identical units each carry infinitely many unordered markers fail A17, but they fail A18 as well. Describable types differ by finitely many markers, so a finite alteration can swap two units.
- So failing A17 needs infinitely many interchangeable units whose types differ at infinitely many rigid positions.
- A11 needs those positions to be told apart only by counting, never by an incidence chain. A chain with series descriptors allows lockstep comparison, which makes tautology undecidable.

Ξ therefore has two levels: columns are interchangeable, and within a column, levels are fixed by marker count.

**Frame Ξ** is defined in B.3, where Lemma G2 proves A11. A proposition's truth at W depends only on its profile at W.

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
- c_u: D_u(x) := ⋀\_{j≤u} Bit_j(x) . NBit_{u+1}(x). The prefix 1^u 0 is unique to β_u; g has no false out-edge; leaves have no out-edge.
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

**D12 at χ\*.** Write CGT(W) for the set of completely general truths of W. Suppose CGT(W) = CGT(χ\*). The following sentences have sense and hold at χ\*, hence at W:

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

Steps 2 and 4 infer uniqueness from true 5.5321 sentences, and step 3 uses ~(Ex)NBit_1(x). Both need the fully named instances to be admitted (note 40): D_g(g), D_g(c_u), D_u(c_v), D_u(c_w), their doubled forms, and NBit_1(c_u). They are admitted: the name tokens sit at distinct column objects (and at g for g), the inner y-binders at sub-leaves of the token columns, and the counting sources at g.

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
- **A17:** MC′\_{i,k} := (Ew)(U_i(w) . (Eu)(Ep_1 … p_k) ⋀\_j (St(p_j, u, w) . p_j(u, w))). Aut(ζ) = ∏\_i Sym(f_{i,1..i}), and equal counts give an automorphism.
- **A18:** marker permutations fix χ\* (all true), so the only world with the completely general truths of χ\* is χ\*.
- **A13, A14, A4, A5, A6a, A6s** (relocation), **A7** (unit shift) and **A8:** as for Φ.

## Appendix C: formal-series decidability

This appendix gives the definitions and argument needed for the A11 theorem stated in Appendix A. All bounds refer to one complete finite input. No finite quotient uniform over contexts with arbitrarily many additional names is asserted.

### C.0 Terms

- **G\*** is the grammar of C.1: expressions built from atoms by N over finite lists, over one-letter abstractions and over series descriptors [B, x, C], with C.1's map discipline. A G\* sign is *admitted* when every stipulated series step, nested steps included, is defined. A11 is decided for closed, meaningful, admitted G\* signs; admission is promised, not tested.
- **Map-admissible:** a sorted, correctly scoped expression whose required series substitutions, nested ones included, have well-defined maps. It need not have sense: a generated term may fail its own fitting or exposed-atom test and be excluded by C-nv while remaining map-admissible.
- **Closure, V, N_br.** A descriptor's closure is the least set of letters and names that contains:
  - B's and C's free letters and names outside the holes;
  - the images of an enclosing series' closure, for holes of that series inside the bracket.

  It is closed under the hole maps. V is its set of free letters, less the letters bound above a hole; N_br is its set of names.
- **H1 words:** the entries of a hole's written image μ_j(V ∪ N_br), identities included. Each is a letter or a name, written at the hole as a word of the sign. Map sources are not free at the hole.
- **Declaration names:** names that occur in a hole's written image. They count among the original names n.
- **Idle unit:** an entry of a written image, or a binder, that reaches no filler after a substitution. Normalization deletes idle units and nothing else.
- **Own holes:** the hole letter x of a descriptor itself, as against holes of enclosing series that occur inside it.
- **Bag:** a node's set of free object and form letters. The **augmented live bag** adds the node's names, and at a binder the binder letter.
- **Live boundary:** the identities a subexpression exposes to its context: free letters, names and active parameter roles. A **boundary-role chart** indexes which exposed identity plays which role. Auxiliary charts index intermediate composites.
- **Port reindexing:** renaming the rows of a record when a hole map μ identifies or permutes boundary roles (C.6).
- **Profile, cap b, H_b, M_P:** C.3–C.5.

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

These tables describe unanchored existential fitting. They do not assert equivalence when a token is externally fixed to a small-capacity Φ unit. Semantic names do not impose such pinning.

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

The frame, world space and axioms are those stated in the paper. This appendix supplies the finite descriptions, fitting witnesses and actual-world proof used in Appendix A. No decidability oracle is a premise.

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

Write Δ(W)={s∈𝔸 : W(s)≠χ\*(s)}. A truth-changing alteration W is minimal when no W′ with Δ(W′) a proper subset of Δ(W) changes the same proposition from its value at χ\*. Minimality here is by inclusion, not by numerical cardinality.

Let p change truth between χ\* and W, and suppose W has the same completely general truths as χ\*. By A17 and the frame automorphism calculation, W is either χ\* or χ†=swap(a,b)(χ\*): all markers are true, so marker permutations make no difference. The first possibility cannot change p. The difference D between χ\* and χ† is infinite.

Both worlds lie in G. At χ† choose a basic finite-coordinate neighborhood on which p has the same truth value relative to G. Flip χ\* only on the finitely many coordinates of D needed to enter that neighborhood. The result χ' is in G by invariance, and p at χ' equals p at χ†, differing from p at χ\*. Its change set is a finite proper subset of D. Therefore χ† was not an inclusion-minimal alteration changing p. This proves A18.

The argument does not assume minimal alterations always exist. It proves the required statement for every alteration that is minimal. It also does not infer finite sensitivity of a Borel function at arbitrary points.

#### D.3.4 Optional forcing presentation

The forcing presentation specifies a pair Cohen-generic [Coh1963] over a countable transitive M coding the signs. If such an M is supplied with the relevant Borel codes, its generic points form a comeagre subset of X. Intersecting that set with G still gives a permissible χ\*. This is an optional presentation of the actual-world choice; the Baire proof above already establishes existence.

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

For D_b reverse the final two orientations. The two-way pair forces an R-form; U_i0 and the incoming edge then force R_i0. Its actual orientation selects a for D_a and b for D_b. Crucially, there is no Rf conjunct here: reinstating it would make Rf's four tokens exhaust the support {h, o_m, a, b} of p's token R_m, so p(x, y) could not be placed.

At the named satisfying instance place x at a, w at a fresh o_m, p at R_m, the incoming-edge binder at h, the counting blocks at h' and markers, and the reverse-edge binder at b. The D_b case uses the same fitting pattern. All named successful prefixes can be realized with fresh target-disjoint forms. Thus the descriptions really admit their unique intended objects; they are not merely first-order formulas that become empty under C-nv.

A16 also demands sense of the 5.5321 uniqueness sentence, not just unique truth. For a description φ, the sentence is (exists x φ(x)) and not (exists x,y (φ(x) and φ(y))), with the stipulated exclusive quantifiers. For U_i the two copies can use distinct fresh leaf units. For h,h' and D_a,D_b place the two outer argument binders at a and b. Each copy's inner reverse-edge binder can use the other token because the other outer argument is absent from that inner binder's local body. Counting and off-edge blocks use fresh units as above. At this written stage the outer arguments are bound letters, not two global name reservations. Hence the doubled sign fits.

Existence holds by the successful single instance. The doubled existential cannot have an admitted true witness with two distinct object values: each component can be true only of the one selected object, and N+ excludes equal values. Some instantiated doubled ranges can be empty, but that does not invalidate the meaningful written uniqueness sentence or its true negation. This verifies both unique truth and sense of the uniqueness sentence. Therefore A16 holds at the same χ\* used for A18.

### D.5 The remaining axioms

A4: Λ is stipulated to be all of {0,1}^𝔸. Selecting χ\* inside X does not remove any other worlds.

A6a: M = 𝔸: all sign-medium states are frame states by fitting, including written descriptor tokens. This is not replaced by a new requirement that every medium state be true in the selected actual valuation. Logical operation signs have no additional projected state as specified in the signature.

A6s: The picture class excludes any nonempty invariant subset of the finite token medium under its projection. For finite D this is the no-directed-cycle condition. It is enforced in admissibility, rather than deduced for every arbitrary projection. The fresh-copy construction below shows it does not block A7. The finiteness premise is explicit in the picture definition (Signature).

A7: Let s be a nonempty finite situation. It uses finitely many units and finitely many markers in each. Choose distinct fresh unit indices large enough to accommodate those markers. Keep a,b,h,h' fixed, transport leaves and R-forms to those units, and transport markers injectively. This gives a token copy of the situation's finite state support, preserving every shared object/form and incidence. Name it and use the conjunction of the literals required by s. Projection from the copy onto the original support is well defined and bijective there; its token forms and target forms are disjoint, so it satisfies hereditary A6s. The literal signs have exactly s as their represented situation. If medium valuation at a witnessing world is required, A4 permits the required finite valuation. No unproved disjoint-copy property for arbitrary frames is assumed.

A8: Choose the stipulated finite, uniform, well-founded definition discipline and hygienic notation; expand definitions under X47. The grammar's future map-legality promise is syntactic and world-independent. A8 does not supply, and this proof does not claim, an algorithm deciding that infinite promise. Definitions do not depend on the truth of the expressions being defined.

A13: a,b occur together; h occurs with each o_i; h' occurs with each o_i through its nonempty marker set; every o_i therefore occurs with another object.

A14: Every displayed state has exactly two distinct object entries.

A19: At the all-false world the global swap(a,b) is an automorphism of both frame and valuation. Name-free formulas are equivariant: atomic incidence and truth, token fitting, N+, own-instance filtering, legal substitutions and normalization all transport under this automorphism. Structural induction and the finite-index series induction preserve sense and truth. Thus a and b have matching sense and truth for every name-free one-object formula. Their difference in the actual world is irrelevant: A19 asks for some world.

A11: Use the theorem of Appendix C. It depends on the frame and full world space, not on computing the selected χ\*. No actual-world oracle enters the decision procedure.

## Appendix E: concordance

Every one of the 526 propositions of the 1922 printing is listed below with its class and its selected reading. This is the evidence for the spanning claim (note 2). No proposition is violated. Each is one of the following:

- a source of an axiom or a commitment: 20 and 5;
- a definition: 108;
- notation: 9;
- derived: 264;
- an expressibility limit: 41;
- a consistent remark: 79.

Fourteen are restricted.

**Legend.**

- **A4–A19**: a source of that axiom.
- **S1, S3, S4**: a source of that commitment.
- **DEF**: a definition.
- **THM**: derived in *TLP*; premises after ←.
- **UNS**: an expressibility limit. What it says cannot be said is, in *TLP*, what shows (a metatheorem).
- **NOT**: notation or convention.
- **REM**: a remark (restatement, illustration, analogy or example) with no further content.
- **R**: restricted, i.e. read narrowly (the table of restricted propositions).
- **V2**: witness selected at grade V2 (note 2).

The readings follow the ledger's proposition tags, normalized to this paper's numbering: retired axiom numbers are replaced by their derivations. X, E and J numbers give provenance in the ledger. DE and EN refer to the German and English texts of 1922. V1–V3 grade how well the alternative witness admits the selected reading.

- **1** · DEF · world := W, the obtaining states of affairs (content supplied at 2.04)
- **1.1** · THM · facts are true situations over 𝔸, so the world is fixed by χ\* on 𝔸, not by O; W ⊆ 𝔸 is its positive part. O is world-invariant, so things cannot tell worlds apart  ← S1, DEF fact
- **1.11** · THM · W plus closure fixes χ\*  ← 2.04, 2.063
- **1.12** · THM · 𝔸 \ W = χ\*^-1(0)  ← 1.11, S1 (A fixed in advance)
- **1.13** · REM · world as χ\* (facts in logical space); W and χ\* interdefinable  ← 2.063
- **1.2** · THM · unique decomposition into one-atom facts (true one-atom situations, positive or negative; DE "zerfaellt in Tatsachen")  ← DEF fact, S4
- **1.21** · THM · closure under single flips; its converse would need a finitary constraint on worlds (S2), which TLP does not adopt (X45)  ← A4
- **2** · DEF · fact := nonempty true situation. Positive fact := one assigning only 1 (2's literal "Bestehen"); 2.06 admits negative facts
- **2.01** · DEF · state of affairs := configuration kappa(a) of objects ("Verbindung von Gegenstaenden"; S4). A14-compatible: the plural alone does not carry A14 (X13); the reciprocals do (2.03-2.032, 2.14, 2.15, 4.0311).
- **2.011** · THM · F(o) nonempty (D3; Mudersbach Axiom 5)  ← A13
- **2.012** · S1 · forms are world-invariant (F not indexed by world)
- **2.0121** · A13 · every object can combine with others ("Verbindung mit anderen" / "connexion with other things", V1): it occurs in some state of affairs together with a different object ("im Verbande des Sachverhalts"), so with D1, |O| >= 2. Mixed (E11): the first sentence and parenthesis come to D3, S1, A4 (THM). The content sentence is a limit in form ("so koennen wir uns keinen Gegenstand ... denken"), with A13 as its formal content
- **2.0122** · THM · V2 · objects are constant, yet occur only in configurations  ← S1, D3; parenthesis fwd 3.3. Versions: EN "in all possible circumstances" selected; DE "in allen moeglichen Sachlagen" is V2 (read as "all sorts of situations")
- **2.0123** · THM · knowing o means knowing F(o): F is internal  ← DEF F, S1
- **2.01231** · DEF · int(o) := F(o); ext_chi(o) := obtaining states containing o, with o's slots. "Obtaining" makes ext positive-only; 2.06 counts the non-obtaining as negative facts, so for 2.02331 ext is χ\* restricted to 𝔸_o (X21). TLP takes the features invariant under the automorphisms of the frame and χ\* (D15)
- **2.0124** · THM · 𝔸 = union of the 𝔸_o  ← DEF 𝔸_o, S4 (kappa(a) nonempty)
- **2.013** · THM · "empty space" world exists (all of 𝔸_o false)  ← A4; nonempty space ← D3
- **2.0131** · THM · form-level reading consistent with A4; world-level reading (at least one colour; DE "eine" also admits exactly one) contradicts A4 if colour ascriptions are elementary  ← A4
- **2.014** · THM · every situation is drawn from the union of the 𝔸_o  ← 2.0124 (concerns Sachlagen)
- **2.0141** · DEF · form of o := F(o), with o's slots. "Same form" is 2.0233's DEF: some g in Aut(F) with g(a) = b
- **2.02** · THM · objects are simple  ← 2.021
- **2.0201** · DEF · contextual (Russellian) definition of complexes; analysis well-founded  ← A8
- **2.021** · THM · objects not composite: composites can fail to exist, substance cannot  ← S1, A4
- **2.0211** · THM · sense independent of χ\*, given substance  ← S1, A8
- **2.0212** · THM · without substance, no pictures  ← 2.0211
- **2.022** · THM · every imagined world shares the real world's form  ← S1
- **2.023** · DEF · form := (O, F)
- **2.0231** · THM · substance fixes Λ, not χ\*; contingency |Λ| >= 2  ← D1, S1, D3, A4
- **2.0232** · REM · "colorless": int(o) contains no determinates (metaphor)
- **2.0233** · DEF · same form := same Aut(F)-orbit. THM: same-form objects differ in bare identity  ← S1
- **2.02331** · THM · D15, derived from A16 (X22). Horn 1: every object fixed by the automorphisms of the frame and χ\* is singled out by one general description. Mixed (E11): horn 2 and "Denn" are UNS: indiscernibles cannot be singled out or named apart. With D15, describable iff fixed (X20). Judgments J2, J4, J5. A de re reading of horn 1 (with 2.06) also follows from A16 (X21)  ← 5.526
- **2.024** · S1 · substance independent of what is the case: constant domain (S5, Barcan)
- **2.025** · DEF · substance = form + content (content = bare objects)
- **2.0251** · THM · determinables in F, determinates in χ; if determinates are atoms, their exclusion contradicts A4  ← A4
- **2.026** · THM · O nonempty (the antecedent, a fixed form, comes from 2.022-2.023). D1: A19 gives two distinct objects  ← 5.5302
- **2.027** · THM · the fixed = the existent = the object  ← S1, S4 (A and F are functions of O)
- **2.0271** · THM · objects fixed, configuration varies  ← S1, DEF Λ
- **2.0272** · DEF · configuration of objects = state of affairs (= 2.01; plural: A14)
- **2.03** · S4 · objects hang together with no glue; slot rendering vs. labels is NOT (inter-translatable); "ineinander": a source of A14
- **2.031** · DEF · structure := dom kappa(a); distinct states have distinct maps (D2). DE "verhalten sich ... zueinander" (objects relate to one another; A14); Ogden "are combined" is V1
- **2.032** · DEF · structure of a state of affairs (= 2.031): how the objects hang together (A14)
- **2.033** · DEF · form of states of affairs := admissible structures S
- **2.034** · THM · structure of a fact = structures of its states  ← DEF fact
- **2.04** · DEF · world := W; with A5 (χ\* exists)
- **2.05** · THM · = 1.12  ← 2.04, S1
- **2.06** · DEF · reality := χ\* (positive and negative facts)
- **2.061** · A4 · independence: Λ = {0,1}^𝔸, i.e., C empty
- **2.062** · THM · pairwise independence (strictly weaker)  ← A4
- **2.063** · THM · world = total reality, given fixed A  ← 2.04, 2.06
- **2.1** · DEF · picture P = (D, ρ, tau) in Pi; D a nonempty finite set of states of affairs (the medium); sense at χ := sigma_{P,χ} = (χ|D) o r^-1
- **2.11** · DEF · V2 · sense := sigma_P; place := [[sigma_P]]. V2: Ogden's "the facts" (plural, factive) for "die Sachlage" (singular, possible); it echoes 1.13 rather than 2.202-2.203
- **2.12** · REM · picture as model (sigma extends to worlds)
- **2.13** · DEF · ρ total on picture elements; each element stands for one object (with 2.14-2.15: A14)
- **2.131** · DEF · = 2.13
- **2.14** · DEF · configuration pi := χ|D (χ the world considered; actual: χ\*)
- **2.141** · A6a · media are facts of the world they depict (M = world)
- **2.15** · DEF · structure; pictorial form (r well-defined and injective)
- **2.151** · DEF · strict pictorial form: r carries pi_D(Sol C) bijectively onto pi_r(D)(Sol C) (projections, not the edges of C inside D). Into-half: 3.02; onto-half: 2.171
- **2.1511** · REM · contact with reality via ρ alone
- **2.1512** · REM · ruler image (returns in 1929 as the one-hot scale)
- **2.15121** · THM · (= 2.223) truth needs χ\* only on r(D)  ← DEF 2.222
- **2.1513** · DEF · the pictorial relationship belongs to the picture: P = (D, ρ, tau). Only the medium is a fact (A6a); the projection is not a configuration
- **2.1514** · DEF · pictorial relationship := ρ
- **2.1515** · REM · feelers
- **2.16** · THM · picture and depicted share something  ← 2.151
- **2.161** · THM · partial embedding of object-forms. "das eine ... des anderen" needs two relata; supports A6s  ← 2.151
- **2.17** · THM · pictorial form is independent of χ\*, so serves both truth values  ← DEF
- **2.171** · THM · within a medium, every configuration over r(D) is depictable  ← 2.151 (onto-half)
- **2.172** · UNS · pictorial form is not a situation, so not depictable (type distinction)
- **2.173** · THM · R · no self-depiction: r(D) and D are disjoint in the elementary case. Two equally plain readings (X40): material (the picture is not among the states it represents; with 4.01 and 2.201) and standpoint (the outside is the form; "darum ... richtig oder falsch" gives bipolarity). RESTRICTED (X41): kept as A6s (no picture is its own object). s and p v s are not outside their object and cannot be false where they exist  ← A6s
- **2.174** · UNS · = 2.172 for representational form (DE "Form der Darstellung"; Ogden's "form of representation" also renders "Form der Abbildung", so in EN it restates 2.172)
- **2.18** · DEF · logical form := what every pictorial form preserves (incidence + hypercube)
- **2.181** · DEF · logical picture
- **2.182** · THM · every picture is logical (forgetful map is total)  ← 2.18
- **2.19** · A7 · adequacy: every nonempty finite situation is the sense of some picture at some world. The whole world only collectively (D finite; finite A: D21)
- **2.2** · REM · 2.18 restated
- **2.201** · DEF · sense is a partial assignment (confirms Sachlage)
- **2.202** · THM · [[sigma]] nonempty  ← 2.203
- **2.203** · THM · weak reading ← A4 (finite independence); strict reading ← DEF 2.151
- **2.21** · THM · bivalence  ← DEF truth, A5 (χ\* total)
- **2.22** · THM · sense independent of truth  ← DEF
- **2.221** · DEF · sense
- **2.222** · DEF · truth: sigma_P ⊆ χ\*
- **2.223** · THM · comparison is finite: χ\* on r(D) only  ← DEF 2.1 (D finite), DEF 2.222
- **2.224** · THM · R · truth not recognizable from the picture alone. No picture's truth value is fixed by its own configuration. RESTRICTED: read for the picture as a token (J-tok), s and p v s fail it. Kept: the type reading, that no picture's sense fixes its truth value  ← 4.01, A4
- **2.225** · THM · no a priori true picture. Diagonal reading (true wherever its configuration obtains): From D6b; (X41, J-apriori): not a reading of "a priori wahr". s is true wherever its sign exists, but knowing that requires perceiving the sign, which is experience (cf. 5.634). Plain reading, extensional ([[sigma]] ≠ Λ)  ← A4, DEF 2.1 (D nonempty)
- **3** · DEF · thought := logical picture
- **3.001** · DEF · V2 · thinkable := depictable (by some picture at some world). DE "ein Bild ... machen" selected; Ogden's "imagine" is V2
- **3.01** · THM · true thoughts jointly picture χ\*  ← A7 (atomic case; thoughts as types), A6a
- **3.02** · THM · thinkable implies possible  ← weak: A4; strict: 2.151 (into-half)
- **3.03** · THM · senses of thoughts (pictures) lie in P(Λ) \ {empty, Λ}: we cannot think anything unlogical. Tautology and contradiction have the null sense (LI reading)  ← 2.203, 2.225
- **3.031** · THM · logic excludes no point of {0,1}^𝔸  ← A4
- **3.032** · UNS · contradiction is ill-typed for pictures (sigma must be a function)
- **3.0321** · REM · physics = constraints on points of Λ; geometry/logic = index structure (A, H)
- **3.04** · DEF · a priori correct := the thought's possibility ensures its truth. (X41, J-apriori): the diagonal reading is not a reading. Extensional [[sigma]] = Λ excluded  ← 2.225
- **3.05** · THM · a priori knowable only if truth is recognizable from the thought itself: an "only if". Extensional [[sigma]] in {empty, Λ} excluded  ← 3.03
- **3.1** · DEF · proposition := picture in a perceptible medium
- **3.11** · DEF · projection (ρ, tau), supplied by thinking
- **3.12** · DEF · propositional sign; proposition = (S, ρ, tau)
- **3.13** · A6s · form of sense = orbit; content = ρ. THM: the sign fixes form, not content. Mixed: the parenthesis ("heisst") is DEF; sentences 1-3 and the last are assertions about the Satz of 3.12. (Sit) reads s1-s2. (X41, J-3.13): plain reading (Sit): the projected situation, the sense, is not part of the Satz, only its possibility. Source of AX6s. The tag reading is weak (the projection, ρ included, belongs to the Satz); (Act) is co-plain at most  ← DEF
- **3.14** · A6a · propositional sign is a fact (A6a for signs). Mixed: s1 ("besteht darin, dass ... seine Elemente, die Woerter ...") is DEF; s2 (A6a's source) an assertion. S1 grounds (7b) (a token for each propositional letter of a bracket) and (H1) (what a hole writes are words)
- **3.141** · THM · a sign is not the set of its elements  ← 3.14
- **3.142** · THM · sense needs a configuration; a set of names has none  ← DEF sense
- **3.143** · THM · against Frege's composite name: names map into O, propositions into P(Λ). An assertion: print obscures that the Satzzeichen is a fact  ← 3.14
- **3.1431** · REM · furniture example: the medium is arbitrary
- **3.1432** · S4 · relation signs belong to tau, not ρ: relations are not objects (textual source for S4's slots; C3)
- **3.144** · UNS · situations cannot be named (Sit ∩ O empty); polarity as arrow
- **3.2** · THM · a completely analysed expression exists  ← A8, D9 (THM)
- **3.201** · DEF · simple sign; completely analysed
- **3.202** · DEF · name
- **3.203** · DEF · meaning := ρ(n); "A" = "A" is NOT (ρ on sign types)
- **3.21** · THM · configuration correspondence  ← DEF picture (2.15)
- **3.22** · REM · = 2.131
- **3.221** · UNS · "what" objects are is invariant across Λ, hence unsayable  ← S1
- **3.23** · A8 · analysis well-founded, iff sense determinate
- **3.24** · THM · complexes: inclusion of senses; false if nonexistent; descriptions give non-cylinder senses, explicit contractions multi-coordinate cylinders  ← 2.0201, A8
- **3.25** · THM · sign level ← A8 (Newman's lemma); sense level ← A4 + primitive move graph (Sabidussi-Vizing)
- **3.251** · REM · = 3.23 + 3.141
- **3.26** · DEF · names are primitive (sinks of the definition graph)
- **3.261** · THM · definition graph is a DAG; defined and primitive signs signify differently. A defined sign signifies through its definiens, so a sign with defined signs fits, and has sense, as its translation  ← A8
- **3.262** · UNS · category = incidence profile; what the signs do not express, their use shows
- **3.263** · THM · elucidations fix ρ only up to the automorphisms of the frame and χ\*: sense needs r to land in the frame (S3), truth fixes χ\*. A weakening to the automorphisms of the medium would assume frame-blind elucidations, which S3 excludes  ← S1, D9 (THM)
- **3.3** · THM · context principle  ← 3.142, 2.0123
- **3.31** · DEF · expression
- **3.311** · THM · an expression determines its class of propositions  ← DEF
- **3.312** · DEF · presentation by variable
- **3.313** · DEF · propositional variable
- **3.314** · THM · all variables are propositional; quantification substitutional (needs D9 (THM))  ← DEF
- **3.315** · DEF · logical prototype := pattern with all arbitrary constants variabilized
- **3.316** · DEF · the stipulation is the variable
- **3.317** · DEF · stipulation is syntactic and extensional
- **3.318** · THM · compositionality  ← recursive DEF of [[.]]
- **3.32** · DEF · sign := perceptible part of a symbol
- **3.321** · REM · one sign, several symbols
- **3.322** · THM · sign shape carries no semantic information  ← DEF
- **3.323** · REM · ordinary-language examples ("is")
- **3.324** · REM · philosophy full of such confusions
- **3.325** · DEF · correct notation: no sign in two symbols. (X43, J-3.325): within a propositional sign, each element (token) belongs to one symbol category, so a name and a variable never share a token; binders may share (one symbol, the variable). Until "injective projection in which shape determines category". Mixed: s1 (the requirement) an assertion; s2 ("Eine Zeichensprache also, die der logischen ... Syntax ... gehorcht", the first occurrence of "logische Syntax") a gloss, DEF. X43 rests on s2 being DEF or on both (St) marks lying below kind 2
- **3.326** · THM · symbol recognized by use (category = substitution class)  ← 3.262
- **3.327** · REM · = 3.326
- **3.328** · THM · meaning = role; empty profile means no meaning  ← 3.262
- **3.33** · A8 · syntax "must admit of being established without mention being thereby made of the meaning of a sign" (DE "aufstellen lassen": formulable, drawn up): settled without meaning. Effective syntax would be a strengthening, not a reading, and is not adopted
- **3.331** · REM · critique of Russell
- **3.332** · UNS · no proposition can say anything about itself, i.e. about the complex that is its own sign, which it could do only by describing it (3.24); its sign would then contain itself (containment reading, X40). Follows from well-founded finite signs (A8) and 3.144, so it sources no axiom. A support reading (the support of its sense disjoint from its medium; the retired axiom A6d) is at best equally plain (X40). Mixed (X46): the main clause a limit; the reason clause an assertion; the parenthesis a gloss
- **3.333** · THM · occurs check: s = s -> t has no finite solution  ← 3.33
- **3.334** · THM · syntax rules follow from categories  ← 3.262
- **3.34** · DEF · essential vs. accidental features
- **3.341** · THM · essential := invariant on the sense fiber. An assertion: "das Wesentliche" is fixed at 3.34  ← 3.34
- **3.3411** · DEF · real name := invariant of all symbols for o (F(o) + bare identity)
- **3.342** · THM · arbitrariness only up to a stabilizer  ← 3.341
- **3.3421** · REM · possibility of notation discloses essence (Erlangen)
- **3.343** · DEF · definitions = translation rules. THM: correct languages inter-translatable  ← 2.18, 2.151
- **3.344** · DEF · what signifies := invariant under substitution
- **3.3441** · THM · functional completeness of {not, or}  ← every finite-arity truth function has a DNF; "and" by De Morgan
- **3.3442** · A8 · analysis uniform across contexts
- **3.4** · THM · a place exists once the constituents exist  ← S1, S4, 2.0124
- **3.41** · DEF · logical place = sign + coordinates
- **3.411** · REM · a place is a possibility
- **3.42** · DEF · place extends to Boolean combinations. THM: closure in a fixed P(Λ)  ← A4. Expressible places are at most ℵ0, since signs are finite strings over countably many names (A11)
- **3.5** · DEF · thought = applied, thought-out propositional sign
- **4** · THM · thought := proposition with sense (= 3, 3.5; sense in P(Λ) \ {empty, Λ}). An assertion: it identifies terms fixed at 3, 3.5 and 3.12  ← 3, 3.5
- **4.001** · DEF · language := Prop, the totality of propositions
- **4.002** · REM · colloquial language disguises logical form
- **4.003** · REM · most philosophical "propositions" are nonsense (unsinnig), not false; cf. 5.4733
- **4.0031** · REM · philosophy as critique of language; Russell: apparent form need not be real form (cf. 2.0201, 3.24)
- **4.01** · THM · V2 · contingent propositions are pictures: extends DEF 2.1 to compounds, with sense in Clopen(Λ); "ein Modell der Wirklichkeit, so wie wir sie uns denken" (as we conceive it); Ogden's "as we think it is" is V2. An assertion: "Satz" is fixed at 3.12  ← 3, 4
- **4.011** · REM · score and phonetic script: symbolisms are pictures
- **4.012** · REM · aRb as likeness
- **4.013** · REM · apparent irregularities (sharps, flats) also picture
- **4.014** · REM · record, musical thought, score, sound waves share a logical structure (= 2.18, 3.343)
- **4.0141** · DEF · law of projection := rule of translation between media (= (ρ, tau), 3.11; cf. 3.343)
- **4.015** · REM · similes rest on the logic of representation
- **4.016** · REM · hieroglyphs to alphabet without loss of representational essence
- **4.02** · THM · the sense of a propositional sign is understood without explanation  ← 3.318
- **4.021** · THM · understanding a proposition = knowing the situation it presents  ← 3.318, 2.221
- **4.022** · DEF · shows := its sense [[phi]] is displayed by sign + projection; says := χ\* in [[phi]]
- **4.023** · THM · V2 · sense is a definite cut of Λ (fixed to yes or no); conclusions can be drawn from a false proposition (entailment is [[.]]-inclusion, independent of χ\*). V2: (b) "Beschreibung eines Sachverhaltes" / "description of a fact" are both loose (a proposition describes a Sachlage; Ogden's "fact" is factive). (a) Ogden drops "muss ... fixiert sein": V1. R9 closed: the paraphrase is Wittgenstein's own (Letters to Ogden O.2, p. 27). Read "fixed to yes or no", not "Yes/No suffices". The 1922 German prints "Der Wirklichkeit" (typo for "Die")  ← 2.21, 2.22, 3.23
- **4.024** · THM · understanding = knowing truth-conditions, independent of truth; compositional. Supports A6s (a self-depicting picture could be understood only by knowing that it is true)  ← 2.22, 3.318
- **4.025** · THM · translation is constituent-wise  ← 3.318, 3.343
- **4.026** · THM · meanings of simple signs must be given: ρ is not read off the sign  ← 3.322, 3.263
- **4.027** · THM · a proposition can communicate a new sense: each uses finitely many names, senses are unbounded  ← 3.318
- **4.03** · THM · a proposition says something ("sagt ... aus") only insofar as it is a picture ← 4.01, 4.027
- **4.031** · REM · a situation (Sachlage; Ogden: "state of affairs") is "put together for the sake of experiment" (= 2.11, 2.12)
- **4.0311** · DEF · ρ injective on the names of a proposition (one name, one thing; cf. 5.53); the names "untereinander verbunden": a source of A14
- **4.0312** · THM · fundamental thought: logical constants do not stand for ("vertreten") anything. Operation signs have no ρ-image; truth-operations act on senses (Boolean operations on P(Λ)), not on O  ← 4.4, 4.0621
- **4.032** · THM · a picture only insofar as articulated: an unarticulated sign has no configuration, hence no sense  ← 3.142
- **4.04** · THM · same logical multiplicity: names and depicted objects in bijection  ← 2.15, 4.0311
- **4.041** · UNS · multiplicity cannot itself be represented (= 2.172)
- **4.0411** · THM · a generality notation must record bound places, scope, and co-reference; each index notation loses one of the three  ← 4.04
- **4.0412** · REM · "spatial spectacles" fail for the same reason
- **4.05** · REM · reality is compared with the proposition (= 2.223)
- **4.06** · THM · true or false only as pictures  ← 4.01, 2.222
- **4.061** · THM · sense is independent of the facts, so true and false are not two sign-thing relations with equal rights. Supports A6s (a self-depicting picture's sense would be fixed by the facts it depicts)  ← 2.22
- **4.062** · THM · using p to mean ~p changes the sense to its complement, not the truth relation  ← 2.222, 4.0641
- **4.0621** · THM · ~ has no ρ-image: [[~~p]] = [[p]]; p and ~p have complementary senses and one reality  ← 4.4
- **4.063** · REM · black-spot simile; a proposition is not a name of a truth-value (= 3.144, 2.22)
- **4.064** · THM · affirmation and negation ("Bejahung", "Verneinung") presuppose sense; they do not confer it  ← 2.22
- **4.0641** · THM · V2 · denial determines the complementary place, [[~p]] = Λ \ [[p]]; that denial iterates shows the denied is already a proposition. V2: Ogden's "by saying" for "beschreibt"; "sagen" is technical (4.022, 4.1212), and with it ~p would say something about its own place  ← 4.4, 3.41
- **4.1** · THM · a proposition presents existence and non-existence of states of affairs: [[phi]] ⊆ Λ  ← 4.4
- **4.11** · DEF · natural science := {phi : χ\* in [[phi]]}
- **4.111** · REM · philosophy is not a natural science
- **4.112** · REM · philosophy as activity: elucidations, not propositions (cf. 6.54)
- **4.1121** · REM · psychology; theory of knowledge as philosophy of psychology
- **4.1122** · REM · Darwinism irrelevant to philosophy
- **4.113** · REM · philosophy limits the disputable sphere of natural science
- **4.114** · REM · limit the unthinkable from within: Prop is generated, not carved from a larger space (cf. 4.5)
- **4.115** · REM · the unsayable meant by displaying the sayable
- **4.116** · THM · whatever can be thought or said can be so clearly: every sense is a definite subset of Λ  ← 3.23
- **4.12** · UNS · logical form is not representable: representing it would need a medium outside the world  ← 2.172, A6a
- **4.121** · UNS · logical form mirrors itself in propositions; shown, not said (= 2.172)
- **4.1211** · THM · co-reference, contradiction and entailment are read off the signs (computed from sign + ρ), not asserted  ← 4.4, 4.0311
- **4.1212** · UNS · what can be shown cannot be said: Λ-invariants have no contingent sense  ← 3.03
- **4.1213** · REM · a correct symbolism as the right logical conception
- **4.122** · UNS · internal (formal) properties and relations are invariant across Λ; they show in propositions, not asserted by them  ← S1, 4.1212
- **4.1221** · DEF · feature := internal property of a fact
- **4.123** · DEF · internal := unthinkable that its object lacks it (invariant across Λ). The example (brighter/darker shades) is an internal relation among determinates: 1929 pressure
- **4.124** · UNS · ascribing or denying a formal property is equally nonsense (unsinnig)  ← 4.122
- **4.1241** · UNS · forms are not distinguished by predication  ← 4.124
- **4.125** · UNS · internal relations between possible situations show as internal relations between the propositions presenting them  ← 4.122
- **4.1251** · REM · the dispute over internal vs. external relations disappears
- **4.1252** · DEF · formal series := series ordered by an internal relation (numbers; aRb, (Ex)(aRx.xRb), ...); successor. S3's series (assertion, 4) is written in G\* with name variabilization; judged by the union (X35)
- **4.126** · DEF · formal concept := propositional variable whose constant feature is the formal property. UNS: falling under it is not expressible by a proposition, and it is not a function. Mixed: DEF and UNS  ← 3.313, 3.315
- **4.127** · DEF · the variable signifies the formal concept; its values signify the objects under it
- **4.1271** · THM · every variable is the sign of a formal concept  ← 3.313, 4.126
- **4.1272** · UNS · R · "object" is a formal concept (variable name x). "There are n objects" and "there are ℵ0 objects" are nonsense. With exclusive quantifiers, "there are n objects which phi" is sayable, but the bare count has no contingent sense (S1). It shows in which exclusive-quantifier sentences are tautologies. RESTRICTED: "there are n objects which phi" is sayable where the n-fold instances fit; under X31's strict token rule it is not for Cyc in Φ. Mixed: s1 an assertion (from 4.127); s2 an assertion about expression; s3 its example (REM); the rest limits; the mark is (assertion, 4)  ← S1, 3.03, 4.126
- **4.12721** · THM · a formal concept is given with its objects; the concept and its instances cannot both be primitive  ← 3.262, 4.126
- **4.1273** · THM · "b is a successor of a" needs the general term of a formal series (first term + operation), i.e., the ancestral: not a finite truth-function, not first-order (compactness). The Frege-Russell definition is circular. The last sentence (assertion) grounds name variabilization; G\*'s terms differ from the printed ones under N+, judged by the union (X35)  ← 4.1252, 4.126
- **4.1274** · UNS · existence questions about formal concepts are nonsense (unsinnig). Not violated by A14, a frame axiom, not a proposition (as D1 with 4.1272; X18)  ← 4.126
- **4.128** · THM · R · logical forms are anumerical: no number pre-eminent. RESTRICTED (J6): ℵ0 is singled out by A16's cap and A11's countable names as the bound on what completely general signs can fix or name (X45, X49)  ← A6a, A6s
- **4.2** · DEF · sense := agreement and disagreement with the truth-possibilities: [[phi]] ⊆ Λ (= 2.11 for compounds)
- **4.21** · DEF · elementary proposition := picture with D = {d}, sign present (pi(d) = 1), sense {r(d) -> 1}
- **4.211** · THM · no elementary proposition contradicts another (fails under color exclusion, C nonempty)  ← A4, 4.21
- **4.22** · DEF · elementary proposition = concatenation of names: a slot map (S4; 3.14), with at least two names of distinct objects (A14)
- **4.221** · THM · analysis ends in elementary propositions. The unity question ("how the propositional connexion comes to be") is answered by S4: no glue (2.03)  ← 3.2, 3.25
- **4.2211** · THM · substance does not depend on finite analysis: O and 𝔸 nonempty even if facts and states of affairs are infinitely complex. D-S4's finiteness excludes the second hypothesis  ← D1, D3
- **4.23** · THM · names occur only in elementary propositions  ← 3.3, 4.221
- **4.24** · NOT · R · names x, y, z; elementary propositions fx, phi(x, y); p, q, r. RESTRICTED: "fx" is schematic notation, not a claim that single-object elementary propositions exist (A14; 5.554)
- **4.241** · DEF · a = b := sign a is replaceable by sign b (a rule about signs; a = b Def.). A defined sign and its definiens share fit and sense
- **4.242** · THM · a = b asserts nothing about the meanings of a and b  ← 4.241
- **4.243** · THM · understanding two names includes knowing whether they co-refer; "a = a" is not a significant sign (cf. 5.53-5.5352)  ← 4.241, 3.203
- **4.25** · THM · an elementary proposition is true iff its state of affairs obtains  ← 4.21, 2.222
- **4.26** · THM · all true elementary propositions describe the world completely  ← 1.11, 4.25, A7
- **4.27** · A4 · all 2^n combinations of n states of affairs are possible (K_n = sum_nu C(n, nu))
- **4.28** · THM · 2^n truth-possibilities of n elementary propositions  ← 4.27, 4.21
- **4.3** · THM · truth-possibilities = projection of Λ onto the depicted atoms  ← 4.25
- **4.31** · NOT · truth-table schemata
- **4.4** · DEF · Prop (finite stage) := truth-functions of elementary propositions. [[phi]] = union of agreeing truth-possibilities, an element of Clopen(Λ). Operation signs have no ρ-image; D_phi := union of the elementary media
- **4.41** · DEF · the truth-possibilities of the elementary propositions are the truth-conditions
- **4.411** · REM · elementary propositions are basic; general propositions depend on them (cf. 5.52)
- **4.42** · THM · 2^(2^n) truth-functions of n elementary propositions (as many distinct senses only under A4 with distinct atoms)  ← 4.4, 4.28
- **4.43** · NOT · mark T for agreement
- **4.431** · THM · a proposition is the expression of its truth-conditions; truth-values are not objects (against Frege)  ← 4.4, 3.144
- **4.44** · DEF · propositional sign := the sign formed by coordinating T with truth-possibilities
- **4.441** · THM · no logical objects  ← 4.0312
- **4.442** · THM · (TTFT)(p, q) is a propositional sign; Frege's assertion sign is meaningless. No proposition asserts its own truth: truth needs the projection, which is not a configuration  ← 2.1513
- **4.45** · THM · L_n = 2^(2^n) groups of truth-conditions, orderable in a series  ← 4.42
- **4.46** · DEF · tautology := [[phi]] = Λ; contradiction := [[phi]] = empty
- **4.461** · THM · R · tautology and contradiction are without sense (sinnlos): no truth-conditions. RESTRICTED: the null sense, which says nothing (cf. 4.4611's 0). "No sense at all" would contradict 4.5(iii)  ← 3.03, 4.46
- **4.4611** · THM · V2 · but not nonsense (unsinnig): part of the symbolism, as the sign 0 is part of arithmetic's (both are limiting cases; 4.466). Ogden's "not senseless" is V2 ← 4.4
- **4.462** · THM · not pictures: their senses are Λ or empty, not situations  ← 3.03, 4.46
- **4.463** · DEF · range := [[phi]]. Tautology leaves all of logical space, contradiction none. Calls logical space "infinite": textual support for A infinite. Mixed: DEF (first sentence), REM (the simile), assertion (the rest; "unendlichen" is weighed as an assertion, X7). Satisfied by the D21 (A6s)
- **4.464** · DEF · certain := [[phi]] = Λ; possible := contingent; impossible := empty (cf. 5.15)
- **4.465** · THM · p.Taut = p: identity of the symbol = identity of the sense  ← 4.4, 3.341
- **4.466** · THM · tautology and contradiction are exactly the propositions whose sense is invariant under every reassignment of meanings; their sign-combination corresponds to no combination of objects  ← A4, D21 (|𝔸| > n suffices)
- **4.4661** · THM · relations among the signs of a tautology are inessential to the symbol  ← 4.466, 3.341
- **4.5** · A7 · general propositional form, "such and such is the case": (i) Prop is generated (no unforeseeable form); (ii) every possible sense is expressed by one symbol (A7, per-situation); (iii) every symbol expresses a sense under some ρ (D10; tautologies: the null sense). Restricted in (X29: p v s had no admissible choice of meanings; HIGH ALERT #2, D10s). Mixed: the "das heisst" gloss of s1 is DEF, with (ii) and (iii) as definiens (J-4.5a); s1's hedge and s2-s4 are assertions; K's restriction of (iii) is (DEF, 1); K has no route through s3-s4 and 6 (J-4.5b). Unrestricted since D10 holds
- **4.51** · DEF · Prop := what can be built from all elementary propositions
- **4.52** · THM · propositions follow from the totality of elementary propositions plus the fact that it is the totality; generality needs the totality fact (cf. 5.52)  ← 4.51
- **4.53** · DEF · the general propositional form is a variable (cf. 6)
- **5** · DEF · propositions are truth-functions of elementary propositions; an elementary proposition is a truth-function of itself (= 4.4)
- **5.01** · DEF · elementary propositions are the truth-arguments of propositions
- **5.02** · THM · argument vs. index: the sense of ~p is a function of the sense of p, not an index in a name; against Frege's propositions-as-names  ← 4.431, 3.144
- **5.1** · THM · truth-functions can be ordered in series; basis of probability  ← 4.45
- **5.101** · DEF · truth-grounds := truth-possibilities that verify the proposition (16-row schema for two arguments)
- **5.11** · DEF · follows: the common truth-grounds of the premises are truth-grounds of the conclusion (∩ of premise senses ⊆ conclusion sense)
- **5.12** · DEF · p follows from q iff [[q]] ⊆ [[p]]
- **5.121** · THM · V2 · restates 5.12. V2: the German "des einen ... des anderen" with 5.12's order suggests the inverse inclusion; Ogden states the right one (q in p)  ← 5.12
- **5.122** · THM · if p follows from q, the sense of p is contained in that of q (content = excluded worlds)  ← 5.12
- **5.123** · THM · a world where p is true contains all of p's objects; entailment cannot be created separately  ← S1, 5.12
- **5.124** · THM · V2 · a proposition affirms ("bejaht") every proposition that follows from it. Not "says" in the sense of 3.332. V2 (E6b): Ogden's "asserts" for "bejaht"; it bites here, since consequences include tautologies, which say nothing (4.461)  ← 5.12
- **5.1241** · THM · V2 · p.q affirms p and q; opposed := no proposition with sense (sinnvoll: non-null sense) affirms both ([[p]] ∩ [[q]] = empty); contradicting = denying . V2: Ogden's "assert" (his word for "behaupten") for "bejahen" (affirm); also at 5.124  ← 5.12, 4.461
- **5.13** · THM · entailment is perceived from the structure of the propositions  ← 4.1211
- **5.131** · UNS · entailment is an internal relation; it exists with the propositions and needs no connecting proposition  ← 4.125
- **5.1311** · THM · in stroke notation the inner connexion is visible; inferring fa from (x).fx shows generality is in the symbol  ← 5.13
- **5.132** · THM · R · V2 · inference is justified by the two propositions alone; laws of inference are without sense (sinnlos) and superfluous. RESTRICTED as 4.461 (null sense). V2: Ogden's "senseless" is his word for "unsinnig" (4.003, 4.1272, 6.54), against "sinnlos" ("without sense" at 4.461)  ← 5.13
- **5.133** · THM · all inference is a priori: [[.]]-inclusion is independent of χ\*  ← 5.12, 2.22
- **5.134** · THM · from an elementary proposition no other elementary proposition can be inferred  ← A4, 4.21
- **5.135** · THM · no inference from one situation (Sachlage) to an entirely different one  ← A4
- **5.136** · THM · no causal nexus justifies such an inference (C empty)  ← A4
- **5.1361** · THM · the future cannot be inferred from the present; superstition is belief in the causal nexus  ← A4
- **5.1362** · THM · R · V2 · freedom of the will: future actions cannot be known now; knowing requires logical necessity; "A knows that p is the case" is without sense (sinnlos) if p is a tautology. RESTRICTED as 4.461. V2: as 5.132, "senseless" for "sinnlos"  ← A4, 4.461
- **5.1363** · REM · obviousness is no justification
- **5.14** · DEF · if p follows from q, q says more than p
- **5.141** · THM · mutual entailment means one and the same proposition  ← 5.12, 4.465
- **5.142** · THM · a tautology follows from all propositions; it says nothing  ← 4.46, 5.12
- **5.143** · THM · V2 · contradiction is the outer limit (bottom), tautology the substanceless centre (top) of the propositions. V2: Ogden's indefinite "something shared" for the definite "das Gemeinsame" (the reading needs a unique bottom); his comma also lets "which" attach to "propositions"  ← 4.46, 5.12
- **5.15** · DEF · probability r gives s := Trs : Tr. General form: mu([[r]] ∩ [[s]]) / mu([[r]]) (SIGNATURE: mu)
- **5.151** · NOT · counting T's in the 5.101 schema
- **5.1511** · THM · no special object for probability propositions  ← 4.441, 5.15
- **5.152** · THM · independent := no common truth-arguments. Two elementary propositions give each other 1/2 [ok]. Entailment gives 1; certainty is the limiting case. The corrected witness ("Zwei Elementarsaetze ...", Lewy 1967) is selected and no longer RESTRICTED; the 1922 German and Ogden are V3. Record: "Independent propositions ... give to one another the probability 1/2" holds for propositions of prior 1/2, as in W's example; the general clause contradicts 5.15 (P(r v s | p) = 3/4)  ← 5.15, A4
- **5.153** · THM · a proposition in itself is neither probable nor improbable; probability is a relation  ← 5.15
- **5.154** · REM · urn: equal probability means known circumstances favor neither event (empirical frequency vs. logical probability)
- **5.155** · DEF · unit of the probability proposition: unknown circumstances give an event a degree of probability
- **5.156** · THM · probability is a generalization. A proposition can be an incomplete picture of a situation (Sachlage), yet it is always a complete picture (a partial assignment with a determinate sense)  ← 2.201, 3.23
- **5.2** · THM · the structures of propositions stand in internal relations  ← 4.125
- **5.21** · DEF · presenting a proposition as the result of an operation on bases
- **5.22** · DEF · operation := expression of a relation between the structures of result and bases
- **5.23** · DEF · operation := what must be done to one proposition to make another. DEF doubtful under X46 (5.21, 5.22 fix "Operation" first); a retagging candidate; nothing rests on it
- **5.231** · THM · operations depend on formal properties (internal similarity of forms)  ← 5.22
- **5.232** · THM · the internal relation ordering a series = the operation generating it  ← 4.1252, 5.22
- **5.233** · DEF · an operation first occurs where logical construction begins
- **5.234** · DEF · truth-operations := operations with elementary propositions as bases
- **5.2341** · THM · the sense of a truth-function of p is a function of the sense of p; denial reverses the sense  ← 4.4, 4.0641
- **5.24** · THM · R · an operation shows itself in a variable; it expresses the difference between forms. (E11): UNS until now, but it states no limit. RESTRICTED: the parenthesis holds for operations that keep their bases; under variabilization base and result share the base's form  ← 4.126
- **5.241** · THM · an operation characterizes a difference of forms, not a form  ← 5.24
- **5.242** · THM · the same operation iterated is expressible only by variables  ← 4.1273
- **5.25** · THM · an operation asserts nothing; its occurrence does not characterize the sense  ← 4.0621
- **5.251** · THM · V2 · a function cannot be its own argument (3.333), but the result of an operation can become a basis of the same operation ("ihre eigene Basis werden"; iteration) . V2: "ihre eigene Basis" (feminine: the operation's basis) against Ogden's "its own basis" (most naturally the result's); the dropped "werden" is secondary  ← 3.333
- **5.252** · THM · progress through a formal series (and through Russell's type hierarchy) is possible only by operations  ← 5.251
- **5.2521** · DEF · successive application: O'O'O'a. Mixed: s1 DEF ("nenne ich"); the parenthesis an assertion (separates fixed contexts, J-subst); s2 DEF in substance (a way of speaking; no tuple notation)
- **5.2522** · DEF · general term of a formal series: [a, x, O'x], a variable. The third member DEF; X51's kind-first outcome rests on it
- **5.2523** · THM · successive application = "and so on": the ancestral is primitive in the notation  ← 5.2522, 4.1273
- **5.253** · THM · operations can cancel one another  ← 5.2341
- **5.254** · THM · operations can vanish: ~~p = p  ← 4.0621
- **5.3** · THM · every proposition is the result of truth-operations on elementary propositions; truth-operations on truth-functions yield truth-functions  ← 4.4, 5.234
- **5.31** · THM · the 4.31 schemata and the 4.442 sign work with non-elementary arguments  ← 5.3
- **5.32** · THM · every truth-function results from finitely many applications of truth-operations (each possibly over an infinite class, 5.52)  ← 5.3
- **5.4** · THM · there are no logical objects or logical constants  ← 4.441
- **5.41** · THM · results of truth-operations that are the same truth-function are identical  ← 4.465
- **5.42** · THM · v and ⊃ are not relations; crosswise definability shows they are not primitive  ← 4.0312
- **5.43** · THM · infinitely many consequences (~~p, ~~~~p, ...) are one proposition; the propositions of logic all say the same, i.e., nothing  ← 5.41, 4.461
- **5.44** · THM · truth-functions are not material functions; ~~p does not treat of ~  ← 4.0621
- **5.441** · THM · apparent constants vanish: ~(Ex).~fx = (x).fx; (Ex).fx.x = a = fa  ← 5.52, 5.53
- **5.442** · THM · given a proposition, all truth-operations on it are given with it (closure)  ← 5.3
- **5.45** · DEF · if there are logical primitive signs, their mutual position must be made clear
- **5.451** · A8 · primitive ideas independent; introduced uniformly in all contexts (textual source for A8 "uniform")
- **5.452** · REM · a new expedient in logic must be justified everywhere it is used
- **5.453** · THM · R · no numbers in logic; no pre-eminent numbers (= 4.128). RESTRICTED as 4.128 (J6)  ← 4.128
- **5.454** · REM · in logic there is no side by side and no classification
- **5.4541** · REM · simplex sigillum veri
- **5.46** · THM · introducing the logical signs introduces all their combinations; the proper primitive is the general form of combination  ← 5.442
- **5.461** · THM · the need for brackets indicates ("deutet ... hin") that v and ⊃ are not real relations  ← 4.0312
- **5.4611** · THM · logical operation signs are punctuation  ← 4.0312
- **5.47** · THM · R · all logical operations are already in the elementary proposition: fa says the same as (Ex).fx.x = a; the one logical constant is the general form. RESTRICTED: "fa" is schematic, R(a, b) as a function of a (3.318; A14)  ← 5.441, 4.5
- **5.471** · DEF · the general form of proposition is the essence of proposition
- **5.4711** · REM · essence of proposition = essence of description = essence of the world
- **5.472** · DEF · the general propositional form is the one primitive sign of logic
- **5.473** · S3 · logic must take care of itself; "a possible sign must also be able to signify"; what is possible in logic is permitted. "Socrates is identical": no meaning given, not an impermissible symbol. Restricted in (X29, as 4.5(iii)); unrestricted since (X41). Mixed: s1-s3 and the last sentence assertions; the parenthesis has limit form
- **5.4731** · THM · we cannot think illogically  ← 3.03
- **5.4732** · THM · we cannot give a sign the wrong sense: sense is fixed by sign + projection  ← 3.13
- **5.47321** · THM · Occam: unnecessary elements in a symbolism mean nothing (= 3.328). It applies to the units of every sign, terms included (X51): idle binders are transparent (J-vac); hole units (H1); normal-form terms (J-norm)  ← 3.328
- **5.4733** · THM · every possible proposition is legitimately constructed; lack of sense comes only from missing meanings. Holds: every possible sign has a sense under some admissible projection (D10)  ← 5.473, D10
- **5.474** · THM · the number of fundamental operations depends on the notation  ← 3.3441, 5.5
- **5.475** · THM · what matters is a sign system of a definite multiplicity  ← 4.04
- **5.476** · REM · a rule is expressed, not a number of primitive ideas
- **5.5** · THM · every truth-function results from successive application of N to elementary propositions  ← 5.3, 5.502
- **5.501** · DEF · (xi-bar) := the values of a propositional variable, order indifferent. Described by: 1 enumeration; 2 a function fx; 3 a formal law (formal series). DE "Wir koennen drei Arten ... unterscheiden" (Ogden: "We may distinguish 3 kinds"); that these are all of them is a signature commitment (weight 0), not the wording (K3, the one left; X24). The values of fx are the propositions fa that have sense, a not named in the scope. The kind-3 unit (assertion, 3) is written in G\*; a vacuous binder is transparent, not a function fx
- **5.502** · NOT · N(xi-bar) := negation of all values of xi
- **5.503** · THM · construction by N is exactly expressible (a formal grammar)  ← 5.502
- **5.51** · THM · N(p) = ~p; N(p, q) = ~p.~q  ← 5.502
- **5.511** · REM · "connected into an infinitely fine network, to the great mirror"
- **5.512** · THM · what denies in ~p is what all signs denying p have in common (the rule), not "~"  ← 3.344, 4.0621
- **5.513** · THM · p.q is what all symbols asserting p and q share; each proposition has exactly one negative (the complement); q:p v ~p says the same as q  ← 4.0641, 4.465
- **5.514** · DEF · in a fixed notation, rules for constructing all propositions that assert p, deny p, etc., are equivalent to the symbols and mirror their sense
- **5.515** · THM · what v and . connect must be propositions; the arguments of truth-operations need a sense. DE: this must show itself ("zeigen") in our symbols. Mixed: the "zeigen" sentence is an assertion; the closing argument ("kann es allein nicht Sinn haben") is a limit  ← 3.142
- **5.5151** · THM · a negative fact can serve as a sign of a negative proposition (a medium with pi(d) = 0, as DEF 2.1 allows); positive and negative presuppose each other  ← 2.1, 4.0641
- **5.52** · THM · N over all values of fx is ~(Ex).fx: generality without a truth-function of its own  ← 5.501, 5.502
- **5.521** · DEF · the concept "all" is separated from the truth-function (DONE: Rogers & Wehmeier)
- **5.522** · DEF · the generality symbol refers to a logical prototype and makes constants prominent (= 3.315)
- **5.523** · THM · the generality symbol occurs as an argument  ← 5.52
- **5.524** · THM · given the objects, all objects are given; given the elementary propositions, all are given: the totality fact of 4.52  ← S1, 4.52
- **5.525** · UNS · certainty, possibility, impossibility are not said but shown: tautology, contingent, contradiction  ← 4.464
- **5.526** · A16 · the world can be completely described by completely general propositions, names attached afterwards ("the world": the actual world, as worded). The first sentence is D12, derived from A17 (5.5262, sentence 2); the kind stays an assertion. Second sentence: A16, plain (X22): every object is singled out by a completely general description, so |O| <= ℵ0. "Singled out" read as both: the description is true of that object only, and "es gibt ein und nur ein x, welches ..." (5.5321) has sense (X42)
- **5.5261** · THM · a completely general proposition is composite; phi and x signify separately. Restricted in (X29, M+: its binary instance (E phi)(Ex, y) phi xy had no sense). Unrestricted since S has sense  ← 3.142
- **5.5262** · A18 · mixed: first sentence A18 (minimal alterations, X26); second sentence A17 (X25); parenthesis REM (the ceteris-paribus illustration, X25). Not restricted
- **5.53** · DEF · R · identity of object by identity of sign; difference by difference of signs (exclusive quantifiers; DONE: Rogers & Wehmeier). RESTRICTED: weak exclusion; strong exclusion would break 5.54 and A11 (Lemma U)  ← 4.0311
- **5.5301** · THM · identity is not a relation between objects  ← 5.53
- **5.5302** · A19 · Russell's "=" fails: two objects may share all properties, which is significant even if never true (indiscernibles, 2.0233). Read plainly, a frame condition, A19; never true at χ\* (A16). Model: Φ.
- **5.5303** · THM · saying two things are identical is nonsense; saying one is identical with itself says nothing  ← 5.53
- **5.531** · NOT · f(a, a), not f(a, b).a = b; f(a, b), not f(a, b).~a = b (f need not be elementary; under A14 no state of affairs has a single object, and for an elementary f, f(a, a) is no proposition
- **5.532** · NOT · (Ex).f(x, x), not (Ex, y).f(x, y).x = y; (Ex, y).f(x, y) for distinct x, y
- **5.5321** · NOT · R · instead of "(x): fx ⊃ x = a" (only a satisfies f, 5.5301): (Ex).fx.⊃.fa : ~(Ex, y).fx.fy; "only one x satisfies f( )": (Ex).fx : ~(Ex, y).fx.fy. RESTRICTED: it says "only one" where the doubled instances have sense; under X31's token rule it is vacuous for f = Cyc in Φ. Both formulas; the first has no sense for a and h in Φ. Mixed: "schreiben wir" is notation; that the formulas say what the words say is an assertion; the mark is (assertion, 4)
- **5.533** · THM · the identity sign is not essential to logical notation (DONE: Rogers & Wehmeier)  ← 5.53
- **5.534** · THM · a = a, a = b.b = c.⊃ a = c, (x).x = x, (Ex).x = a cannot be written in a correct notation  ← 5.53
- **5.535** · UNS · the axiom of infinity would show in infinitely many names with different meanings (it concerns |O|; D21 concerns |𝔸|)  ← D9, 4.0311
- **5.5351** · UNS · R · V2 · "p is a proposition" is nonsense (Unsinn). Russell's attached hypothesis p ⊃ p is without sense (sinnlos; RESTRICTED as 4.461), and it becomes nonsensical (unsinnig) for non-propositional arguments. V2: both "unsinnig" become "meaningless" and "senseless", and "sinnlose" also "senseless"; Ogden's "to show that" for "damit ... koennten"  ← 4.126
- **5.5352** · REM · "there are no things" as ~(Ex).x = x fails
- **5.54** · THM · in the general form, propositions occur in propositions only as bases of truth-operations (extensionality)  ← 5.3
- **5.541** · REM · apparent exceptions: "A glaubt, dass p der Fall ist" (A believes that p is the case; Ogden: "thinks", V1), "A thinks p"
- **5.542** · UNS · "A believes that p" has the form "'p' says p": a co-ordination of facts by co-ordinating their objects. That is the projection, not a configuration, so not a truth-function of elementary propositions; 5.54 survives  ← 2.1513, 5.54
- **5.5421** · REM · no soul or subject as conceived in superficial psychology; a composite soul would not be a soul
- **5.5422** · THM · judging nonsense is impossible: what is judged is a sense, and nonsense has none  ← 5.542, 5.4733
- **5.5423** · REM · Necker cube: one medium under two projections gives two senses ("two different facts")
- **5.55** · THM · forms of elementary propositions cannot be given a priori: the axioms fix no form and no number of names (models with |O| = 2 and with infinite O; A13 gives |O| >= 2). Route 2 adds only that each occurring form has infinitely many instances  ← 4.128
- **5.551** · A11 · every question which can be decided at all by logic can be decided without further trouble (1933 English: "off-hand", Lewy; R3). Forces THEOREM 3, a condition on frames: no form full on two infinite filler sets; with 5.5261, 1-place forms do not encode every finite graph; kind 3 restricts further. (The necessary conditions are (a_k\*), (b_k), (d); X27.) For full frames: O finite, or finitely many forms, all 1-place; with A13, O finite
- **5.552** · THM · logic presupposes that something is (D1), not how things are (independent of χ\*)  ← D1, S1
- **5.5521** · REM · logic and the world
- **5.553** · THM · no pre-eminent number of relata (= 4.128)  ← 5.55
- **5.554** · THM · specifying ("Angabe") any special form a priori would be arbitrary  ← 5.55
- **5.5541** · REM · 5.55's demand for a case: "Es soll sich a priori angeben lassen" (it is supposed to be possible to specify a priori; Ogden: "decide", V1) whether a 27-termed relation sign is needed. 5.5542 asks whether the question can be put; 5.557 answers it (application decides).
- **5.5542** · THM · a sign form with nothing that could correspond to it: under A6a the sign is itself a state of that form, so the form is instantiated  ← A6a
- **5.555** · REM · the concept of elementary proposition apart from its special forms; the system of construction matters
- **5.556** · THM · no hierarchy of forms of elementary propositions; we foresee only what we construct  ← 5.55
- **5.5561** · THM · empirical reality is limited by the totality of objects; the limit shows itself ("zeigt sich") again in the totality of elementary propositions; hierarchies are independent of reality. Not mixed: the "zeigt sich" sentence states no limit  ← S1
- **5.5562** · THM · if logic says there must be elementary propositions, everyone who understands unanalysed propositions knows it  ← 4.221
- **5.5563** · REM · propositions of colloquial language are logically in order as they are
- **5.557** · THM · the application of logic decides which elementary propositions there are ("welche"; Ogden: "what", V1); logic cannot anticipate it. Plain reading; the RESTRICTION is withdrawn. Route 2 anticipates only that each occurring form has infinitely many instances; A11 that the objects and forms are countable  ← 5.55
- **5.5571** · THM · trying to give elementary propositions a priori yields nonsense  ← 5.557
- **5.6** · THM · the limits of my language mean the limits of my world: every situation is expressible and every sense lies in Λ  ← A7, 4.1
- **5.61** · THM · logic fills the world. "This and this there is in the world, that there is not" cannot be said: O is constant across Λ (S1), so no sense excludes an object. We cannot say what we cannot think  ← S1, 4.1272, 3.001
- **5.62** · UNS · what solipsism means is correct but shows itself: the limits of the language (the projection is mine) mean the limits of my world  ← 2.1513, 5.6
- **5.621** · REM · the world and life are one
- **5.63** · REM · I am my world (the microcosm)
- **5.631** · UNS · there is no thinking, presenting subject: in "The world as I found it" the body could be reported, the subject not. The projection is not a configuration  ← 2.1513
- **5.632** · UNS · the subject does not belong to the world; it is a limit of the world  ← 2.1513, A6a
- **5.633** · UNS · nothing in the visual field permits the inference that it is seen from an eye: no sense records the projection  ← 2.1513
- **5.6331** · REM · the figure: the visual field does not contain the eye (cf. 2.173)
- **5.634** · THM · no part of experience is a priori: whatever we see or describe could be otherwise; no a priori order of things  ← 3.03, A4
- **5.64** · THM · solipsism strictly carried out coincides with pure realism: the I shrinks to an extensionless point (the projection adds no state of affairs); reality remains  ← 2.1513, A6a
- **5.641** · UNS · the philosophical I: the metaphysical subject, the limit, not a part of the world  ← 5.632
- **6** · DEF · general form of truth-function [p-bar, xi-bar, N(xi-bar)]: Prop is the least class containing the elementary propositions and closed under N over any selection described by 5.501's kinds. This is the general form of proposition (= 4.5)
- **6.001** · THM · every proposition results from successive applications of N to elementary propositions  ← 6, 5.5
- **6.002** · THM · the general form of construction gives the general form of operation  ← 6
- **6.01** · DEF · general form of operation: Omega'(eta-bar) = [xi-bar, N(xi-bar)]'(eta-bar) = [eta-bar, xi-bar, N(xi-bar)]
- **6.02** · DEF · numbers: x = Omega^0'x Def.; Omega'Omega^nu'x = Omega^(nu+1)'x Def.; 0 + 1 = 1 Def., etc.
- **6.021** · DEF · a number is the exponent of an operation
- **6.022** · UNS · the concept number is the variable number (formal concept, 4.1272); equality of numbers is the general form of special equalities  ← 4.126
- **6.03** · DEF · V2 · general form of (natural) number: [0, xi, xi + 1] (a formal-series variable, 5.2522). Ogden's "cardinal" selected over DE "ganze Zahl" (V2)
- **6.031** · THM · class theory is superfluous in mathematics: the needed generality is not accidental (numbers via operations, not classes)  ← 6.021, 6.1231
- **6.1** · THM · the propositions of logic are tautologies  ← 4.46, 6
- **6.11** · THM · so they say nothing (analytic)  ← 6.1, 4.461
- **6.111** · THM · theories that make logic substantial are false: "true"/"false" are not properties among others  ← 4.431, 6.11
- **6.112** · REM · the explanation of logical propositions must give them a peculiar position
- **6.113** · THM · logical propositions show their truth "in the symbol alone": [[phi]] = Λ is computed from sign + ρ. Second sentence: non-logical propositions' truth cannot be recognized from them alone. (X41, J-tok): "am Satz allein" read as a type, after "am Symbol allein" (co-plain; LI selects it): the sense alone does not fix the truth value. D6b for compounds  ← 4.466
- **6.12** · UNS · that propositions combined in a certain way give a tautology shows their formal properties  ← 4.122, 6.1
- **6.1201** · THM · examples: ~(p.~p) shows p and ~p contradict; (p ⊃ q).(p) :⊃: (q) shows q follows; (x).fx :⊃: fa shows fa follows from (x).fx  ← 6.12, 5.12
- **6.1202** · THM · contradictions would serve as well  ← 6.12
- **6.1203** · NOT · intuitive T-F bracket method, for tautologies without generality signs
- **6.121** · THM · zero-method: logical propositions bring propositions into equilibrium, which shows their logical construction  ← 6.12
- **6.122** · THM · we can do without logical propositions: an adequate notation shows formal properties on inspection. A ground of J-N  ← 6.121, 4.1211
- **6.1221** · THM · q follows from p ⊃ q.p: seen from the propositions, or shown by the tautology p ⊃ q.p :⊃: q  ← 6.1201
- **6.1222** · THM · logical propositions can be neither confirmed nor refuted by experience: [[phi]] = Λ is independent of χ\*  ← 6.1
- **6.1223** · THM · logical truths are "postulated" only as far as we postulate an adequate notation. A ground of J-N  ← 6.122
- **6.1224** · REM · logic as the theory of forms and of inference
- **6.123** · THM · laws of logic obey no further laws; one law of contradiction suffices (not one per type): all senses lie in one algebra P(Λ)  ← 4.4, 3.42
- **6.1231** · THM · general validity is not the mark of logic: being true of all objects in χ\* is accidental; tautology is [[phi]] = Λ  ← 4.46
- **6.1232** · THM · essential vs. accidental general validity; the axiom of reducibility, if true, is true by happy chance  ← 6.1231
- **6.1233** · THM · a world violating the axiom of reducibility is thinkable ("denken"), so it is not logical  ← 6.1232, 3.03
- **6.124** · UNS · logical propositions present the scaffolding of the world; they presuppose that names have meaning and elementary propositions have sense. Which signs are tautologies depends on the form (e.g., exclusive-quantifier counts show |O|) and so shows it  ← S1, 4.1272
- **6.125** · THM · all logical propositions can be described at the outset. Holds by A11 in both branches of THEOREM 3, for all kinds of generality  ← 6.1, A11
- **6.1251** · THM · no surprises in logic  ← 6.125
- **6.126** · A11 · V2 · whether a proposition belongs to logic "kann man berechnen" (can be calculated) by calculating the logical properties of the symbol (A11). Ogden: "determined by determining", V2. Proof is sign manipulation by mere sign-rules ("Zeichenregeln") without regard to sense
- **6.1261** · THM · in logic process and result are equivalent  ← 6.126
- **6.1262** · THM · proof in logic is only a mechanical expedient to recognize complicated tautologies. Presupposes decidability  ← A11
- **6.1263** · THM · logical proof of a significant proposition and proof in logic are quite different  ← 6.1, 5.12
- **6.1264** · THM · a significant proposition's proof shows that it is so; every logical proposition is the form of a proof (a modus ponens in signs; modus ponens is not a proposition). Mixed: the parenthesis ("kann man nicht durch einen Satz ausdruecken") is a limit  ← 6.1201
- **6.1265** · THM · logic can be conceived so that every proposition is its own proof  ← 6.127
- **6.127** · A11 · all logical propositions are of equal rank; every tautology shows itself to be one (A11, positive half only; the two-sided "whether" comes from 5.551 and 6.126). Not mixed: both sentences are assertions
- **6.1271** · THM · the number of primitive propositions is arbitrary (one conjunction suffices); self-evidence is no criterion  ← 6.127
- **6.13** · UNS · logic is not a theory but a reflexion of the world; logic is transcendental  ← 6.124
- **6.2** · THM · mathematics is a logical method; its propositions are equations, hence pseudo-propositions  ← 4.241, 6.021
- **6.21** · THM · mathematical propositions express no thoughts  ← 6.2
- **6.211** · REM · mathematics is used to infer between non-mathematical propositions
- **6.22** · UNS · the logic of the world shows in tautologies (logic) and in equations (mathematics)  ← 6.12, 6.2
- **6.23** · THM · = between expressions means substitutability, which must show itself in the expressions  ← 4.241
- **6.231** · THM · affirmation as double denial; 1+1+1+1 as (1+1)+(1+1): properties of form  ← 4.0621, 6.02
- **6.232** · THM · against Frege's same meaning, different senses: identity of meaning is perceived from the expressions  ← 4.243
- **6.2321** · THM · provability of mathematical propositions = correctness seen without comparison with facts  ← 6.2
- **6.2322** · THM · identity of meaning cannot be asserted: knowing the meanings, I know whether they coincide  ← 4.243
- **6.2323** · THM · an equation marks only the standpoint of equality of meaning  ← 6.2322
- **6.233** · REM · language supplies the intuition needed in mathematics
- **6.2331** · THM · calculation is not an experiment  ← 6.2321
- **6.234** · THM · mathematics is a method of logic  ← 6.2
- **6.2341** · THM · working with equations: every mathematical proposition is self-intelligible  ← 6.234
- **6.24** · THM · mathematics proceeds by substitution according to equations  ← 6.23
- **6.241** · THM · proof of 2 x 2 = 4 by substituting operation exponents  ← 6.02, 6.24
- **6.3** · THM · logical research is the investigation of all regularity; outside logic all is accident (C empty)  ← A4
- **6.31** · THM · induction is not a logical law: it is a significant proposition, hence not a priori  ← 3.03, 6.3
- **6.32** · DEF · the law of causality is the form of a law, not a law
- **6.321** · REM · "law of causality" as a class name; least-action laws
- **6.3211** · REM · the a priori certain proves purely logical
- **6.33** · THM · we know a priori not a conservation law but the possibility of a logical form  ← 6.3
- **6.34** · DEF · the principle of sufficient reason ("Satz vom Grunde"; Ogden: "law of causation"), continuity and least expenditure are a priori insights ("Einsichten") into the possible form-giving of scientific propositions
- **6.341** · THM · mechanics as a network: the form of description is arbitrary (square, triangular, hexagonal mesh). Formally, alternative generating sets of the sense algebra (3.25)  ← 3.25
- **6.342** · THM · that the world can be described by a given net asserts nothing; that it can be described more simply by one system says something about the world  ← 6.341
- **6.343** · DEF · mechanics: constructing all true propositions needed for describing the world according to a single plan
- **6.3431** · REM · through logic, physical laws still speak of the objects of the world
- **6.3432** · THM · mechanical description is always general (some points, never particular ones)  ← 6.343
- **6.35** · THM · the network is purely geometrical and a priori; laws treat of the network, not of what it describes (= 3.0321: index structure vs. constraints)  ← 6.341
- **6.36** · UNS · "there are natural laws" cannot be said; it shows itself  ← 6.35
- **6.361** · REM · Hertz: only uniform connections are thinkable
- **6.3611** · THM · no "passage of time": only comparisons of processes. Describing one of two mutually exclusive events needs an asymmetry (cf. 2.02331)  ← 2.02331
- **6.36111** · REM · incongruent counterparts: congruent figures in a space need a higher dimension to coincide
- **6.362** · THM · what can be described can happen; what the law of causality is supposed ("soll") to exclude cannot be described  ← 3.02, 6.35
- **6.363** · THM · induction assumes the simplest law compatible with experience  ← 6.31
- **6.3631** · THM · this has no logical foundation, only a psychological one  ← 6.31, A4
- **6.36311** · THM · that the sun will rise tomorrow is a hypothesis  ← 6.3631
- **6.37** · A4 · no necessity for one thing to happen because another has: only logical necessity (C empty; textual source for A4)
- **6.371** · REM · the illusion that natural laws explain natural phenomena
- **6.372** · REM · people stop at natural laws as the ancients stopped at God and Fate
- **6.373** · THM · the world is independent of my will  ← A4
- **6.374** · THM · no logical connexion between will and world  ← A4, 6.373
- **6.375** · A4 · only logical impossibility (textual source for A4)
- **6.3751** · THM · two colors at one place at the same time ("zugleich") is a logical impossibility; the logical product of two elementary propositions is neither tautology nor contradiction. So color ascriptions are not elementary, and must be analysed. 3.25 (K_k prime): no binary analysis respects one-change-apart values. 1929 breaks here  ← 4.211, A4, 3.25
- **6.4** · THM · all propositions are of equal value  ← 6.41
- **6.41** · UNS · the sense of the world lies outside the world. Every sense is contingent (accidental) or degenerate, so a non-accidental value has no sense in Prop. C1: value as an objective (an ordering of Λ), not a constraint (a subset)  ← 3.03, 4.461
- **6.42** · UNS · no ethical propositions; propositions cannot express anything higher  ← 6.41
- **6.421** · UNS · ethics cannot be expressed; ethics is transcendental; ethics and aesthetics are one  ← 6.42
- **6.422** · REM · ethical reward and punishment lie in the action itself
- **6.423** · UNS · of the will as the bearer of the ethical we cannot speak  ← 6.42, 5.632
- **6.43** · THM · good or bad willing changes only the limits of the world, not the facts: it does not select χ\*. The world waxes or wanes as a whole  ← 6.373
- **6.431** · REM · in death the world does not change but ceases
- **6.4311** · REM · death is not an event of life; eternity as timelessness
- **6.4312** · REM · temporal immortality solves no riddle
- **6.432** · UNS · how the world is, is indifferent for what is higher; God does not reveal himself in the world  ← 6.41
- **6.4321** · REM · the facts belong only to the task, not to the solution ("Loesung")
- **6.44** · UNS · not how the world is (χ\*) is the mystical, but that it is (D1, A5)  ← D1, A5, 5.552
- **6.45** · REM · the world sub specie aeterni: a limited whole; the mystical feeling
- **6.5** · THM · if a question can be put, it can be answered: a question has a sense, and by bivalence χ\* settles it  ← 2.21, 4.1
- **6.51** · THM · scepticism is nonsense (unsinnig) where no question can be asked  ← 6.5
- **6.52** · REM · when all scientific questions are answered, the problems of life are untouched
- **6.521** · REM · the solution of the problem of life is its vanishing
- **6.522** · UNS · there is the inexpressible; it shows itself: the mystical  ← 4.1212
- **6.53** · DEF · the right method: say only propositions of natural science (4.11); show the metaphysician that some signs have no meaning (5.4733)
- **6.54** · THM · "my propositions are elucidatory ... senseless" (DE "unsinnig": nonsense; Ogden's word also renders "sinnlos"): the Tractatus's propositions concern forms and invariants (4.1212, 4.122), so they are not in Prop. C7: holds by typing. The ledger's tags are themselves of this kind  ← 4.1212, 4.122
- **7** · UNS · whereof one cannot speak, thereof one must be silent  ← 4.1212

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
