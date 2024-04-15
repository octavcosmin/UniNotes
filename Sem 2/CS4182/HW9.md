## 1.
---
$$\begin{split}
S(0) &= 1 \\
S(S(0)) &= 2 \\
S(S(S(0))) &= 3 \\
S(S(S(S(0)))) &= 4 \\
S(S(S(S(S(0))))) &= 3
\end{split}$$
## 2.
---
$$sssssss0 = ssssss1 = sssss2 = ssss3 = sss4 = ss5 = s6 = 7$$
## 3.
---
$$\begin{split}
Mult(6,4) &= Mult(6, 3) + 6 = 18 + 6 = 24\\
Mult(6,3) &= Mult(6,2) + 6 = 12 + 6 = 18\\
Mult(6,2) &= Mult(6,1) + 6 = 6 + 6 = 12\\
Mult(6,1) &= Mult(6,0) + 6 = 0 + 6 = 6\\
Mult(6,0) &= 0 \nearrow
\end{split}$$
## 4.
---
$$\text{Base case}:
\begin{split}
n = 1: 1 + 2^1 &= 2^{1+1} - 1 \\
&= 2^2 - 1 \\
&= 4 - 1 \\
&= 3
\end{split}$$
We assume:
$$n = k: 1 + 2^1 + 2^2 + ... + 2^k = 2^{k+1} - 1$$
Determine the successor, adding $2^{k+1}$:
$$\begin{split}
1 + 2^1 + 2^2 + ... + 2^k &= 2^{k+1} - 1\quad |+2^{k+1}\\
1 + 2^1 + 2^2 + .. + 2^{k+1} &= 2^{k+1} - 1 + 2^{k+1}\\
&= 2^{k+1}(1+1) - 1\\
&= 2^{k+2} - 1
\end{split}$$
So, it is true for $n = k+1$, which means that it is true for all $n \geq 1$

