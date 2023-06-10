# Read Topics 18:

## The Caesar Cipher:

The basic principle of the Caesar Cipher involves substituting each letter in the plaintext (the original message) with a letter that is a fixed number of positions down the alphabet.

Historically, the Caesar Cipher was used as a substitution cipher by Julius Caesar to protect military communications. It provided a simple way to encode messages that could only be understood by those who knew the shift value.

## Symmetric V.S. Asymmetric encryption:

**Symetric:**

1- *Single Key:* Symmetric encryption uses a single shared secret key for both encryption and decryption.

2- *Efficiency:* Symmetric encryption is computationally efficient, making it ideal for encrypting large amounts of data.

3- *Secure Key Exchange:* The challenge lies in securely exchanging the secret key between the communicating parties.

**Asymetric:**

1- *Key Pair:* Asymmetric encryption uses a pair of keys—a public key and a private key.

2- *Encryption and Decryption:* The public key is used for encryption, while the private key is used for decryption.

3- *Secure Key Exchange:* Asymmetric encryption solves the key exchange problem by allowing anyone to encrypt using the public key, while only the owner possesses the private key to decrypt.

Asymmetric encryption is used to establish a secure channel for symmetric key exchange. For example, in protocols like Transport Layer Security (TLS), the server's public key is used to encrypt a shared secret key, which is then used for symmetric encryption throughout the session. This ensures confidentiality and secure communication between parties.

## 