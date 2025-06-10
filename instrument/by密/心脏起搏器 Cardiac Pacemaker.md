
- Sinoatrial (SA) node: The heart's natural pacemaker with spontaneous rhythm capability
	窦房结 自发节律
- Electrotherapy: Using external electricity sources to stimulate human tissue for therapeutic benefits


![[Pasted image 20250427144313.png]]
[[Pulse Generators 脉冲发生器]]

##### History
除颤

电容，莱顿瓶

1800 Volt

re-animation

1957 美敦力
myocardial wire 经皮穿到心外膜
however, 停电，患者成仙

1956 硅晶体管！！1958 植入式起搏器
无线充电
*导线抗疲劳性，抗腐蚀（人体高盐环境），漏电流*

Wilson Greatbatch
- 导线[[BC 生物相容性]]！！！
做ocsillerator时，拿错电阻，发现可以做成植入式的！封口！
1960 bow tie team

- 锂电池！！--电脉冲发放
从锌汞电池的置换反应（会产氧生锈，气泡也会影响发电效率）


后来：静脉导管就无需开胸了

Nuclear Pacemaker KO Battery Powered（but核难民用）


1980s:类固醇洗脱导线(减少炎症)
1990s:Microprocessor-driven pacemakers（实现复杂控制）


To sum up
医生+Double E

交叉学科：要某领域顶尖后才跨科涉猎

### Main
Review：[[心动周期 cardiac cycle]]

解决两种问题
1. 起搏，节律
2. 心房传导

分类：

By Electrode Configuration 根据起搏电极
- **Unipolar**: One electrode with ground reference
- **Bipolar**: Two electrodes placed in the heart


By Relationship to Cardiac Electrical Activity 
##### Asynchronous (Fixed-Rate) 非同步型(固定频率型)

- **仅用于心室起搏**
- Delivers stimulation pulses at fixed intervals regardless of heart's natural activity
- Primarily used for electrophysiological examinations
- Suitable for persistent third-degree atrioventricular block or overdrive pacing
	持久性三度房室传导阻滞
- Core component: Pulse generator


### Synchronous (Demand) 同步型

Used for **atrioventricular block and arrhythmias**
		适用于**房室传导阻滞、心律不齐**

##### Pacing 起搏
产生周期性的电流脉冲

1. 没有感知自身心搏信号
	自身心搏过缓，则起搏器发出一个起搏脉冲，随后即使心脏自身有搏动电信号，但由于心肌处于不应期而被抑制
2. 感知到自身心搏信号
	自身心搏较快，则起搏器的反应方式又有两种类型
	**触发型（备用型）**[[P波同步型]]VAT
	立即发出(触发)一个起搏脉冲，落于自身心搏的绝对不应期中，沦为无效放电脉冲，避免了易激期刺激
	由于总有刺激脉冲作为心脏起搏的备用信号，故又称为备用型
	Immediately delivers a pacing pulse after sensing natural heartbeat, falling within refractory period
	
	**抑制型（按需型）！！！**[[R波抑制型]] VVI
	取消(抑制)下一个预定脉冲发放避免了心搏竞争，并以感知的自身心搏开始重新一次起搏周期，又称为按需型
	Cancels scheduled pulse when natural heartbeat is detected, avoiding competition
	
	![[Pasted image 20250406231127.png]]

##### Sensing 感知
识别心脏内部自主电活动

##### Output inhibition 输出抑制
检测到自主电活动时，抑制起搏脉冲的释放


### Technical Components

导线 leads?!
![[Pasted image 20250406232340.png]]

分为主动固定式(螺旋结构)和被动固定式(翼状)，材料一般与电极相同，具有良好的导电性和生物相容性。
- 被动式：机械结构
- 主动式：机体响应包裹

- **Active fixation**: Helical structure, mechanically anchored
- **Passive fixation**: Wing-shaped, relies on tissue encapsulation


>[!FAQ]- lead??!!导联导线？？
>## How to Distinguish Them
The easiest way to distinguish these concepts:
 **ECG Lead (导联)**: A measurement concept or virtual pathway (not a physical object)
 **Pacemaker Lead (导线)**: A physical wire that actually touches the heart
>
In English medical terminology, unfortunately, the same word "lead" is used for both concepts, which can be confusing. The context usually clarifies which meaning is intended - when discussing ECG recordings, "lead" means 导联; when discussing pacemaker hardware, "lead" means 导线.

##### 电极

单极型:导管中只有一根导线，*采用金属外壳作为参考电极*
双极型:两个导线，分别连接刺激电极和参考电极


##### Furthermore

- Self-powering technology: Utilizing kinetic energy from heartbeats
- Symbiotic cardiac pacemakers 纳米发电机: Implementing nanogenerator technology