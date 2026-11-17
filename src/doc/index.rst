
.. raw:: latex

    \pagestyle{plain}
    \thispagestyle{plain}
    %% Suppress all TOC entries for the overview chapter (sections, subsections,
    %% Copyright addcontentsline) — restored just before \sphinxtableofcontents
    %% so chapters from Introduction onward appear in the TOC normally.
    \let\osiaorigaddcontentsline\addcontentsline
    \renewcommand{\addcontentsline}[3]{}

.. _chapter-overview:

Accountability and Attribution After an Agent Has Acted
=======================================================

.. only:: html

    **Record-side requirements (AAR-REQ). Proposal for a new work item**

.. raw:: latex

    \begin{center}\textbf{Record-side requirements (AAR-REQ). Proposal for a new work item}\end{center}

Abstract
--------

When an act by an agent is questioned later, the party asking was usually not present, and establishing what happened
can require "an investigation rather than a lookup" (FG-TIDA/themes#1). This contribution proposes a work item that
states what an action-time record must be able to carry, and what properties every claim it carries needs, so that
such a party can establish the execution that performed the act and, where one exists, its supported relation to a
logical agent; under whose delegated authority; within what declared scope; and that the record is unaltered. It
consolidates requirements R1–R8, the lineage requirements and the absence states developed in the open thread on
themes#1 since August 2026, each clause under its author's name, and maps them to cases. It states requirements only and
prescribes no encodings, schemas, protocols or identifiers.

History
-------

.. list-table::
    :header-rows: 1
    :widths: 10 26 18 14 32

    * - Version
      - Document
      - Approval
      - Focus Group
      - Working Group
    * - 0.1
      - AAR-REQ: proposal for a new work item
      - —
      - TIDA
      - Incubation (proposed)
    * - 0.2
      - Co-author added; status and copyright wording corrected
      - —
      - TIDA
      - Incubation (proposed)
    * - 0.3
      - Two co-authors and a contributor added; a linked contribution record listed
      - —
      - TIDA
      - Incubation (proposed)

To access this Document as a PDF, open the published documentation site in your web
browser and click the PDF download link, or navigate directly to
https://tyche-dev.github.io/tida-aar-req/specification.pdf.

Authors
-------

.. list-table::
    :header-rows: 1
    :widths: 30 40 30

    * - Name
      - Affiliation
      - Contact
    * - Anton Sokolov (editor)
      - Tyche Institute MTÜ, Estonia
      - anton.sokolov@tyche.institute; GitHub @tyche-dev
    * - Syed Amir Hamza
      - Forkit AI
      - GitHub @syedofc
    * - Nika Novak
      - ICAM Research Programme
      - GitHub @danyka-icam
    * - Xinghua Zhao
      - Independent expert
      - GitHub @zhaoxinghua09-cell

Contributors. The requirements come from the open thread on FG-TIDA/themes#1. Its originating proposer is Oleh
Vasylenko (@OlehVasylenko2000), Management Company Elixir LLC (Ukraine), who takes part as proposer and reviewer.
Co-author Nika Novak (@danyka-icam) co-drafted the lineage requirements and cases and contributed use case #12.
Co-author Syed Amir Hamza (@syedofc) co-drafted the identity and state continuity requirements (R8) and contributed use
case #7. Co-author Xinghua Zhao (@zhaoxinghua09-cell) is named for the null-case refinement on R5 and for the linked
contribution record on the verifier side (:ref:`chapter-relation`). @Abracadabrastartup (DEUSPROOF) raised the point
recorded under open question 12, an asserted or witnessed moment (a possible R7.2a). Every clause in
:ref:`chapter-requirements` names its author.

Keywords
--------

Agentic AI; accountability; attribution; action-time record; carried claim; rejection class; delegated authority;
lineage; tamper-evidence.

.. raw:: latex

    \newpage
    \osiacenternextsection

Foreword
--------

Agentic AI systems now act as autonomous entities capable of reasoning, planning, and
executing tasks across services, infrastructures, and organizational boundaries. This
fundamentally changes the nature of identity in digital systems: identity is no longer
limited to human users and static machine instances but must also encompass autonomous,
dynamic, and goal-oriented agents. And identity alone is insufficient — the core question
extends beyond "what an entity is" to "whether, and under what conditions, that entity
should be trusted to act".

The Focus Group on Trust and Identity for humans and agentic AI (FG-TIDA) addresses trust
management and interoperable digital identity infrastructure for humans and for agentic AI,
supporting the development of secure, trustworthy digital ecosystems in which humans and
agentic AI can safely interact and collaborate.

FG-TIDA was established under Recommendation ITU-T A.7 (Focus groups: Establishment and
working procedures), with ITU-T Study Group 17 as its parent group. Further details are
available in the group's terms of reference.

For more news and updates about the TIDA Community, including its supporter organizations,
please refer to the community's published resources.

.. raw:: latex

    \osiacenternextsection

Note
----

This document is a proposal for a new work item, to be submitted to FG-TIDA Incubation by 22 November 2026 as an
input to the first FG-TIDA meeting (Paris, 30 November – 1 December 2026). It is not yet registered, and it is not
adopted Focus Group text. The requirement text it summarises
stands in the posted comments listed in :ref:`chapter-annexes`.

.. Intellectual Property Rights — section commented out. To restore it, remove the
   leading ".." and the indentation below, and re-add a ".. raw:: latex" block with
   "\osiacenternextsection" before the heading (to centre it on the PDF).

   Intellectual Property Rights
   ----------------------------

   ITU draws attention to the possibility that the practice or implementation of this
   Recommendation may involve the use of a claimed Intellectual Property Right. ITU takes no
   position concerning the evidence, validity or applicability of claimed Intellectual Property
   Rights, whether asserted by ITU members or others outside of the Recommendation development
   process.

   As of the date of approval of this Recommendation, ITU had not received notice of intellectual
   property, protected by patents/software copyrights, which may be required to implement this
   Recommendation. However, implementers are cautioned that this may not represent the latest
   information and are therefore strongly urged to consult the appropriate ITU-T databases
   available via the ITU-T website at http://www.itu.int/ITU-T/ipr/.
   Implementers should also be aware that the organization that originated the technically
   equivalent document listed in the Bibliography may have received notices of intellectual
   property required for the implementation of this Recommendation.

.. raw:: latex

    %% Copyright notice commented out. To restore, uncomment the lines below.
    %% \vspace{4em}
    %% \begin{center}\textcopyright{} ITU 2024\end{center}
    %%
    %% \medskip
    %% All rights reserved. No part of this publication may be reproduced, by any means whatsoever, without the
    %% prior written permission of ITU.

    %% Restore \addcontentsline so the TOC below (and Chapter 1 onward) populate.
    \let\addcontentsline\osiaorigaddcontentsline
    \sphinxtableofcontents
    \osiamainmatter

.. toctree::
    :maxdepth: 3
    :numbered:
    :hidden:

    chapters/01_scope
    chapters/02_requirements
    chapters/03_relation_to_other_work
    chapters/04_programme_of_work
    chapters/05_annex/index
    chapters/07_references
