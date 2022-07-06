# Cryptography

## Encryption, Decryption & Hacking
- The Caesar Cipher is a simple substitution cipher which replaces each original letter with a different letter in the alphabet by shifting the alphabet by a certain amount.
- Example:
```
S	E	C	R	E	T
Y	K	I	X	K	Z
```
- ^ The letters above are just shifted by 6. 
- Caesar always used a shift of 3. So EHZDUH EUXWXV == BEWARE BRUTUS.
- Three main techniques to crack code: frequency analysis, known plaintext, and brute force.
- Frequency Analysis: analyze the frequency of the characters in the message. For example, e is the most used letter in English. 
- Known plantext: plaintext is ordinary readable text before being encrypted into ciphertext or after being decrypted.
- Brute force: guessing possible combinations of a targeted password until the correct password is discovered. There are only up to 25 possible shifts, so you can keep trying different shifts until you get a message that makes sense. 
- Definitions:
  1. Encryption: scrambling the data according to a secret key (in this case, the alphabet shift).
  2. Decryption: recovering the original data from scrambled data by using the secret key.
  3. Code cracking: uncovering the original data without knowing the secret, by using a variety of clever techniques.
  
## Ceasar Cipher
- The Ceasar Cipher is not really used anymore because it is not secure. Most people could easily crack it.
- Some Examples:
```
Plain:    ABCDEFGHIJKLMNOPQRSTUVWXYZ
Cipher:   XYZABCDEFGHIJKLMNOPQRSTUVW
-----------------------------------------------------
Plaintext:  THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG
Ciphertext: QEB NRFZH YOLTK CLU GRJMP LSBO QEB IXWV ALD
```
- The encryption can also be represented using modular arithmetic:
```
E_{n}(x)=(x+n)\mod {26}
```
- Decryption is performed similarly:
```
D_{n}(x)=(x-n)\mod {26}
```
- Two situations to consider for breaking Ceasar Cipher: 
  1. an attacker knows (or guesses) that some sort of simple substitution cipher has been used, but not specifically that it is a Caesar scheme.
  2. an attacker knows that a Caesar cipher is in use, but does not know the shift value.