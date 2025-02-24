Is a mathematical scheme for demonstrating the authenticity of a digital message or document. 
DS use public keys because messages cannot be verified using shared keys. The signer uses their private key and the verifier checks is with the signer's public key.

The message is sent and alongside, an digest of the message encrypted with the sender's private key. The receiver uses the sender's public key to decrypt the digest and then checks if the messages are identical.

Digital signatures provide [[**authenticity**]] and **integrity**, but they do not provide message *confidentiality*.

## Digital Signature Algorithm - DSA
---
DSA uses the public/private key pairs created for use with the RSA algorithm to create and verify signatures. The DSA is for signing documents only and is not an encryption algorithm.

## Ensure Confidentiality
---
To provide confidentiality as well, the sender has to:
1. Encrypt using its own private key
2. Encrypt using receiver's public key

The receiver has to:
1. Decrypt using its own private key
2. Decrypt using sender's public key