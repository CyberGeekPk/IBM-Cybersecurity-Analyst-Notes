# Security Best Practices

## Learning Objectives

- Explore password management best practices, password use policies, and password managers
- Explore authentication methods, permissions, access control, and accounting
- Evaluate methods used to secure and harden devices, contrast open vs secure WIFI, and demonstrate installation of software updates and patches
- Explore device use best practices, source safe software, contrast OEM websites vs third party websites, and demonstrate unwanted and malicious software removal
- Explore encryption types, and common encryption uses, and learn the difference between encrypting data at rest and data in motion
- Identify how to manage email and spam, and demonstrate email security best practices

## Encryption

Encryption is the act of taking readable text and scrambling it so it can only be read by a recipient that has the decryption key. Data that has not been encrypted is called plain text because it's readable. Algorithms used to scramble plain text are called ciphers. Encrypted plain text is called ciphertext. An encryption key is a series of random, unique numbers, combined with very powerful algorithms that are used to encrypt (or scramble) your data before you send it. The person on the receiving end has a decryption key that's used to decrypt (or unscramble) the data so it's in a readable or useable format. 

### Symmetric Encryption

Symmetric encryption, also called “single-key” or “private key” encryption, is when a single key is used between parties to encrypt and decrypt data. 
With only one key, symmetric encryption uses less memory, which is great for quickly and securely processing larger amounts of data. That’s why it is often used to protect the main data exchange in a session. But it’s harder to keep a single key secret, especially if it needs to be broadly distributed. If this key is intercepted by a hacker, then they can decrypt your messages, hack your account, and steal or tamper with your data. 
3DES and CAST are examples of symmetric encryption technologies.

### Asymmetric Encryption

Asymmetric encryption, also called “Public Key Cryptography”, uses a public key and a private key. Asymmetric encryption takes longer because it is more complex. It is used for smaller amounts of data. It is safe to widely share the public key for encryption or decryption, because only the secret key can undo the public key’s action. Uses include: authentication, digital certificates, digital signatures, and key exchange – where a symmetric encryption key is shared only to the intended recipients. The RSA cipher is used in most asymmetric encryption.

