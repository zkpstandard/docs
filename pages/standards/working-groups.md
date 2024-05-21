---
layout: default
title: Working Groups
parent: ZKProof Standards
nav_order: 2
permalink: /standards/wg
---
# ZKProof Working Groups (WG)
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

The purpose of this webpage is to identify [current](#wg-current) and [past](#wg-past) ZKProof Working Groups, and provide quick links to some of their reference material. ZKProof supports the dissemination of WG's reference material for community discussion, but each WG is reponsible for their own goals and documentation, including the descriptions provided below.

<a id="wg-current"></a>
## Working Groups since 2024

Since the creation of the [ZKProof Standards Committee](https://docs.zkproof.org/standards) (2023), and the [process for WG creation](https://docs.zkproof.org/standards/process#process-WG) (2024), the following groups have been created:

<a id="fiat-shamir"></a>
### Fiat-Shamir Compiler
The Fiat-Shamir heuristic is a method for transforming a public-coin interactive proof into a non-
interactive proof via cryptographic hash functions. This project aims to bridge the theoretical and practical aspects of the Fiat-Shamir transforms. The WG's goal is to develop a technique that is easy to implement using sponge functions, algebraic hashes, and the NIST SHA2 API (update and digest) now used in most programming languages.
- Team contact: `[TBA]`
- Main repo: `[TBA]`

<a id="oracle"></a>
### Oracle Compilers
An oracle compiler converts an interactive oracle proof (IOP) into an interactive proof (IP). In practice, this involves composing the IOP with a cryptographic commitment scheme, resulting in an interactive argument. The primary purpose of the Oracle Compiler Working Group is to define a high-level interface between IOPs and commitment schemes, informed by protocols and implementations being used in the wider community. Details relating to only IOPs (e.g. rounds of interaction) are not in the scope of this working group.
- Team contact: `zkproof-oracle-compilers(at)googlegroups(dot)com`
- Main repo: `[TBA]`

<a id="plonkish"></a>
### Plonkish Constraint System
An arithmetisation is a language that a proof system uses to express statements. A circuit is a program in this language. The associated computation has been computed correctly if and only if all of the constraints in the circuit are satisified. The primary purpose of this ZKProof Working Group is to specify a particular arithmetisation: the "Plonkish" arithmetisation used in the Halo 2 proving system.
- Team contact: `plonkish-team(at)googlegroups(dot)com`
- Main repo: https://github.com/zkpstandard/wg-plonkish

<a id="sigma"></a>
### Sigma Protocols
Sigma ($\Sigma$) protocols, introduced by Schnorr in 1991, play an essential component in the building of a  number of cryptographic constructions, such as anonymous credentials, password-authenticated key exchange, signatures, ring signatures, blind signatures, multi-signatures, threshold signatures and more. This WG (continuing the work proposal submitted in 2021 to ZKProof Workshop 4) develops guidelines for correctly implementing Sigma protocols.
- Team contact: `sigma-protocols(at)zkproof(dot)org`
- Main repo: https://github.com/zkpstandard/wg-sigma-protocols


<a id="wg-past"></a>
## Working groups prior to 2022

Between 2019 and 2021, ZKProof motivated the submission of proposals for specifications, and the creation of various working groups.

Throughout various ZKProof workshops, "proposals" were submitted for discussion by the community. Some of these led to the creation of "working groups" (WG) intended to subsequently develop/refine/improve the proposals, possibly toward future standards. While they have not been subject to any formal process for subsequent standardization, they have produced various documents (see below) that may serve as useful reference material.

Note: there is another webpage with a [list of initial proposals](https://docs.zkproof.org/standards/proposals) submitted to ZKProof workshops.


| \#| WG Name (Telegram Group) | Goal | Repo | Documents |
| - | -------- | -------- | ----- | ----|
| 1 | Commit-and-Prove ZKP Systems & Extensions ([TG](https://t.me/joinchat/Ua0M-VFxwB59HA-u)) | Standardize how to modularly create verifiable commitments and ciphertexts with any ZK system  |  [repo](https://github.com/dariofiore/wg-cpzkp-standard)  |   [W2](https://docs.zkproof.org/pages/standards/accepted-workshop2/proposal--zk-commit-and-prove.pdf), [W3](), [W4](https://docs.zkproof.org/pages/standards/accepted-workshop4/proposal-commit.pdf), [Notes](https://hackmd.io/@workshop4/commit), [Slides](https://www.binarywhales.com/assets/misc/CP-standard-ZKProof-slides.pdf),  [Charter](https://hackmd.io/@dariofiore/rkXo8EBp8) |
| 2 | Σ-protocols ([TG](https://t.me/joinchat/Bg3emHC1tD04N2Jk)) | Standardize ZK interactive sigma protocols| [repo](https://github.com/zkpstandard/wg-sigma-protocols) | [W4](https://docs.zkproof.org/pages/standards/accepted-workshop4/proposal-sigma.pdf) |
| 3 | DAPOL ([TG]()) | v | --- | [W3](https://eprint.iacr.org/2020/468), [CCS21](https://eprint.iacr.org/2021/1350), [ACNS21](https://eprint.iacr.org/2021/239), [Notes](https://hackmd.io/wTDRz9xUR4SrYSO3HSq9Jg?view) |
| 4 | zkInterface ([TG](https://t.me/joinchat/WMsiVhK9n6avLeuo)) | Standardize interoperability between frontends and backends in ZK systems | [repo](https://github.com/QED-it/zkinterface) | [W2](https://docs.zkproof.org/pages/standards/accepted-workshop2/proposal--zk-interop-zkinterface.pdf), [W3](https://docs.zkproof.org/pages/standards/accepted-workshop3/proposal-zkinterface.pdf), [Notes](https://hackmd.io/@HtwXZr-PTFCniCs7fWFSmQ/ryoXg2BYL) |
| 5 | Snark-Friendly Primitives ([TG](https://t.me/joinchat/VM4YKXPiLq0Lxkuh)) | Standardize the use of specific cryptographic primitives inside of the circuit of a ZK system | [repo](https://github.com/daira/zkproof) | [Charter](https://hackmd.io/AY8DfYzyQiaSHbrhSmgOpQ), [Notes](https://hackmd.io/@workshop4/zcr-primitives) |


## Other Discussion Groups

| \#| WG Name (Telegram Group) | Goal | Repo | Documents |
| - | -------- | -------- | ----- | ----|
| 1 | Groth16 & SnarkPack ([TG](https://t.me/joinchat/2AivFqHTj4ViYTNk)) | Standardize Groth16 and aggregation/amortization methods | --- | [W4](https://docs.zkproof.org/pages/standards/accepted-workshop4/proposal-aggregation.pdf), [Notes](https://hackmd.io/@workshop4/aggregation)|
| 2 | Rinocchio: SNARKs for Ring Arithmetic ([TG](https://t.me/joinchat/3HS-fhBs5II5NDY0)) | Standardize a generic method for using ZK over rings, yielding efficiency improvements for some applications | --- | [W4](https://docs.zkproof.org/pages/standards/accepted-workshop4/proposal-rinocchio.pdf), [Notes](https://hackmd.io/@workshop4/rinocchio) |
| 3 | Leo: A Programming Language for Formally Verified ZK Applications ([TG](https://t.me/leolanguage)) | Standardize the fundamental components of a ZK language | --- | [W4](https://docs.zkproof.org/pages/standards/accepted-workshop4/proposal-leo.pdf), [Notes](https://hackmd.io/@workshop4/leo) |

**Legend:** **W2** = paper @ 2th workshop; **W3** = paper @ 3rd workshop; **W4** = paper @ 4th workshop.


For comments and updates, send email to `standards at zkproof dot org`