
>1.
>>a. $S \times T = \{(w,m),(w,n),(w,o),(w,p),(x,m),(x,n),(x,o),(x,p),(y,m),(y,n),(y,o),(y,p),(z,m),(z,n),(z,o),(z,p)\}$
>
>>b. $\#(S \times T) = 4 \times 4 = 16$

>2. 
>> a. There are no pairs ($S \times T = \emptyset$)

>3.
>>a. $S \times T = \{(10,a),(10,b),(10,c),(11,a),(11,b),(11,c),(12,a),(12,b),(12,c),(13,a),(13,b),(13,c)\}$
>
>>b. $\#(S \times T) = 4 \times 3 = 12$
>
>>c. $m = \{(10,a), (11, c), (12, a), (13, b)\}$
>
>>d. $\#m = 4 = \#S$

>4.
>>a. $\begin{align} Programme \times YearOfStudy = \{&(BScCS,1),(BScCS,2),(BScCS,3),(BScCS,4),\\&(BScGD,1),(BScGD,2),(BScGD,3),(BScGD,4),\\&(HDipS,1),(HDipS,2),(HDipS,3),(HDipS,4),\\&(MScSE,1),(MScSE,2),(MScSE,3),(MScSE,4)\} \end{align}$
>
>>b. $\#(Programme \times YearOfStudy) = 4 \times 4 = 12$

>5.
>>a. $m:(Programme \times YearOfStudy) \rightarrow GradYear$ 
>
>>b. $\begin{align} m = \{&((BScCS,1),2027),((BScCS,2),2026),((BScCS,3),2025),((BScCS,4),2024),\\&((BScGD,1),2027),((BScGD,2),2026),((BScGD,3),2025),((BScGD,4),2024),\\&((HDipS,1),2027),((HDipS,2),2026),((HDipS,3),2025),((HDipS,4),2024),\\&((MScSE,1),2027),((MScSE,2),2026),((MScSE,3),2025),((MScSE,4),2024)\} \end{align}$
>
>>c. `public int calcGradYear(String course, int year){...}`
>>    $calcGradYear: (String \times int) \rightarrow int$
