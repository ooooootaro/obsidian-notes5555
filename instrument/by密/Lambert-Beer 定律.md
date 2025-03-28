当入射光透射过某种均匀、无散射溶液时，其光吸收特性遵从Lambert-Beer定律


透光率
$$T = \frac{I}{I_0} = 10^{-\alpha cl} $$
	α：吸收系数
	c：浓度
	l： 穿透长度
	

为了线性--吸光度$$ A = -\lg \frac{I}{I_0} = -\lg T = \alpha cl$$
				


血液颜色
						![[Pasted image 20250319152648.png]]
由于是混合物， 等效的吸光系数是  $\alpha = \alpha_O \cdot SaO_2 + \alpha_H \cdot (1 - SaO_2)$

> 推导
> 用两种波长照射 得两个方程
> ![[Pasted image 20250319155959.png]]


$$ 
\begin{aligned}
SaO_2 = \frac{a_2 Q - b_2}{(a_2 - a_1)Q - (b_2 - b_1)} \\

\\

当波长\quad \lambda_1 (\sim 805nm) \quad
a_2 = a_1 = a \\

\\

SaO_2 = \frac{a}{b_1 - b_2} Q + \frac{b_2}{b_2 - b_1} = kQ + d 
\end{aligned}
$$

为了线性，第一个波长选择吸光度相同的波长


其实检测的是 SaO2（X），输出的是吸光度 Q（Y)
为了灵敏度公式里的 k 越小越好  $\Rightarrow$ 第二个波段取差值大的部分（比如  650 nm）
