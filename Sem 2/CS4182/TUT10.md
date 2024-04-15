## 1.
---
Find an inductive definition for a function $sq$:
$$sq(n + 1) = sq(n) + 2*n + 1$$
1. Base case
2. Recursive definition
$$\begin{split}
(n+1)^2 &= n^2 + 1 + 2n \\
sq(n+1) &= sq(n) + 1 + 2n \\
sq(n) &= sq(n-1) + 1 + 2(n-1)
\end{split}$$
Base case: $n = 0$
Recursive definition: $sq(n) = sq(n-1) + 1 + 2(n-1)$
## 2.
---
```java
int sq(int n) {
	if (n == 0)
		return 0;
	else
		return sq(n-1) + 1 + 2*(n-1);
}
```
## 3.
---
```java
int sq(int n) {
	int retult = 0;
	for(int i = 0; i < n; ++i)
		result = result + 2*i + 1;
	return result;
}
```
## 4.
---
__Recursive:__

|      CALL<br>STACK      | RETURN<br>VALUES |
| :---------------------: | :--------------: |
|                         |                  |
|     sq(0): return 0     |        0         |
| sq(1): return sq(0) + 1 |        1         |
| sq(2): return sq(1) + 3 |        4         |
| sq(3): return sq(2) + 5 |        9         |
|       main: sq(3)       |       ---        |

__Iterative:__

|    CALL<br>STACK     | RETURN<br>VALUES |
| :------------------: | :--------------: |
|                      |                  |
| sq(3): return result |        9         |
|     main: sq(3)      |       ---        |
## 5.
---
Define strings of the form $a^mba^m$ recursively for $m \geq 0$. The letter $m$ represents how many times the letter is repeated.

Base case: All elements $\in$ PL
1. if $\lambda \in PL$ then $\lnot \lambda \in PL$
2. if $\lambda, B \in PL$ then $(\lambda \land B) \in PL$
3. if $\lambda, B \in PL$ then $(\lambda \lor B) \in PL$
4. if $\lambda, B \in PL$ then $(\lambda \Leftrightarrow B) \in PL$
5. if $\lambda, B \in PL$ then $(\lambda \Rightarrow B) \in PL$

Suppose $T$ is the set of strings.
Base case: $m = 0 \Rightarrow b \in T$
Use generating rule: $t \in T$ then $ata \in T$
$$T = \{b, aba, aabaa, aaabaaa, aaaabaaaa, ...\}$$

__Prove that all strings have an odd number of characters:__
Base case: $b \in T \rightarrow |b| = 1$, odd number
Assume $\gamma \in T \rightarrow |\gamma| = 1$, odd number
For a new string $a\gamma\\a \in T \rightarrow |a\gamma\\a| = |\gamma| + 2$, so $\text{odd number} + \text{even number} = \text{odd number}$
