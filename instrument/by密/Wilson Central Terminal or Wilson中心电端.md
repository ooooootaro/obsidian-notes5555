- **Purpose**: Creates a stable reference voltage during the cardiac cycle
- **Implementation**:
    - Uses 5-300kΩ resistors to equalize resistance between limb electrodes and heart
    - Creates a common point by connecting these resistors
    - Voltage at this point equals the average voltage of the connected electrodes
- **Function**: Connected to the negative input of the amplifier to eliminate common-mode noise in unipolar leads

- 在心动周期内获得一个比较稳定的电压，作为体表上的基准值
- 串联5~300$k\Omega$使==三肢体端与心脏的电阻数值相互接近==
	因而把它们连接起来获得一个公共点，称为威尔逊中心电端
	它的电压是个电极上的电压平均值
- 作为参考点连接放大器的负端输入，消除单极导联的共模噪声，保持参考电压稳定
