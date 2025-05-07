##### 脉冲信号
Short-duration voltage or current signals

			![[Pasted image 20250405200330.png]]

Critical parameters: 
	power efficiency and compact size**功率！体积！**

# 心
起搏器脉冲(埋藏式)参数:
1. Pacing Rate 起搏频率
	最大心输出的心率，约60-90次/min，可调节，婴幼儿更高
	- Typically 60-90 pulses/minute (adjustable)
	- Higher rates for infants and young children
	- Optimized for maximum cardiac output
2. Amplitude and Width
	5 V ；0.3~1.5ms
	Parameters determine energy delivery and battery life
				![[Pasted image 20250405205623.png]]

### 原理

##### *Multivibrator* Oscillators 多谐振荡器
*多谐：非单一频率，可以产生方波*

more
- 产生方波
	使非门周期性地开通和关闭，即可在输出端得到矩形波
- 如何控制非门
	加入反馈，产生延迟与原信号相位相反
- 双暂稳态

##### Monostable Circuit 单稳态电路
调节脉冲参数

稳态：输出信号只能在一种状态(逻辑高或低)下是稳定的
	or稳定维持在某频率（？）

so制成扳+半稳态，以满足足够低的**q--占空比**

- Controls pulse parameters precisely
- Stable in only one state (high or low)
- Configured for very low duty cycle operation

##### Output Circuit 输出电路
射极输出，提高电流，**降低输出阻抗（确保有足够的能量在仪器上）**

more
复合管VT1，VT2
射极输出电路:电流放大，降低输出阻抗
C隔直流
DW:稳压管，限幅

- Emitter follower configuration
- **Key function**: Current amplification and reduced output impedance
- Ensures sufficient energy delivery to cardiac tissue
- Components include:
    - Composite transistors (VT1, VT2)
    - DC blocking capacitor
    - Zener diode for voltage limiting


### Pros n Cons

- **Limitation**: Fixed-rate pacing unrelated to natural heart rhythm
- **Risk**: Can create competing rhythms **竞争心律** leading to:
    - Ventricular fibrillation
    - Tachycardia
    - Reduced cardiac output
- lead to 心颤（射血不足？）or过速

The fundamental engineering challenges of pacemaker pulse generators revolve around reliability, power efficiency, precise timing control, and sufficient energy delivery while maintaining the smallest possible size.