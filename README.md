# AKMA and PE-AKMA ProVerif implementation

This project contains the code of ProVerif implementation of AKMA and PE-AKMA presented in [Privacy-Enhanced AKMA for Multi-Access Edge Computing Mobility](https://www.mdpi.com/2073-431X/12/1/2) by Gizem Akman, Mohamed Taoufiq Damir, Philip Ginzboorg, and Valtteri Niemi. 

## Objective

This project aims to implement formal verifications of 5G AKMA and PE-AKMA in ProVerif.

Authentication and Key Management for Applications (AKMA) is a service in the 5G system that supports authentication and security protection between the UE and applications [[1]](#1).

We propose a privacy-enhanced version of AKMA (PE-AKMA) that fixes the shortcomings of 5G AKMA.

## Content

We provide Formal Verification codes for the followings.

### src file:

**AKMA.pv** - 5G AKMA protocol

**AKMA_forwardsecrecy.pv** - 5G AKMA (only checks forward secrecy)

**AKMA_enhanced.pv** - PE-AKMA protocol

**AKMA_enhanced_forwardsecrecy.pv** - PE-AKMA protocol (only checks forward secrecy)

### out file:

The graphical representation of the attacks that ProVerif finds related to the queries.

## ProVerif

ProVerif is a state-of-art tool for formal verification for the symbolic modeling and analysis of security protocols. It uses Dolev-Yao as an adversary model. ProVerif uses the applied pi-calculus as a formal language, and translates the protocol into a set of Horn clauses, then tries to conclude if some security property is falsified, i.e., finds an attack.

For more information, [Proverif Manual](https://bblanche.gitlabpages.inria.fr/proverif/manual.pdf) is available online.

## Contact

Corresponding author is Gizem Akman. You can contact via gizem [dot] akman [at] helsinki [dot] fi.

## References

<a id="1">[1]</a>
3GPP TS 33.535 V17.6.0 (2022).
Authentication and Key Management for Applications (AKMA) based on 3GPP credentials in the 5G System (5GS).
Technical Specification.
# ProVerif-PE-AKMA
