# Assignment 1

* **Q1**

  (a)
  $$
  \begin{align}
  mean_{std}&=\sum_{i}^{n}x_ip_i\\&=20\times20\%+30\times50\%+50\times30\%\\&=34(M)\\mean_{h}&=\sum_{i}^{n}x_ip_i\\&=-20\times20\%+40\times50\%+90\times30\%\\&=43(M)
  \end{align}
  $$
  (b)
  $$
  \begin{align}
  V_s&=\sum_{i}^{n}(x_i-E[x])^2p_i\\&=(30-34)^2\times20\%+(30-34)^2\times50\%+(50-34)^2\times30\%\\&=124\\V_h&=\sum_{i}^{n}(x_i-E[x])^2p_i\\&=(-20-43)^2\times20\%+(40-43)^2\times50\%+(90-43)^2\times30\%\\&=1461
  \end{align}
  $$
  (c) It depends on how much risk can this company take. Choosing the way of horizontal drilling is expected to get more playoffs, but the variance of this approach also bigger than another one, which means the playoffs may not stable.

  (d) If the company intends to use the standard drilling, then they'd like to change to horizontal drilling with an 80%(30%+50%) probability after the geological evaluation:
  $$
  90\times30\%+40\times50\%-(50\times30\%+30\times+50\%)=17(M),
  $$
  so, the money pay for the evaluation no more than 17M makes sense.

  If the company intends to use the horizontal drilling, then they'd like to change to standard drilling with an 20% probability after the geological evaluation:
  $$
  (20-(-20))\times20\%=8(M),
  $$
  so, the money pay for the evaluation no more than 8M makes sense.

  

* **Q2**

  (a) Divided each frequency by 100 to get the probability as the table below.

  |            | YES  |  No  | Total |
  | :--------: | :--: | :--: | :---: |
  |  **Male**  | 19%  | 41%  |  60%  |
  | **Female** | 12%  | 28%  |  40%  |
  | **Total**  | 31%  | 69%  | 100%  |

  (b)
  $$
  P(X=smoker)=31\%
  $$
  (c)
  $$
  \begin{align}
  P(Y=female|X=smoker)&=\frac{P(Y=female,X=smoker)}{P(X=smoker)}\\&=\frac{12\%}{31\%}
  \end{align}
  $$
  (d)
  $$
  P(Y|X)=\frac{P(Y,X)}{P(X)}
  $$

  |                    | X=smoker | y=non-smoker |
  | :----------------: | :------: | :----------: |
  |  **P(X\|Y=male)**  |  31.67%  |    68.33%    |
  | **P(X\|Y=female)** |   30%    |     70%      |

  

* **Q3**

  (a)
  $$
  \begin{align}
  P(X=TA|Y=UF)&=\frac{P(X=TA,Y=UF)}{P(Y=UF)}\\&=\frac{P(Y=UF|X=TA)\times P(X=TA)}{P(Y=UF|X=TA)\times P(X=TA)+P(Y=UF|X=PM)\times P(X=PM)+P(Y=UF|X=PL)\times P(X=PL)}\\&=\frac{80\%\times15\%}{80\%\times15\%+10\%\times42.5\%+20\%\times42.5\%}\\&=\frac{12\%}{24.75\%}
  \end{align}
  $$
  (b)
  $$
  \begin{align}
  E&=\sum x \times p\\
  &=60\times P(Y=UF|X=TA)+80\times P(Y=UF,X=PM)+(-5)\times P(Y=UF,X=PM)\\
  &=60\times\frac{P(Y=UF,X=TA)}{P(Y=UF)}+80\times\frac{P(Y=UF,X=PM)}{P(Y=UF)}+(-5)\times\frac{P(Y=UF,X=PL)}{P(Y=UF)}\\&=35.35(K)
  \end{align}
  $$



* **Q4**

  (a) 
  $$
  \begin{align}
  P(X=5)&=(\frac12)^5\times(\frac12)^2\times C_7^5\\
  &=\frac{21}{128}
  \end{align}
  $$
  (b)
  $$
  \begin{align}
  P(X>=5)&=(\frac12)^7\times(C_7^5+C_7^6+C_7^7)\\&=\frac{29}{128}
  \end{align}
  $$
  

  (c) Since the function pbinom caculate the cumulative probability, we use 1-pbinom(19,28.0.5) to get Probability of get a total of 20 out of 28 correct.

  ![avatar](https://github.com/hoho-wenda0228/MS5721_ASSIGNMENT/raw/master/Assignment_1/3(c).jpg)

  (d)



* **Q5**

  (a)
  $$
  \begin{align}
  E[Y_1]&=E[0.25\times X_A+0.75\times X_B]\\&=0.25\times E[X_A]+0.75\times E[X_B]\\&=0.25\times3\%+0.75\times10\%\\&=0.825\%\\
  E[Y_2]&=E[0.5\times X_A+0.5\times X_c]\\&=0.5\times E[X_A]+0.5\times E[X_c]\\&=0.5\times3\%+0.5\times15\%\\&=9\%\\
  E[Y_3]&=E[0.5\times X_C+0.5\times X_B]\\&=0.5\times E[X_C]+0.5\times E[X_B]\\&=0.5\times15\%+0.5\times10\%\\&=12.5\%
  \end{align}
  $$
  (b)
  $$
  \begin{align}
  V_{Y_1}&=V(Y_1)\\&=V(0.25\times X_A+0.75\times X_B)\\&=0.25^2\times V(X_A)+0.75^2\times V(X_B)+2\times 0.5\times 0.75Cov(X_A,X_B)\\&=0.563125\%\\
  V_{Y_2}&=V(Y_2)\\&=V(0.5\times X_A+0.5\times X_C)\\&=0.5^2\times V(X_A)+0.5^2\times V(X_C)+2\times 0.5\times0.5Cov(X_A,X_C)\\&=1.0025\%\\
  V_{Y_3}&=V(Y_3)\\&=V(0.5\times X_C+0.5\times X_B)\\&=0.5^2\times V(X_C)+0.5^2\times V(X_B)+2\times 0.5\times0.5Cov(X_C,X_B)\\&=0.5^2\times (20\%)^2+0.5^2\times(10\%)^2+2\times 0.5^2Cor(X_C,X_B)Std(X)Std(Y)\\&=1.25\%+0.35\%\\&=1.6\%
  \end{align}
  $$
  (c) Since A, B, C are both normally distributed, the values within two standard deviation of the mean account for about 95% of the set.
  $$
  \begin{align}
  RangeY_1:E[Y_1]\pm2\sqrt{V_{Y_1}}&=0.825\%\pm2\times7.5\%\\RangeY_2:E[Y_2]\pm2\sqrt{V_{Y_2}}&=9\%\pm2\times10\%\\Range Y_3:E[Y_3]\pm2\sqrt{V_{Y_2}}&=12.5\%\pm2\times12.65\%
  \end{align}
  $$