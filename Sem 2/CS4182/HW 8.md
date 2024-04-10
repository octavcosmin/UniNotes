| i   | result                           |
| --- | -------------------------------- |
| 1   | 1                                |
| 2   | 1 + 2 = 3                        |
| 3   | 1 + 2 + 6 = 9                    |
| 4   | 1 + 2 + 6 + 24 = 33              |
| 5   | 1 + 2 + 6 + 24 + 120 = 153       |
| 6   | 1 + 2 + 6 + 24 + 120 + 720 = 873 |

$$\begin{split}
\{i \leq n \land sum = \sum_{j = i}^n j!\}
\end{split}$$
1. We prove that it is correct for $n = 1$
$$\begin{split}
\{n = 1 & \land i = 1 \land sum = 0 \land f = 1\} sum = 1 \{sum = \sum_{j = 1}^1 j!\} \Leftrightarrow \\
& \Leftrightarrow \{...\} sum = 1 \{sum = 1! = 1\} \text{, which is correct}
\end{split}$$
2. We assume that it is correct for $n = k$
3.  We prove that it is correct for $n = k + 1$
$$\begin{split}
\{n = k \land i = 1 \land sum = 0 \land f = 1\} ...\{sum = 1 + 1\times2 + 1\times2\times3 + 1\times2\times...\times k \} \Leftrightarrow \\
\end{split}$$