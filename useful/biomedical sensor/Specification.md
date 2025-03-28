### basic performance specification of the sensors
- 线性度（*非线性误差* ）
	 $$ \varepsilon  = \varDelta max \space / \space Y_{FS} *100\% $$
	 传感器校准曲线与拟合直线的最大偏差 / 满量程
	 var = variant; FS = Full Scale
	 
- 灵敏度
	 $$K = \varDelta Y / \varDelta  X  \ \ \  (dy / dx \ \ for\ nonlinear\ sensor)$$
	  输出量变化量与delta input的比值
	 	 
- 迟滞
	$$ \delta _H  = \varDelta H_{max} / Y_{FS} *100\% $$
	 	 传感器的正向（输入量增大）和反向（输入量减少）特性不一致的extent
		 Numerically 正反行程间最大偏差/满量程

- 重复性
	
	在input按同一方向做 FS 多次变动后所得特性曲线不一致extent
	特性曲线一致，重复性好，误差小
	与迟滞现象有相同产生原因（？）


# 改进方法


[[误差]]


为了减小[[零漂]]和[[温漂]]对传感器性能的影响 --> 补偿技术
	ex: 温度补偿和零点补偿
	这些补偿技术通过使用校准和补偿电路
	能够抵消些温度变化和其他环境影响引起的漂移，提高传感器的稳定性和准确性


- 结构 、材料 、参数的合理选择
- 平均技术
	 对 output 求平均提高[[信噪比]]
	 对多次采样的数据平均以减少[[随机误差]]
- [[差动技术]]
