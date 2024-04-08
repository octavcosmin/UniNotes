## Q2
---
$ssss0 = 4$

## Q3
---
$$\begin{split}
& Add(x, 0) = x & \text{Base case}\\
& Add(x, S_y) = S(Add(x, y))\quad & \text{Recurrence Relation}
\end{split}$$
## Q4
---
Prove that $n^2 \geq 2n + 3$ for $n \geq 3$.

>1. Base case: $n = 3$
>2. Assume inductive hypothesis: $n = k$
>3. Inductive step: Prove for $n = k + 1$

1. $$\begin{split}
n^2 &= 3^2 = 9 \\
2n + 3 &= 2 \times 3 + 3 = 9 \\
\text{so: } n^2 &\geq 2n + 3
\end{split}$$
2. Assume $k^2 \geq 2k + 3$
3. Prove for $n = k + 1$
$$\begin{split}
\text{Prove } &(k+1)^2 \geq 2 (k + 1) + 3 \\
&k^2 + 2k + 1 \geq 2k + 2 + 3 \\
\text{From (2) } &k^2 \geq 2k + 3 \\
\text{Prove } &2k+1 \geq 2 \Leftrightarrow 2k \geq 1 \text{ so true}
\end{split}$$
## Q5
---
Prove that $2^n \geq n^2$ for $n \geq 4$

>1. Base case: $n = 4$
>2. Assume inductive hypothesis: $n = k$
>3. Inductive step: $\text{Prove for } n = k + 1$

1. 
$$\begin{split}
\text{For } n = 4\text{: } & 2^n = 2^4 = 16 \\
& n^2 = 4^2 = 16 \\
\text{So: } & 16 \geq 16 \text{ means that } 2^n \geq n^2, \forall n \geq 4
\end{split}$$
2. Assume $2^k \geq k^2$
3.  Prove for $n = k + 1$
$$\begin{split}
\text{Prove: } & 2^{k+1} \geq (k+1)^2 \Leftrightarrow 2^k \times 2 \geq k^2 + 2k + 1 \\
\text{From (2): } & 2^k \geq k^2 \Leftrightarrow 2^k \times 2 \geq k^2 \times 2 \\
\text{Prove: } & k^2 \times 2 \geq k^2 + 2k + 1 \Leftrightarrow k^2 \geq 2k + 1 \Leftrightarrow k^2 - 2k + 1 \geq 2 \\
& \Leftrightarrow (k-1)^2 \geq 2 \\
\text{Because } k \geq 4\text{: } & (4-1)^2 \geq 2 \Leftrightarrow 9 \geq 2 \text{ so true}
\end{split}$$
