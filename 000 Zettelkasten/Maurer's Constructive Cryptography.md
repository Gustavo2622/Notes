202502211856

Status: #MOC
Tags: [[Cryptography]]

# Maurer's Constructive Cryptography

```ad-quote
 *Constructive cryptography* is a new paradigm in which the security definition
of cryptographic schemes is radically different. For example, a MAC is defined to be secure if it constructs an authenticated communication channel from an insecure communication channel and a secret key, for a well-defined, simulation-based notion of “construct” and for well-defined definitions of an insecure and an authenticated channel
```

This concept revolves around the idea of proving security through construction and showing that these constructions compose nicely. 
This is a consequence of [[Maurer's General Construction Composability Theorem]].

# Motivating Examples

## [[One-Time Pad]]

### Why is this relevant 

This protocol exhibits [[One-Time Pad is Information-Theoretically Secure|information-theoretic security]]. But the proof of this does not carry over to the practical setting where the secret key is generated from a short secret key by a [[Pseudo-Random Function]]. It would be desirable that stronger security guarantees always reduce to less strong ones when considered in a (more limited) practical setting ([[General Definitions should specialize]]).

Another problem with this notion of security is that we allow [[Cryptographic Message Malleability|malleability]] of the message.

A third potential problem is that ciphertext length leaks full information about message length. It could be argued that the proof (and so the "perfect" security intuition) only applies to messages of a fixed size and that in real use this limitation should be addresses, but it is probably better to include this limitation in what is actually being proven (and so, the definition of security in use).

This is the claim of Constructive Cryptography:

> [!important]
> Proofs ask for what they require and inform about what they deliver.

### How does this instantiate

What are the resources?
- Real Resources:
	- Authenticated Channel (AUT)
	- Secret Key (KEY)
- Ideal Resource:
	- Secure Channel (SEC)


## [[Additive Stream Cipher]]

In this case, since the keystream is fully derived from a short secret key, [[Information Theoretical Security of a Cryptographic Protocol|information-theoretic security]] is not a feasible proof goal. Therefore we must rely on a notion of [[Computational Security of a Cryptographic Protocol|computational security]]. 

The main goal for a security definition here is that the [[Computational Security of an Additive Stream Cipher|computational security of the protocol]] follows from the [[One-Time Pad is Information-Theoretically Secure|information-theoretic security of the OTP]] and the property that the [[Stream Cipher]] is a [[Cryptographically Secure Pseudo-Random Generator|CSPRNG]]. 

For this we need: 
- A computational version of "securely construct"
- A composition theorem allowing the composition of secure construction statements

# Main Definitions

- Ideal Resource
- Real Resource
- [[Computational Simulator]]
- Converters

# Main Theorems

---
# References

- [[Constructive Cryptography - A New Paradigm for Security Definitions; Ueli Maurer]] 