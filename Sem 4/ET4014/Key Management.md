## Key Transport
---

## Key Agreement
---
Both parties generate a piece of the key, which guarantees that $K_{ab}$ is a fresh key.
$$K_{ab} = H(N_a||N_b)$$
## Key Distribution
---
Assume A initiates the request.
1. $A \rightarrow \text{KDC}: A, B, N_a$
2. $\text{KDC} \rightarrow A: \{K_{ab}, A, B, N_a\}K_a, \{K_{ab}, A, N_a\}K_b$
3. 

## Kerberos
---
Is based on the Needham-Schroeder, but has __4 steps__ instead of __5 steps__.
In Kerberos the thrusted third party is called the Kerberos Key Authentication Server.