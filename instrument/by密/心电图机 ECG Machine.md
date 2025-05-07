### History

心电图机的开发流程
	1901年：弦线式电流计，利用电流通过式产生的磁场使针偏移，需要非常细得银包裹石英丝
	1930s：电子管，晶体管式的心电图机
	1980s：数字式心电图机
![[equipment.png]]
特殊心电图：
- 动态心电图 (Holter监测心电图仪)：长时间连续记录
- 运动负荷心电图：透过一定量的运动增加心脏负荷进行评估
	对已知或怀疑患有心血管疾病，
	尤其是冠状动脉粥样硬化性心脏病（冠心病）进行临床评估
- 胸前体表标测（胸前多导）心电图
	等电位体表标测图（body surface maps）
- 穿戴式心电图

### 要点  

##### by徐学姐

完整理解：功能原理，简答题会出现用自己的话说

例如：心电、脑电导联、起搏器、除颤器同步非同步的区别

要记忆的书上的每个机器的基本功能

导联和电极的概念有什么区别

导联分为哪几大类，怎么设计中心电端，单极导联、双极导联是什么，有什么好处

心电12导联中哪些是双级的的哪些是单极的

生物电信号：基本定义、本质、检测过程中的基本要求是什么

# Design

[[心动周期 cardiac cycle]]

电极将心脏产生的电信号转化为电压信号
并通过仪器进行放大、滤波、采样、数字化等得到心电图
--- start-multi-column: ID_2247
```column-settings
Number of Columns: 3
Largest Column: standard
```

**难点**
- 信号弱$(10\mu{V}\sim5mV)$ 
- 频率低($0.05\sim 100Hz$)
$\qquad\to$干扰多
- 噪音强
- 随机性强
- 信号源阻抗高

--- column-break ---

**要求**
- 心电信号放大
- 抑制[[心电信号干扰]]
- 提高安全性(控制仪器风险等级)

--- column-break ---

**要点：**
- [[导联 leads]]
- [[生物电位放大器]]
- 滤波器[[50Hz陷波器]]
- 接地（解决共模干扰）
- 隔离 、屏蔽
	减少电场和磁场耦合的干扰

--- end-multi-column
如何测量胎儿心跳？
	腹部电极测量胎儿和母亲的心电信号
	[[反符合检测器]]以消除母亲QRS复波
	胸部电极测量母亲的心电信号。虽然腹部和胸部的心电信号幅度不同，但在同时出现信号时，将两者相减，得到胎儿的单独出现信号


**接地--公共接地**
所有仪器的接地应要先接一起，保证地是同一端
（避免又形成回路）

### 心电图机基本结构--滚瓜烂熟！

隔离与保护——信号检测——ADC——存储与显示![[Pasted image 20250303210258.png]]
![[Pasted image 20250309191901.png]]

- **Input (输入)** - The tiny electrical signals (0-5mV) captured from the body via electrodes
- **Preamplifier (前置放大)** - Initial amplification stage *with very high gain (80dB) to boost the weak signal*
	This stage needs extremely high input impedance and low noise characteristics to avoid distorting the tiny cardiac signals.
- **Amplifier/Adder (放大/加法器)** - Further amplification with reference to half supply voltage *(1/2 Vdd)*
	Further amplifies the signal and centers it around a reference voltage (1/2 Vdd), accounting for any DC offset in the signal. This ensures the signal remains within the operating range of subsequent stages.
- **Frequency Modulation (调频调制)** - Converts voltage to frequency (V-F) for transmission through isolation barrier
	This stage converts the voltage signal to a frequency-modulated signal. 
>[!FAQ]- Why V-F conversion?
>- **Noise immunity**: Frequency signals are more resistant to noise than voltage signals during transmission
>- **Isolation compatibility**: It's easier to pass frequency information across an isolation barrier
>- **Signal integrity**: Converting to frequency helps preserve signal information across the isolation barrier without analog degradation
>- **Safety**: This approach allows complete electrical isolation between patient and measurement circuits

- **Optical Isolation (光隔离)** - Creates electrical safety barrier between patient-connected circuitry and measurement electronics
	The frequency-modulated signal drives an LED, and a photodetector on the other side recreates the signal.
- **Demodulation (解调)** - Converts frequency back to voltage (F-V) after isolation
- **Amplifier/Subtractor (放大/减法器)** - Further signal conditioning
	*Conditions the demodulated signal, adjusting gain and removing any common-mode interference that may have been introduced.*
- **Low-pass Filter (滤波)** - *Removes high-frequency noise using RC circuit*
- **Output (输出)** - Provides the final clean ECG signal at a standardized voltage range (±5V) suitable for display or further processing.


放大（加法器）：由于二极管只接受正的驱动
	![[Pasted image 20250309205859.png]]

芯片：调制，Chip (芯片)/Modulation (调制)
	把缓慢变化的信号变高频

Optical Isolation 光电隔离（safety）
和12V电压共同加载到发光二极管

Demodulation Chip 解调芯片：
	变低频

减法器就是加法器的反向

最后再电容，[[RC电路]]低通滤波
low-pass filter stage which uses capacitors in an RC circuit configuration


![[Pasted image 20250309210607.png]]









