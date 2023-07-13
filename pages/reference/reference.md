---
layout: default
title: Community Reference
nav_order: 4
has_children: true
permalink: /reference
---

# Community Reference
{: .no_toc }

ZKProof promotes best practices for proper development and deployment of zero-knowledge proof (ZKP) systems, aligned with security and interoperability. The ZKProof Community Reference (ZkpComRef) intends to comprehend terminology, examples, explanations and recommendations, driven by research and experience. This serves as a reference from and for the community.


The ZkpComRef is a live document. Check below for info about its version history and how to contribute. The latest PDF file compilation is available at https://docs.zkproof.org/reference.pdf

We are grateful and thank the many contributions!


## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## [Version 0.3](/pages/reference/versions/ZkpComRef-0-3.pdf)

Available since 2022-July-17. In a nutshell, the main update from [v0.2](/pages/reference/versions/ZkpComRef-0-2.pdf) to [v0.3](/pages/reference/versions/ZkpComRef-0-3.pdf) was the revision of the **paradigms** chapter. The old section "Taxonomy of constructions" was replaced by a new "Background" section, followed by two sections on "Information-Theoretic Proof Systems" and "Cryptographic Compilers". This change was inspired by Yuval Ishai's blog posts on IT proof systems [[1]([1](https://zkproof.org/2020/08/12/information-theoretic-proof-systems/)),[2](https://zkproof.org/2020/10/15/information-theoretic-proof-systems-part-ii/)]. The "IP based" subsection (under "Linear IOP") was provided by Justin Thaler. The revised chapter was structured and edited by the ZKProof Editors. Various editorial corrections were externally suggested, during the public review phase. Some were incorporated, others are queued for future revisions. Suggestions from Jens Groth improved Table 1.1 in Section 1.2.

The ZkpComRef 0.3 PDF file contains attached:
- a .bib file mentioning all contributors and the editors, to facilitate citation
- a .pdf file with a mindmap of the IT-proof systems

**Upcoming:** The call for contributions toward v0.4 will be published soon


## [Version 0.2](/pages/reference/versions/ZkpComRef-0-2.pdf)

Available since 2019-Dec-31. The changes are marked in a [diff file](/pages/reference/diffs/diff-v0.2-from-v0.1.pdf). Highlights of v0.2:
- A consolidated preamble: new abstract, new context “About this community reference”, new IP expectations; more detailed “Table of contents”; new “Executive summary”.
- A “Version history” section and an “Acknowledgments” section after the main chapters.
- A new chapter on “Construction paradigms”, encompassing the previous section on “Taxonomy” of constructions, and including a new section on “Interactivity”.
- Several portions of revised text and content, for example on proofs of knowledge vs. membership, benchmark parameters, gadgets, and applications.


### Call for Feedback for v0.3

We are open for public feedback on all aspects of the ZKProof Community Reference version 0.2. The feedback will be helpful to prepare topics of discussion at the [3rd ZKProof workshop (April 20 – May 21)](https://zkproof.org/events/workshop3), which will kick-off a new cycle open to contributions. Please send your feedback by email to [editors@zkproof.org](mailto:editors@zkproof.org). When commenting on specific portions of text, please refer to the line numbers in the ["annotated changes" version](/pages/reference/diffs/changes-v0.2-from-v0.1.pdf). Note that the [ZKProof community forum](https://community.zkproof.org) also remains as a resource for community discussion.

**Here is a list of examples of feedback we are looking for**

- What portions of technical text can benefit from further clarification?
- What basic concepts to further clarify, such as membership vs. knowledge, etc?
- Each item in section 2.3 should be expanded into a new section — what to include?
- What new pictorial examples (diagrams, etc.) to add?
- What bibliographic references to add, to better support the claims and concepts?


## Version History of the ZkpComRef

Date | Version Nº (PDF link) | Version hint | Editors | Other Links
-----|---------|-------|---------|---------
2022-Jul-17 |  [0.3](/pages/reference/versions/ZkpComRef-0-3.pdf) | (ZkpComRef) **Paradigms** addon | Daniel Benarroch, Luís Brandão, Mary Maller, Eran Tromer | [Diff PDF (0.2→0.3)](https://github.com/zkpstandard/zkreference/raw/master/diff-v0.3-from-v0.2.pdf)
2019-Dec-31 | [0.2](/pages/reference/versions/ZkpComRef-0-2.pdf) | (ZkpComRef) **Consolidated** draft | Daniel Benarroch, Luís Brandão, Eran Tromer | [Diff PDF (0.1→0.2)](/pages/reference/diffs/diff-v0.2-from-v0.1.pdf) & [Annotated changes (0.1→0.2)](/pages/reference/difs/changes-v0.2-from-v0.1.pdf)
2019-Apr-11 | [0.1](/pages/reference/versions/ZkpComRef-0-1.pdf) | (ZkpComRef) 1st **LaTeX/PDF** compilation | Luís Brandão | [GitHub repo](https://github.com/zkpstandard/zkreference)
2018-May-12 | [0.0-security](/pages/reference/versions/zkproof-security-20180801.pdf) | Proceedings Track **Security**  | Jens Groth, Yael Kalai, Muthu Venkitasubramaniam | [Google Doc](https://docs.google.com/document/d/1uXKovVpYuXRybCpFH97iMm9IVhzr2zfWCzrVm9jl5JA/edit?usp=sharing)
2018-May-12 |  [0.0-imple</br>mentation](/pages/reference/versions/zkproof-implementation-20180801.pdf) | Proceedings Track **Implementation** | Sean Bowe, Kobi Gurkan, Eran Tromer | [Google Doc](https://docs.google.com/document/d/1gcSXlQp1NOSza-8dBczL3X0KbLNvsYn4JXbpDMhUF2c/edit?usp=sharing)
2018-May-12 | [0.0-appli</br>cations](/pages/reference/versions/zkproof-applications-20180801.pdf) | Proceedings Track **Applications**  | Daniel Benarroch, Ran Canetti, Andrew Miller | [Google Doc](https://docs.google.com/document/d/1spgtYG8iXZ_NjUXdN8AEdKdGmaulE8r-mf7NsQ-_y4E/edit?usp=sharing)
