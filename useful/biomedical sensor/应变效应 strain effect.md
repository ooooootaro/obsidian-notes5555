### overall
导体或半导体材料在受到机械形变时
其电学特性(主要是电阻)发生变化的现象

应变效应包含两个主要组成部分：

1. **几何效应**：（金属，电阻率变化较小）
    - 当导体被拉伸时，长度增加而横截面积减小
    - 当导体被压缩时，长度减小而横截面积增加
    - 这些几何变化直接影响电阻值(R = ρ·l/S)
2. [[压阻效应 piezoresistive effect]]：（半导体，电阻率变化显著）
    - 材料的电阻率(ρ)在应变作用下发生变化
    - 由材料内部晶格结构和电子传导特性变化引起
    - 在半导体材料中尤为显著


公式
$$\frac{dR/R}{\varepsilon} = (1 + 2\mu) + \frac{d\rho/\rho}{\varepsilon} = 定义为K$$
这种效应使我们能够通过测量电阻变化来**间接测量应变**，
从而进一步推算应力、力、压力、位移等物理量，是许多传感器和测量系统的基础


### 推导
$$R = \rho \frac{l}{S}$$
- $\rho$ —— 电阻丝材料的电阻率 (Ω·mm²/m)
- $l$ —— 电阻丝长度 (m)
- $S$ —— 电阻丝截面积 (mm²)

微分分析
对上式两边取对数： $$\log R = \log \rho + \log l - \log S$$

再对等式两边微分，得： $$\frac{dR}{R} = \frac{d\rho}{\rho} + \frac{dl}{l} - \frac{dS}{S}$$

- $dR/R$ —— 电阻的相对变化
- $d\rho/\rho$ —— 电阻率的相对变化
- $dl/l$ —— 金属丝长度的相对变化
- $dS/S$ —— 截面积的相对变化


应变关系
设电阻丝的半径为$r$，则： $$\frac{dS}{S} = \frac{d(\pi r^2)}{\pi r^2} = \frac{2dr}{r}$$
令：

- $\frac{dl}{l} = \varepsilon_x$ 为金属丝的轴向应变
- $\frac{dr}{r} = \varepsilon_y$ 为径向应变

材料的轴向应变与径向应变的关系为： $$\varepsilon_y = -\mu\varepsilon_x$$
##### 其中$\mu$为金属材料的[[泊松比]]
代入前式，得： $$\frac{dR}{R} = (1 + 2\mu)\varepsilon_x + \frac{d\rho}{\rho}$$

进一步整理： $$\frac{dR/R}{\varepsilon} = (1 + 2\mu) + \frac{d\rho/\rho}{\varepsilon}$$




