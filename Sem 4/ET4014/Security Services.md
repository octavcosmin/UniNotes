## Authentication
---

Authentication is the assurance that an entity is who it claims to be.

## Identification
---

### Needham-Schroeder Public-Key protocol
1. A sends S the public IDs for A and B.
2. S sends back B's public key and B's ID encrypted with S's private key.
3. A sens B a first random number (Na) and A's public ID, encrypted with B's public key.
4. B sends S the public IDs for B and A.
5. S sends back A's public key and A's ID encrypted with S's private key.
6. B sends back to A Na and another random number (Nb), encrypted using A's public key.
7. A sends back Nb encrypted with B's public key.
![[Pasted image 20250217114508.png]]

This is vulnerable to the **man-in-the-middle attack**. An intruder can force A to start a communication and then relay the messages between A and B, so that B believes they are communicating to A.
![[Pasted image 20250217114623.png]]