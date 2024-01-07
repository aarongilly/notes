---
created: 2023-07-23T21:47-05:00
updated: 2023-07-23T22:21-05:00
---
**The basis behind all sorts of awesome security stuff.**

Public key encryption is a form of asymmetric encryption (the key used to encrypt is different from the key used to decrypt) that is the basis for a LOT of modern security. It uses a pair of keys, one *public* and one *private*. Either key can be used to encrypt a message that can only be decrypted using the other half. It allows for secure encryption, authentication, and is the basis of RSA, amongst other stuff.

Public Key Encryption depends on [[Modular Arithmetic]], [[Primitive Root]]s, and a good [[One-Way Function]].

This uses the 'Diffie-Hellman' Key Exchange Algorithm, explained **very well** in the video in the source. The steps are outlined below.

1. `A` and `B` each have public and private keys.
	```
	A private key = 15
	B private key = 13
	```

2. `A` & `B` agree *publicly* to a Prime Modulus and a [[Primitive Root|Generator]]
	```
	A: "hey, lets do 3 mod 17"
	B: "cool"
	```

3. `A` raises their **private key** to the *generator*, and sends the result to B
	```
	A does => 3^15 mod 17 ≡ 6
	A: "Hey my public key is 6"
	B: "Dope"
	```

4. `B` does the same
	```
	B does => 3^13 mod 17 ≡ 10
	A: "Hey my public key is 12"
	B: "Sweet"
	```

5. `A` takes the **public key** from `B`, raises it to their own private key, and provides the modulus result to `B`. 
	```
	A does => 12^15 mod 17 ≡ 10
	A says "I know that our secret is 10"
	```

6. `B` does the same procedure with the **public key** from `A` and arrives at the same result. 
	```
	B does => 6^13 mod 17 ≡ 10
	B says "I know that our secret is 10"
	```

At this point, `A` and `B` know the shared secret, "10", but they do not know each other's *private key*. What's more - `C`, who was listening to all the *public information*, only has these things to work with:
	- 3 mod 17
	- A sent B "6"
	- B sent A "12"
Using *just* that info, for sufficiently large numbers, it's practically impossible to for `C` to determine secret number "10" now known to `A` & `B`. 

This has to do with the fact that `A` and `B` wound up doing the same [[Modular Arithmetic]], but they "went around the clock" an private number of times.

In reality this is done in conjunction with a pseudorandom generator to encrypt messages between people who've never met before.

---
### Source
- ![Stellar Key Exchange video](https://youtu.be/M-0qt6tdHzk)
- (Kahn Academy)[[](https://www.khanacademy.org/computing/computer-science/cryptography/modern-crypt/v/diffie-hellman-key-exchange-part-1)]

### Related
- [[One-Way Function]]
- [[Primitive Root]]
- [[Modular Arithmetic]]

#### Tags
#technique #math #coding #society 