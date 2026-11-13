
.. _chapter-requirements:

Requirements
============

The clause text stands in 2 comments posted on FG-TIDA/themes#1: R1–R6 of 24 August 2026, and R4.4, R7 and R8 of
12 October 2026 (see :ref:`chapter-annexes`). This table summarises them; where it differs, the posted comments govern.
Each row names who proposed the clause and, in brackets, who refined it.

.. list-table:: Record-side requirements and their authors
    :header-rows: 1
    :widths: 18 56 26
    :class: longtable

    * - Clause
      - Requirement, in one line
      - Proposed (refined) by
    * - R1 Separability
      - A relying party that rejects reports the class of the rejection; a bare accept or reject is not enough.
      - @tyche-dev; asked for as a requirement by @OlehVasylenko2000
    * - R2 The reported reason must be true
      - A correct rejection with a misattributed cause does not conform.
      - @tyche-dev
    * - R3 Tier 1 classes
      - Replayed, expired, malformed, out of mandate: each decidable from the record and the relying party's own state,
        and distinguishable from the others.
      - @tyche-dev (@AntoBud, @OlehVasylenko2000)
    * - R4 Tier 2: standing withdrawn
      - Every tier 1 check passes, but the grantor would not confer the mandate at the moment of the act. The record
        declares whether the grantor's continued standing is checkable (R4.1); a relying party records which moment it
        used (R4.2); neither moment is mandated, and the choice is visible (R4.3).
      - the class @AntoBud; the 2 tiers @tyche-dev
    * - R4.4
      - A carried standing answer is a claim, and it carries what R7 requires.
      - @AntoBud
    * - R5
      - Negative and null assertions are claims, subject to R1–R4 as a positive claim is.
      - @cgorlla; the null case @OlehVasylenko2000 (@zhaoxinghua09-cell)
    * - R6
      - Freshness is a relation, not a property: the record carries the moment its assertion was true and the means, if
        any, of rechecking it.
      - @AntoBud
    * - R7
      - Any carried claim needs attribution (R7.1), a stated moment (R7.2) and tamper-evidence that a party with no
        relationship to the producer can check (R7.3). R7 does not make a claim true.
      - the recursion @OlehVasylenko2000; the names follow @OlehVasylenko2000 and @danyka-icam
    * - Absence and silence
      - The record keeps 3 states apart: a reference was established; a bounded search, with its scope and author,
        returned nothing; nothing was recorded.
      - @pdixon-wpf and @OlehVasylenko2000, on FG-TIDA/themes#9
    * - LR1–LR5 Lineage
      - Descent, transformed descent, independent reconstruction, examined-but-unresolved and record silence stay
        distinguishable; similarity and conformance never stand in for lineage, and missing evidence never yields NO.
      - @danyka-icam (@OlehVasylenko2000)
    * - R8
      - A later relying party can establish the act, the execution that performed it, that execution's supported
        relation to a logical agent where one exists, and the effective state that governed the act at that time, not a
        later state (R8.1–R8.5).
      - @syedofc; R8.3 @OlehVasylenko2000; R8.5 @pdixon-wpf
    * - 3 relations
      - The execution, its supported relation to a logical agent, and the principal or harness context that
        instantiated it stay distinguishable; instantiation alone establishes no authorization.
      - @syedofc; supported by @OlehVasylenko2000

Questions carried open
----------------------

The work item carries the open questions of the theme 1 charter (PR #46, version 0.5), with the positions recorded
under them: the evidence basis of a carried claim (1); whether the record states which checks were in the path (2);
what attribution binds to (3); "and if so where" in R4.1 (5); a third UNCLEAR lineage state (6); multi-step
delegation, the boundary with law and policy, and record-keeping obligations (7); inputs from FG-TIDA/themes#5, #36 and
PR #28 (9); reconstructable or re-computable (10); whether a deployment can meet R8 (11); and an asserted or witnessed
moment (12). On the last: R7.3 lets a party check that a record is unaltered, but not when it was written
(@Abracadabrastartup, 10 November 2026). @OlehVasylenko2000 suggested that D1 first keep 3 moments apart: the moment of
the act; the moment a producer states for a claim; and an independently bounded moment, which shows only that a record
existed no later than a given time and is not the freshness relation of R6 (12 November 2026). If the proposed R7.2a
becomes text, it is a sub-clause of R7.2, and R7 keeps 3 properties.
