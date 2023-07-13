---
layout: default
title: Concrete Schemes
nav_order: 7
has_children: false
permalink: /schemes
---

# ZKProof Wiki of Concrete ZKP Schemes

This wiki (ongoing work) is a resource complementary to the [ZKProof Community Reference](pages/reference/reference
.pdf). The goal is to collect in one place many references about concrete ZKP schemes. For each scheme there is a
 summarized description and various references to available public resources. 

Schemes described here should have a rigorous technical writeup which fully specifies the scheme; clearly states its security properties, model and assumptions; and proves its security (at least at the proof-sketch level).

The following is not an exhaustive list.  It contains references listed in a previous version of the ZkpComRef, as
 well as others suggested during edits. Clearly there are more relevant entries to add --- please send an email to
  [editors@zkproof.com]() with your suggestions. Better yet, submit a pull request to the [resources GitHub repo](https://github.com/zkpstandard/docs)
  or submit a description at [https://forms.gle/NGm9xpUJBDyy6UFr6](https://forms.gle/NGm9xpUJBDyy6UFr6), following
   the [instructions](#Template) further below.

-----------------------
# Index

## Described:

The descriptions are based on contributions obtained via [https://forms.gle/NGm9xpUJBDyy6UFr6](https://forms.gle/NGm9xpUJBDyy6UFr6)

- [2021](#2021): [TurboIKOS](#TurboIKOS) \[GHSVYZ21\], [BooLigero](#BooLigero) \[GSV21\]
- [2020](#2020): [Marlin](#Marlin) \[CHMMVW19\], [Virgo](#Virgo) \[ZXZS19\], [Virgo++](#Virgo++) \[ZLWZSXZ20
\], [Ligero++](#Ligero++) \[BFHVXZ20\], [Mac’n’Cheese](#Mac'n'Cheese) \[BMRS20\]
- [2019](#2019): [Sonic](#Sonic) \[MBKM19\], [Libra](#Libra) \[XZZPS19\], [kimleeoh](#kimleeoh) \[KLO19\], [SAVER](#SAVER) \[YZ20\]
- [2017](#2017): [vSQL](#vSQL) \[ZGKPP17\]

---
## To be described:

The following schemes are yet to be described in the [template format](#Template) provided below.

- **2022:** [NIZK Multiple Verifiers](https://ia.cr/2022/063) \[YW22\], [Feta](https://ia.cr/2022/082) \[BJOSS22\], [gOTzilla](https://ia.cr/2022/170) \[BCGHM22\], [ZK UNSAT](https://ia.cr/2022/206) \[LAHPTW22\]
- **2021:** [Manta](https://ia.cr/2021/743) \[CXZ21\], [Nova](https://ia.cr/2021/370) \[KST21\], [Rinocchio](https://ia.cr/2021/322) \[GNS21\], [Limbo](https://ia.cr/2021/215) \[DGOT21\], [QuickSilver](https://ia.cr/2021/076) \[YSWW21\], [Limbo](https://ia.cr/2021/215) \[GOT21\], [IntRange](https://ia.cr/2021/540) \[CKLR21\], [SubexpDDH](https://ia.cr/2021/514) \[JJ21\], [Cerberus](https://ia.cr/2021/030) \[LSTW21\], [ConstOverZKRamProgs](https://ia.cr/2021/979) \[FKLOW21\]
- **2020:** [HaloInfinite](https://ia.cr/2020/1536) \[BDFG20\], [Quarks (Xiphos and Kopis)](https://ia.cr/2020/1275) \[SL20\], [Dory](https://ia.cr/2020/1274) \[Lee20\], [Wolverine](https://ia.cr/2020/925) \[WYKW20\], [Bulletproofs+](https://ia.cr/2020/735) \[CHJKS20\], [SPARKS](https://ia.cr/2020/994) \[EFKP20\], [Plookup](https://ia.cr/2020/315) \[GW20\], [SuperSonic](https://ia.cr/2019/1229) \[BFS20\], [CompressedSigma](https://ia.cr/2020/152) \[AC20\], [LatticeZKviaOTC](https://ia.cr/2020/1448) \[LKS20\], [GeneralizedCompressedSigma](https://ia.cr/2020/1447) \[ACR20\], [PVZKfromBlockchain](https://ia.cr/2020/1435) \[SSV20\], [LinePointZK](https://ia.cr/2020/1446) \[DIO20\], [PublicCoinZKTime&Space](https://ia.cr/2020/1425) \[BHRRS20\], [Dory](https://ia.cr/2020/1274) \[Lee20\], [DoublyEfficientIP](https://ia.cr/2020/1247) \[ZLWZSXZ20\], [PqSnarks4Rsis-Rlwe](https://ia.cr/2020/1190) \[BCOS20\], [ZAPsAlgebraicLangs](https://ia.cr/2020/286) \[CH20\]
- **2019:** [Fractal](https://ia.cr/2019/1076) \[COS19\], [Halo](https://ia.cr/2019/1021) \[BGH19\], [Plonk](https://ia.cr/2019/953) \[GWC19\], [RedShift](https://ia.cr/2019/1400) \[KPV19\], [Spartan](https://ia.cr/2019/550) \[Setty19\], [Deep FRI](https://arxiv.org/abs/1903.12243) \[BGKS19\], [LatticeZKPs](https://ia.cr/2019/445) \[ESLL19\], [SubversionResistant](https://ia.cr/2019/1162) \[Bag19\], [Darks](https://ia.cr/2019/1229) \[BFS19\], [LatticeSnarkArithmetic](https://ia.cr/2019/1251) \[Nit19\], [ZKPSetMembership](https://ia.cr/2019/1255) \[BCFGD19\]
- **2018:** [Aurora](https://ia.cr/2018/828) \[BCRSVW18\], [FRI](https://doi.org/10.4230/LIPIcs.ICALP.2018.14) \[BBHR18\], [ZKStarks](https://ia.cr/2018/046) \[BBHR18\], [Picnic2](https://ia.cr/2018/475) \[KKW18\], [vRAM](https://doi.org/10.1109/SP.2018.00013) \[ZGKPP18\] (can add to existing vSQL section), [DIZK](https://ia.cr/2018/691) \[WZCPS18\], [UpdatableNIZK](https://ia.cr/2018/280) \[GKMM18\], [HybNIZK](https://ia.cr/2018/557) \[AGM18\]
- **2017:** [Ligero](https://acmccs.github.io/papers/p2087-amesA.pdf) (AHIV17), [ZKB++ and Picnic](https://ia.cr/2017/279) \[CDGORRSZ17\] (discuss alongside ZKBoo), [Hyrax](https://ia.cr/2017/1132) \[WTsTW\], [zk-vSQL](https://ia.cr/2017/1146) \[ZGKPP17\] (can add to existing vSQL section), [Bulletproofs](https://ia.cr/2017/1066) \[BBBPWM17\], [SnarkySigs](https://ia.cr/2017/540) \[GM17\]
- **2016**: [ZKBoo](https://ia.cr/2016/163) \[GMO16\], [BulletproofsPrequel](https://ia.cr/2016/263) \[BCCGP16\], [Groth16](https://ia.cr/2016/260) \[Groth16\], [HybIntZK](https://ia.cr/2016/583) \[CGM16\]
- **2015:** [IP4Muggles](https://eccc.weizmann.ac.il/report/2017/108/) \[GKR15\], [SNARKs-for-MapReduce](https://ia.cr/2015/377) \[CTV15\]
- **2014:** [Geppetto](https://ia.cr/2014/976) \[CFHKKNPZ14\], [CyclesOfCurves](https://ia.cr/2014/595) \[BCTV14\]
- **2013:** [Pinocchio](https://ia.cr/2013/279) \[PGHR13\], [SNARKs-for-C](https://ia.cr/2013/507) \[BCGTV13\], [ZK-vonNeumann](https://ia.cr/2013/879) \[BCTV13\]
- **2012:** [QSP](https://ia.cr/2012/215) \[GGPR12\], [EfficientPCP](https://doi.org/10.1007/978-3-642-28914-9_9) \[IMS12\], [Succinct-NIArgs-LIP](https://ia.cr/2012/718) [BCIOP12]
- **2010:** [Short-PB-NIZKA](https://www.iacr.org/archive/asiacrypt2010/6477323/6477323.pdf) \[Groth10\], [Preprocessing-Verifiable-Computation](https://ia.cr/2009/547) \[GGP10\]
- **2007:** [IKO](https://web.cs.ucla.edu/~rafail/PUBLIC/79.pdf) \[IKO07\], [IVC](https://dspace.mit.edu/bitstream/handle/1721.1/38663/163581090-MIT.pdf) \[V07\]
- **1990s:** [NIZKs-for-NP](https://doi.org/10.1145/116825.116852) \[GMW91\], [KillianPCP](https://people.csail.mit.edu/vinodv/6892-Fall2013/efficientargs.pdf) \[Kilian92\], [CS-proofs](https://doi.org/10.1137/S0097539795284959) \[Micali94\], [ZKP-for-Free?](https://doi.org/10.7146/brics.v4i27.18953) \[CD98\]
- **1980s:** [ZKP](https://doi.org/10.1137/0218012) \[GMR85\], [NIZK](https://doi.org/10.1145/62212.62222) \[BFM88\], [PoK of DL](https://doi.org/10.1007/0-387-34805-0_22) \[Sch89\]



## How to submit a description:
- **[Template description](#Template) and submission instructions**


------------------------------------
# Described Schemes:

## <a id="2021"></a>2021

### <a id="TurboIKOS"></a>TurboIKOS
- **Available resources:** [paper@IACR](https://eprint.iacr.org/2021/478); [code@GitHub](https://github.com/sarahscheffler/TurboIKOS);
- **Where presented:** ACNS 2021 (June)
- **Kind of statements:** General arithmetic circuits in low RAM settings, especially small circuits
- **Information theoretic (IT) system:** MPC-in-the-Head
- **Cryptographic compiler:** IKOS compiler from (semi-honest) MPC protocol to ZKP
- **Complexity/efficiency:** Prover runtime: linear. Verifier runtime: linear. Communication: linear (2 field elements per mult gate per repetition achieving soundness in Theorem 3, plus log(parties) overhead). Round complexity: constant (5 rounds)
- **Models and assumptions:** One-way functions. Smaller weak commitments use ROM (can be removed). Non-interactivity achieved via Fiat-Shamir. 
- **Relation to other schemes:** Focus is on concrete communication/proof size improvement within the setting of asymptotically linear MPC-in-the-head proofs. Shrinks Baum and Nof's PKC 2020 scheme from 4 field elems per gate to 2 field elems per gate. Our scheme has competitive communication/size with Katz, Kolesnikov, and Wang's CCS 2018 scheme with a different parameter tradeoff; our scheme is better for fewer emulated MPC parties (which would occur if lower runtime is desired compared to proof size).


**BibTex citation**
```bibtex
@inproceedings{ACNS:GHSVYZ21,
    title={TurboIKOS: Improved Non-Interactive Zero Knowledge and Post-Quantum Signatures},
    author={Yaron Gvili and Julie Ha and Sarah Scheffler and Mayank Varia and Ziling Yang and Xinyuan Zhang},
    editor = {Kazue Sako and Nils Ole Tippenhauer},
    booktitle = {Applied Cryptography and Network Security},
    volume = {12727},
    address = {Kamakura, Japan},
    month = {June},
    publisher = "Springer, Heidelberg",
    series = "Lecture Notes in Computer Science",
    year = 2021
}
```

### <a id="BooLigero"></a>BooLigero
- **Available resources:** [paper@IACR](https://eprint.iacr.org/2021/121); <span style="color:red">No GitHub Code</span>
- **Where presented:** FC 2021 (March)
- **Kind of statements:** Boolean circuits over "words", especially those containing many (possibly different) subcircuits of linear operations that yield 0 over bits (such as bit masking, even parity testing, permutations of bits within or across words, or similar operations)
- **Information theoretic (IT) system:** MPC-in-the-Head, Interactive Oracle Proofs (IOP)
- **Cryptographic compiler:** BCS'16 (IOP), AHIV'17 (Ligero)
- **Complexity/efficiency:** Prover runtime: $S \cdot log(S)$ where $S$ is circuit size. Verifier runtime: S*log(S) where S is circuit size. Communication: $\sqrt{S}$ where $S$ is circuit size. Round complexity: constant
- **Models and assumptions:** Coding theoretic assumption (same as Ligero: AHIV'17 Lemma 4.2). Non-interactivity comes from Fiat-Shamir.
- **Relation to other schemes:**  Improves Boolean circuit proof size over original Ligero (Ames, Hazay, Ishai
, Venkitasubramaniam CCS'17) by $\sqrt{log(\|F\|)}$ where $F$ is the field; $F$ has a minimum size for Ligero to
 function. In practice this tends to be about a 1-4x proof size reduction.  Further improves upon Ligero by using highly batchable testing for Boolean relations such as a bit masking, even parity, permutations of bits, etc.

**BibTex citation**

```bibtex
@inproceedings{FC:GviSchVar21,
    title={BooLigero: Improved Sublinear Zero Knowledge Proofs for Boolean Circuits},
    author={Gvili, Yaron and Scheffler, Sarah and Varia, Mayank},
    booktitle = {Financial Cryptography and Data Security},
    month = {March},
    publisher = "Springer, Heidelberg",
    series = "Lecture Notes in Computer Science",
    year = 2021
}
```


## <a id="2020"></a>2020

### <a id="Marlin"></a>Marlin
- **Resources:** [paper@IACR](https://eprint.iacr.org/2019/1047); [paper@Springer](https://doi.org/10.1007/978-3-030-45721-1_26); [code@GitHub](https://github.com/arkworks-rs/marlin); [implementation diagram](https://github.com/arkworks-rs/marlin/blob/master/diagram/diagram.pdf); [video@Youtube](https://youtube.com/watch?v=3mZWa6tJaMI).
- **Where presented:** [EUROCRYPT 2020](https://eurocrypt.iacr.org/2020/program.php)
- **Kind of statements:** General arithmetic circuits/R1CS
- **Information theoretic (IT) system:** Interactive Oracle Proofs (IOP), Polynomial IOP
- **Cryptographic compiler:** Polynomial commitment schemes
- **Complexity/efficiency:** Efficiency depends on the maximum number of non-zero entries N across the matrices. When used with Marlin variant of KZG10, over BLS12-381: Proof size: 784 bytes. PK size: $3N$. VK size: 12 G1 + 2 G2. Verification time: < 8ms. Proving time: $O(N)$-sized MSMs over G1
- **Models and assumptions:** ROM + AGM
- **Relation to other schemes:** Alternative to Groth16 that provides universal setup. Alternative to standard that works with R1CS directly

**BibTex citation**

```bibtex
@inproceedings{ChiesaHMMVW20,
    author = {Chiesa, Alessandro and Hu, Yuncong and Maller, Mary and Mishra, Pratyush and Vesely, Noah and Ward, Nicholas},
title = {Marlin: Preprocessing {zkSNARKs} with Universal and Updatable {SRS}},
    booktitle = {Proceedings of the 39th Annual International Conference on the Theory and Applications of Cryptographic Techniques},
    series = {EUROCRYPT~'20},
    pages = {738--768},
    year = {2020},
}
```

### <a id="Virgo"></a>Virgo
- **Available resources:** [paper@IACR](https://eprint.iacr.org/2019/1482); [code@GitHub](https://github.com/sunblaze-ucb/Virgo)
- **Where presented:** IEEE S&P 2020
- **Kind of statements:** Layered arithmetic circuits
- **Information theoretic (IT) system:** Interactive Oracle Proofs (IOP). Combines the IP in GKR with a polynomial commitment based on IOP
- **Cryptographic compiler:** Polynomial commitments
- **Complexity/efficiency:** Prover $O(C+n\log n)$; verifier $O(d\log C+\log^2 n)$; proof size $O(d \log C+\log^2 n)$; transparent setup with $O(1)$ RRS; non-interactive through Fiat-Shamir
- **Models and assumptions:** Collision-resistant hash and ROM, Fiat-Shamir to remove interactivity
- **Relation to other schemes:** It proposes a new polynomial commitment in IOP that removes the trusted setup.

**BibTex citation**

```bibtex
@inproceedings{zhang2020transparent,
    title={Transparent polynomial delegation and its applications to zero knowledge proof},
    author={Zhang, Jiaheng and Xie, Tiancheng and Zhang, Yupeng and Song, Dawn},
    booktitle={2020 IEEE Symposium on Security and Privacy (SP)},
    pages={859--876},
    year={2020},
    organization={IEEE}
}
```


### <a id="Virgo++"></a>Virgo++
- **Available resources:** [paper@IACR](https://eprint.iacr.org/2020/1247); [code@GitHub](https://github.com/TAMUCrypto/virgo-plus)
- **Where presented:** 
- **Kind of statements:** General arithmetic circuits
- **Information theoretic (IT) system:** Interactive Oracle Proofs (IOP). develops a new IP for general arithmetic circuits
- **Cryptographic compiler:** Polynomial commitments
- **Complexity/efficiency:** Prover $O(C+n\log n)$; verifier $O(d\log C+d^2+\log^n)$; proof size $O(d\log C+d^2+\log^n)$; transparent setup with $O(1)$ RRS; non-interactive through Fiat-Shamir
- **Models and assumptions:** collision-resistant hash and ROM, Fiat-Shamir
- **Relation to other schemes:** It generalizes the GKR protocol to general arithmetic circuits while keeping the prover time $O(C)$.

**BibTex citation**

```bibtex
@inproceedings{zhang2021doubly,
    author = {Jiaheng Zhang and Tianyi Liu and Weijie Wang and Yinuo Zhang and Dawn Song and Xiang Xie and Yupeng Zhang},
    title = {Doubly Efficient Interactive Proofs for General Arithmetic Circuits with Linear Prover Time},
    booktitle = {Proceedings of the ACM SIGSAC Conference on Computer and Communications Security (CCS)},
    year = {2021},
}
```

### <a id="Ligero++"></a>Ligero++
- **Available resources:** [paper@CCS2020](https://doi.org/10.1145/3372297.3417893)
- **Where presented:** CCS 2020
- **Kind of statements:** R1CS
- **Information theoretic (IT) system:** Interactive Oracle Proofs (IOP)
- **Cryptographic compiler:** IOP. FRI
- **Complexity/efficiency:** Prover $O(C\log C)$; verifier $O(\log^2 C)$; proof size $O(\log^2 C)$; transparent setup with $O(1)$ RRS; non-interactive through Fiat-Shamir.
- **Models and assumptions:** collision resistant hash and ROM, Fiat-Shamir
- **Relation to other schemes:** It improves the proof size of Ligero to $O(\log^C)$ using the IOP of Aurora and Virgo

**BibTex citation**

```bibtex
@inproceedings{bhadauria2020ligero++,
    title={Ligero++: a new optimized sublinear IOP},
    author={Bhadauria, Rishabh and Fang, Zhiyong and Hazay, Carmit and Venkitasubramaniam, Muthuramakrishnan and Xie, Tiancheng and Zhang, Yupeng},
    booktitle={Proceedings of the 2020 ACM SIGSAC Conference on Computer and Communications Security},
    pages={2025--2038},
    year={2020}
}
```


### <a id="Mac'n'Cheese"></a>Mac'n'Cheese
- **Available resources:** [paper@IACR](https://eprint.iacr.org/2020/1410)
- **Where presented:** 
- **Kind of statements:** Circuits with disjunctions, General circuits
- **Information theoretic (IT) system:** Linear PCP, Ideal Linear Commitment (ILC), IPs with Linear Oracle Verification. It uses basic homomorphic MACs (similar to ILCs) to commit to the witness and then verifies the witness using Linear IOP/ILC techniques
- **Cryptographic compiler:** vOLEs to implement homomorphic MACs, inner product argument to verify product relations
- **Complexity/efficiency:** Prover and verifier time as well as memory are linear in statement size. The online
 proof size is $1+\varepsilon$ field elements per multiplication for arbitrary circuits and decreases to $O(max(\|C_i\|) + log(m))$ for a disjunction over $m$ circuits $C_i$. The computation/communication cost for the preprocessing is linear as well, but communication is much lower: per vOLE in $\mathbb{F}_{2^{61}-1}$ the communication is $0.42$ bits using e.g. Wolverine.
- **Models and assumptions:** LPN assumption to instantiate the vOLE, ROM (Fiat-Shamir) to reduce round complexity
- **Relation to other schemes:** The protocol is related to the Wolverine protocol, although Mac'n'Cheese has a lower communication complexity. It has a comparable, although slightly worse, communication complexity than Quicksilver, and a comparable runtime to it. In comparison to Wolverine & Quicksilver, Mac'n'Cheese has a low communication overhead for disjunctions for which it is optimized.

**BibTex citation**

```bibtex
@inproceedings{C:BMRS21,
    author = {Carsten Baum and
              Alex J. Malozemoff and
              Marc B. Rosen and
              Peter Scholl},
    title = {Mac'n'Cheese: Zero-Knowledge Proofs for Boolean and Arithmetic Circuits with Nested Disjunctions},
  booktitle={Annual International Cryptology Conference},
  year={2021},
  organization={Springer}
}
```

## <a id="2019"></a>2019

### <a id="Sonic"></a>Sonic
- **Available resources:** [paper@CCS'19](https://doi.org/10.1145/3319535.3339817); [paper@IACR](https://eprint.iacr.org/2019/099); [code@GitHub](https://github.com/ebfull/sonic)
- **Where presented:** [CCS'19](https://www.sigsac.org/ccs/CCS2019/) 
- **Kind of statements:** General purpose circuits. Best when the same circuit (for different statements) is proven multiple times and there exists a "helper" to aggregate.
- **Information theoretic (IT) system:** Polynomial IOP. Algebraic holographic proof. A polynomial IOP where the verifier can query on linear combinations of the polynomial oracles.
- **Cryptographic compiler:** Polynomial commitments.  Bilinear pairings.
- **Complexity/efficiency:** Prover time = $O(n\log(n))$, prover memory $(n\log(n))$, proof size = $O(1)$, verifier time and memory = $O(1)$ aggregated or $O(n)$ non-aggregated, "post"-processing, non-interactive under Fiat-Shamir, aggregating time = $O(n)$.
- **Models and assumptions:** ROM and (bilinear) algebraic group model.
- **Relation to other schemes:** Preceeds Plonk and Marlin which are efficient with preprocessing
- **Other comments:** Aggregator improves verifier time rather than proof size.

**BibTex citation**

```bibtex
@inproceedings{MallerBKM19,
  author    = {Mary Maller and
               Sean Bowe and
               Markulf Kohlweiss and
               Sarah Meiklejohn},
  title     = {Sonic: Zero-Knowledge SNARKs from Linear-Size Universal and Updatable
               Structured Reference Strings},
  booktitle = {Proceedings of the 2019 {ACM} {SIGSAC} Conference on Computer and
               Communications Security, {CCS} 2019, London, UK, November 11-15, 2019},
  pages     = {2111--2128},
  year      = {2019},
}
```



### <a id="Libra"></a>Libra
- **Available resources:** [paper@IACR](https://eprint.iacr.org/2019/317); [code@GitHub](https://github.com/sunblaze-ucb/Libra)
- **Where presented:** Crypto 2019
- **Kind of statements:** Layered arithmetic circuits
- **Information theoretic (IT) system:** Linear IOP. It combines the IP of GKR with a polynomial commitment.
- **Cryptographic compiler:** polynomial commitments
- **Complexity/efficiency:** Prover $O(C)$; verifier $O(d\log C)$; proof size $O(d\log C)$; trusted setup with SRS of $O(C)$; non-interactive through Fiat-Shamir.
- **Models and assumptions:** Extractability & KoE, ROM to remove interactivity
- **Relation to other schemes:** Improves the prover time of the GKR protocol to linear in circuit size for any layered arithmetic circuit.

**BibTex citation**

```bibtex
@inproceedings{xie2019libra,
  title={Libra: Succinct zero-knowledge proofs with optimal prover computation},
  author={Xie, Tiacheng and Zhang, Jiaheng and Zhang, Yupeng and Papamanthou, Charalampos and Song, Dawn},
  booktitle={Annual International Cryptology Conference},
  pages={733--764},
  year={2019},
  organization={Springer}
}
```

### <a id="kimleeoh"></a>kimleeoh
- **Available resources:** [paper@IEEE](https://doi.org/10.1109/ACCESS.2020.3019980); [paper@IACR](https://eprint.iacr.org/2019/586)
- **Where presented:** IEEE Access Vol. 8
- **Kind of statements:** quadratic arithmetic circuit
- **Information theoretic (IT) system:** Linear PCP. 
is constructed from the quadratic arithmetic program (QAP), same as in Groth16.
- **Cryptographic compiler:** Bi-linear pairings, same as in Groth16.
- **Complexity/efficiency:** It is a Groth16 variant, which adds simulation extractability. The verification time and the proof size is equivalent to Groth16, and the proving time is similar to Groth16 (same complexity).
- **Models and assumptions:** ROM, algebraic model, KoE
- **Relation to other schemes:** It adds simulation-extractability to Groth16, without sacrificing the proof size and other general computations, by using the hash function.

**BibTex citation**

```bibtex
@article{kim2020simulation,
  title={Simulation-extractable zk-SNARK with a single verification},
  author={Kim, Jihye and Lee, Jiwon and Oh, Hyunok},
  journal={IEEE Access},
  volume={8},
  pages={156569--156581},
  year={2020},
  publisher={IEEE}
}

```

### <a id="SAVER"></a>SAVER
- **Available resources:** [paper@IACR](https://eprint.iacr.org/2020/1270)
- **Where presented:** ???
- **Kind of statements:** Quadratic arithmetic circuit
- **Information theoretic (IT) system:** Linear PCP. It is constructed from quadratic arithmetic circuit.
- **Cryptographic compiler:** Bi-linear pairings
- **Complexity/efficiency:** It improves the efficiency of proving (public-key) encryption, compared with using existing ZKP schemes. It achieves the proving time of less than 1ms, while Groth16 requires 9s for proving RSA-OAEP-2048.
- **Models and assumptions:** Algebraic model, KoE
- **Relation to other schemes:** It takes the idea of commit-and-prove and extends it to encrypt-and-prove to improve the efficiency of encryption.

**BibTex citation**

```bibtex
@article{lee2019saver,
  title={SAVER: Snark-friendly, Additively-homomorphic, and Verifiable Encryption and decryption with Rerandomization.},
  author={Lee, Jiwon and Choi, Jaekyoung and Kim, Jihye and Oh, Hyunok},
  journal={IACR Cryptol. ePrint Arch.},
  volume={2019},
  pages={1270},
  year={2019}
}
```

## <a id="2018"></a>2018

To be described.

## <a id="2017"></a>2017

### <a id="vSQL"></a>vSQL
- **Available resources:** [paper@IACR](https://eprint.iacr.org/2017/1145); [paper@IACR](https://eprint.iacr.org/2017/1146); [slides](https://dimacs.rutgers.edu/archive/Workshops/Outsourcing/Slides/Zhang.pdf)
- **Where presented:** [University presentation 2017](http://dimacs.rutgers.edu/archive/Workshops/Outsourcing/Slides/Zhang.pdf)
- **Kind of statements:** Layered arithmetic circuits
- **Information theoretic (IT) system:** Linear IOP. It proposes the first framework to lift the IP protocol of GKR to a (zero-knowledge) argument through a polynomial commitment.
- **Cryptographic compiler:** Polynomial commitments
- **Complexity/efficiency:** Prover $O(C \log C)$; verifier $O(d \log C)$; proof size $O(d \log C)$; trusted setup with SRS of $O(C)$; non-interactive through Fiat-Shamir
- **Models and assumptions:** KoE and ROM
- **Relation to other schemes:** It is the first to combine the GKR protocol with a polynomial commitment.

**BibTex citation**

```bibtex
@inproceedings{zhang2017vsql,
    title={vSQL: Verifying arbitrary SQL queries over dynamic outsourced databases},
    author={Zhang, Yupeng and Genkin, Daniel and Katz, Jonathan and Papadopoulos, Dimitrios and Papamanthou, Charalampos},
    booktitle={2017 IEEE Symposium on Security and Privacy (SP)},
    pages={863--880},
    year={2017},
    organization={IEEE}
}
```


-----------------------
## <a id="Template"></a>Template description

We'd like each concrete scheme to provide succinct information about the following aspects:

- **Available resources:** 
- **Where presented:** 
- **Kind of statements:** 
- **Information theoretic (IT) system:** 
- **Cryptographic compiler:** 
- **Complexity/efficiency:** 
- **Models and assumptions:** 
- **Relation to other schemes:** [Follows which previous schemes? Has it been superseded?]

**BibTex citation**

```bibtex
insert bibtex entry
```

Please submit this information via the form: [https://forms.gle/NGm9xpUJBDyy6UFr6](https://forms.gle/NGm9xpUJBDyy6UFr6) or submit a pull request to the [resources GitHub repo](https://github.com/zkpstandard/docs).

The editors may make some editorial adjustments to the submitted content, to promote consistency. For comments
, please send an email to [editors@zkproof.org]().

