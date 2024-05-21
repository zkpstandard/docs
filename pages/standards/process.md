---
layout: default
title: Standardization Process
parent: ZKProof Standards
nav_order: 1
permalink: /standards/process
---
# ZKProof Processes for Working Groups and Specifications
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## <a id="process-intro"></a>Introduction

The ZKProof effort (initiated in 2018) aims to develop reference material, specifications and standards that will support adoption of advanced cryptographic schemes, with deployment of secure and interoperable zero-knowledge proof systems.

The [ZKProof Standards Committee](https://docs.zkproof.org/standards) was [formed in 2023](https://docs.zkproof.org/about) to develop a process for community promotion of specifications and standards, and oversee the creation of corresponding [working groups (WG)](https://docs.zkproof.org/standards/wg). Information of proposals submitted to workshops prior to 2022 can be found in the [standards>proposals webpage](https://docs.zkproof.org/standards/proposals). The text below describes two envisioned processes:
1. [Creating a ZKProof Working Group (WG)](#process-WG)
2. [Developing a ZKProof Specification (ZSpec)](#process-ZSpec)

These processes are in an early stage of implementation. Based on ZKProof discussions, the processes will be adaptable to integrate learnings obtained throughout their instantiations. Correspondingly, this webpage will be progessively adapted.

## <a id="process-WG"></a>Process for creating a ZKProof Working Group (WG)

1. **Abstract submission:** Each new working group (for developing a specification) should be formally proposed to the ZKProof Standards Committee, by means of an abstract that identifies various key elements (see below). At a minimum, the proposal of a working group for a specification must include:
    1. **WG Title:** Title of the working group (WG).
    2. **WG Team:** Initial team composition (names, affiliations, contact email-addresses).
    3. **WG public contact:** A contact email-address to be publicly-displayed. This should be a mailing list that automatically forwards to every member of the team.
    4. **WG Liaison:** Contact email-address of the WG member responsible for keeping the Standards Committee aware of relevant WG updates.
    5. **Abstract:** An abstract (<=350 words) explaining the WG goal and motivation.
    6. **Structure:** A section that includes:
        - The expected structure of the future initial draft specification.
        - The planned time-frame for its accomplishment (e.g., weekly meetings, towards an initial draft within 18 months).
        - A list of expected complementary documentation (e.g., open-source reference implementation, test vectors, code instruction).
    7. **References:** A list of technical/scientific references related to the WG goal.
    8. **Context:** The document cover should also include, below the title and team composition, the following text adequately filled: "Submitted on YYYY-Month-DD to the ZKProof Standards Committee". If the submission is an update of a previous abstract, then the cover should mention the current version number, and briefly acknowledge (in a footnote) the previous versions (and dates)."
2. **Abstract review/approval.** Upon internal analysis, the ZKProof Standards Committee will seek initial advisory opinion from the ZKProof Steering Committee and the ZKProof Editors Team. The follow up may then result in either (i) an approval (possibly with editorial suggestions), or (ii) a request for improvement/adjustment based on provided feedback, and subsequent resubmission of the WG abstract. Revisions to the abstract may be submitted under the same process, being identified with an incremental version number and date. (The team composition can be updated at any time, by simple information to the Standards Committee, for update on the webpage)
3. **WG Presentation.** After an initial review of the WG creation proposal, the Standards Committe will also invite the proposed WG to give a video-conference presentation about the goals and plan. The Editors and Steering Committe observers will also be invited to attend, for possible further feedback. In some cases this step can be replaced by a related public presentation at a ZKProof event.

## <a id="process-ZSpec"></a>Process for creating a ZKProof Specification (ZSpec)

Note: The ZKProof-Standards Committee will be available to meet with WGs to discuss suggestions of document structure for the ZSpec-Proposals.

1. **WG plan/abstract.** When the abstract submitted for a ZKProof WG creation (or update) is approved, the abstract will be **[published](http://docs.zkproof.org/standards/proposals)**, and the team will be invited to keep the ZKProof Standards Committee informed of any progress toward the intended specification.
2. **ZSpec-Proposal.** Within a suitable time frame after the approval of a WG abstract, the WG is expected to obtain as its first deliverable a **ZSpec-Proposal** (ZKProof Specification Proposal). The **ZSpec-Proposal** document is expected to be as close as possible to a complete specification (possibly also including a reference implementation), but it will be called a "proposal" because it still lacks a formal ZKProof presentation, discussion & review. The document is submitted (in PDF), via the ZKProof Standards Committee, for oral presentation (a talk) at a public ZKProof workshop/event. There may be a possible feedback/rebuttal process before acceptance for presentation. Once the **ZSpec-Proposal** is accepted for oral presentation, it should be made publicly available before the actual presentation. The talk should be recorded (for posterior video publication), and be included in a session that allows for ample discussion and feedback about the **ZSpec-Proposal**.
3. **ZSpec-Draft.** After the official presentation of the **ZSpec-Proposal**, the WG awaits at least 90 days for subsequent feedback. The WG takes in consideration all received feedback, and produces a new version called **ZSpec-Draft**. The WG submits to the ZKProof Standards Committee the **ZSpec-Draft**, along with a table documenting all the received feedback and how it was addressed. Note: ZKProof will make available a template document with this table, which will require at least: identifying (i) the comments' sources, (ii) the corresponding comments, (iii) explaining the update/reply produced by the WG, and (iv) other updates. The ZKProof Standards Committee will analyze the documentation and decide whether (i) to accept the **ZSpec-Draft** to initiate the next phase, or (ii) to request the WG to further address some of the comments, or provide some clarifications.
4. **ZCall for Comments.** Once there is an accepted **ZSpec Draft**, the WG and the Standards Committee will work together to produce an **Official ZKProof Call for Comments on a ZSpec-Draft**, with an open period of at least 90 days for comments. This call for comments will include a summarization of the process that the specification writing has already undergone, and will point out the goal of the process (such as outputting a final document to be considered as an approved "ZKProof Specification"). Soon after the 90 days (or whichever larger period open for comments), the WG should submit to the Standards Committee the list of received comments, and estimate how long it may take to address them all. Then, the WG will revise the ZSpec-Draft, taking in consideration all received feedback, and correspondingly documenting every edit.
6. **Approved ZSpec.** Once the WG is comfortable with a "final version" of their proposed specification, it will submit it for approval by the ZKProof Standards Committee, who, after consulting with the ZKProof Steering Committee and the ZKProof Editors Team, will issue a determination, either of approval of a new (final) **ZSpec** (ZKProof Specification) or will follow up with a request for further reviews (steps 2, 3 or 4), which may lead to new proposals or drafts. There may be various iterations of these steps (which might include further presentations, reviews, and public calls for feedback).
7. **ZSpec Publication.** Once a new **ZSpec** is approved (i.e., considered final), the ZKProof Standards Committee will ensure it is published in accordance with the ZKProof [Charter](https://docs.zkproof.org/general) and [IP Policy](https://docs.zkproof.org/general#intellectual-property-policy). In particular, the specification should be published under a Creative Commons CC 4.0 BY license, and any associated reference code should be placed under a permissive open-source license (e.g., MIT, ISC or BSD 2-Clause). It is encouraged that the ZSpec serves as a useful reference for standards at other Standards Development Organizations.
8. **Updated Versions** A new "Approved ZSpec" will by default get the version number 1.0. Version updates can be produced following a similar process (proposal/feedback/review/improvement sequence) covering the process of proposal/draft, although possibly with smaller review periods (at least 30 days each), decided by the ZKProof Standards Committee on a case-by-case basis, depending on how simple-to-review the updates are deemed.

For comments and updates, please email `standards at zkproof dot org`