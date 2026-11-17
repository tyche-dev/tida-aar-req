
.. _chapter-relation:

Relation to other work
======================

* **WG2, Identity, Behaviour and Enforcement for AI Agents (IBEA).** The WG2 charter places "the record that carries a
  decision, and the properties any carried claim needs" under FG-TIDA/themes#1 (Out of Scope). For the texts that
  describe this boundary, @OlehVasylenko2000 proposed one line (PR #46, 12 November 2026), which this work item takes:
  "WG2 specifies what a decision is and what its outcome means, including what the decision record states; #1
  specifies the record-side requirements that record must meet and the properties of the claims it carries (R1–R8)."
* **WG1, Continuous and Dynamic Remote Attestation for Agentic AI (CDRA).** WG2 examines with WG1 whether a third party
  can later check an enforcement decision. That check also rests on R7.3: tamper-evidence that a party with no
  relationship to the producer can check.
* **FG-TIDA/themes#5, Provenance of Authority: mutual, not sequential.** Provenance determines what a record can
  truthfully say about authority; the properties of the record determine whether it survives a party who was not
  there.
* **FG-TIDA/themes#6, task 3.** What a conformance verdict asserts and how a verifier checks it. Task 3 takes its tier 1
  and tier 2 rejection classes from R3 and R4 unchanged, and #6 "will reference" R7 rather than restate it (@cgorlla,
  14 October 2026).
* **FG-TIDA/themes#27 and PR #28 (verifier-side requirements in regulated workflows).** Of the change-event record it
  proposes, its drafter wrote that the record-side requirements in themes#1 "define where this record belongs; this
  item specifies what the verifier must be able to read from it" (@zhaoxinghua09-cell, PR #28, 15 October 2026).
* **Verifier-side interface to the record requirements (linked contribution record).** Four clauses, VR1 to VR4, on
  the report a verifier makes: each check as a pair of who performed it and against what; the moment evaluated against;
  what a pass claims and within what boundary; and the report as a claim the next party assesses. The record "adds
  nothing to R1–R8 and alters nothing in them", and it stands beside this document, under its author's name
  (@zhaoxinghua09-cell, PR #46, 16 November 2026):
  https://github.com/LGD-Eval/evaluation-protocol/blob/f66c4658fd1c99b1e6fef99b99eed3865dc8e45f/FG-TIDA-AAR-VERIFIER-SIDE-INTERFACE.md.
  Whether the four clauses move into this work item is for the group to decide.
* **WG0, Use Cases and Terminology.** Use cases #7 (@syedofc) and #12 (@danyka-icam) supply the cases for D2.
* **Format work.** Encodings and profiles for carried claims belong to the bodies that specify formats. The thread
  named the Internet Engineering Task Force (IETF) Remote Attestation Procedures (RATS) architecture and the Entity
  Attestation Token (EAT) as relevant adjacent work; this assigns no standards body exclusive responsibility for future
  formats (@OlehVasylenko2000, PR #46, 26 October 2026).
* **ITU-T Study Group 17 (SG17).** "Work under this theme complements ongoing SG17 work without duplicating it.
  Questions of possible overlap are resolved by the FG Chair and the SG17 Chair on a case-by-case basis, in accordance
  with clause 2 of the Terms of Reference." (wording by @OlehVasylenko2000, 16 September 2026)
