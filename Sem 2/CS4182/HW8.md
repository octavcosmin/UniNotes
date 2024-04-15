| i   | result                           |
| --- | -------------------------------- |
| 1   | 1                                |
| 2   | 1 + 2 = 3                        |
| 3   | 1 + 2 + 6 = 9                    |
| 4   | 1 + 2 + 6 + 24 = 33              |
| 5   | 1 + 2 + 6 + 24 + 120 = 153       |
| 6   | 1 + 2 + 6 + 24 + 120 + 720 = 873 |
$$
\begin{gather*}
sum = \sum_{j=1}^i j! \land i \leq n \\
\{1 \leq n \land sum = \sum_{j=1}^i j! \land i \leq n\} sum = sum + f \{R\} \text{ (1)} \\
\{S\} i = i + 1 \{sum = \sum_{j=1}^i j! \land i \leq n\} \text{ (2)} \\
\end{gather*}
$$
$$\begin{split}
\text{(2) }Q^V_E:\ &(sum = \sum_{j = 1}^i j! \land i \leq n)_{i+1}^i \\
&(sum = \sum_{j = 1}^i+1 \land i + 1 \leq n)
\end{split}$$
We replace $R$ and $S$ with $Q^V_E$, then using the assignment rule: $$\begin{split}
Q^V_E:\ &(sum = \sum_{j = 1}^{i+1} j!)^{sum}_{sum + f} \\
& (sum + f = \sum_{j = 1}^{i+1} j! \land i + 1 \leq n)
\end{split}$$
$$\begin{gather*}
(sum = \sum_{j = 1}^{i + 1} j! \land i + 1 \leq n) && (sum + f = \sum_{j = 1}^{i + 1} j! \land i + 1 \leq n) \\
True & and & False & \rightarrow impossible
\end{gather*}$$
so the HT is correct.

---

```java
i = 0;
total = 0;
while(i < n) {
	i = i + 1;
	total = total + i;
}
```
$\{total = \sum_{j=0}^n j\}$

P and B C Q


