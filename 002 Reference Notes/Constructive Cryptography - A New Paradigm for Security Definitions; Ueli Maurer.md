202502211925

Status: #reading

Tags: #book

# Constructive Cryptography - A New Paradigm for Security Definitions; Ueli Maurer

- Authors: [[Ueli Maurer]]
- Subject: [[Cryptographic Security Proofs]] [[Cryptography]]
- Date of publication: ???

# Synopsis

# Relevant Results

- Concept: [[Maurer's Constructive Cryptography]]
- Definition: Secure Construction of Cryptographic Protocols
- Theorem: [[Maurer's General Construction Composability Theorem]]

# Section Overviews

## Section 1 - *Introduction and Motivation*

Constructive disciplines focus of analyzing building blocks and composing those blocks into more complex structures. For this we need a notion of composition which preserves whatever we are studying/care about. (In the vein of [[Knowledge should accrete]] and [[Composability multiplies effectiveness]]). The stated goal of the paper is to apply this philosophy to [[Cryptography]].

Current (at the paper's SoA) definitions of [[Cryptographic Security]] work well for specific goals, but are insufficient because they fail to compose and specialize (in the sense that a stronger notion of security for a protocol should imply weaker notions of security for that same protocol in a more restricted setting).

The paper discusses a change in the security definitions based on [[Secure Construction of Cryptographic Protocols]] based on a notion of [[Computational Simulator]] and [[Cryptographic Real-World]] vs [[Cryptographic Ideal-World]].

## Section 2 - *Motivating Examples*

Presents the [[One-Time Pad]] and [[Additive Stream Cipher]] as motivating examples for the work (see [[Maurer's Constructive Cryptography]]), arguing that the [[Information Theoretical Security of a Cryptographic Protocol|information-theoretic security]] notion is insufficient as it fails to capture what we want out of the security of the OTP as well as failing to specialize in order to prove the security of the [[Computational Security of an Additive Stream Cipher|additive stream cipher]] under the assumption that stream comes from a [[Cryptographically Secure Pseudo-Random Generator]].



---
# References

- [[ConstructiveCryptography_Maurer.pdf|Constructive Cryptography; Ueli Maurer]] (https://crypto-test.ethz.ch/publications/files/Maurer11.pdf)