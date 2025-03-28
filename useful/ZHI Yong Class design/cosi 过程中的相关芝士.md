### English
required tool: Socket screw keys 凹头螺钉键

Slot nuts 狭槽的螺帽
countersunk 沉头的（countersink过去分词）
Linear bearing 直线轴承


###### step 8 
Ballscrew & spindle nut block 滚珠丝杆 & 主轴螺母座
Fixed bearing & motor holder 固定轴承（用于限制轴向和径向位移）& 电机座
Floating bearing 浮动轴承
Motor coupler 电机耦合器



## main
让我为您详细解释这三种开发板的特点和关系：

### 树莓派 (Raspberry Pi)
- 本质：一台小型计算机
- 主要特点：
  - 运行完整的操作系统（通常是[[Linux]]）
  - 有图形界面
  - 可以运行复杂程序
  - 适合多任务处理
- 主要用途：
  - 教育编程
  - 媒体中心
  - 网络服务器
  - 桌面计算
  - 复杂项目的大脑

### Arduino
- 本质：微控制器开发板
- 主要特点：
  - 简单的单片机系统
  - 实时响应快
  - 直接与硬件交互
  - 稳定可靠
- 主要用途：
  - 硬件控制
  - 传感器读取
  - LED控制
  - 电机驱动
  - 简单自动化项目

### BeagleBone Black (BBB)
- 本质：介于树莓派和Arduino之间
- 主要特点：
  - 运行Linux系统
  - 有实时处理单元
  - 工业级接口
  - 适合控制应用
- 主要用途：
  - 工业自动化
  - 精确控制
  - 实时数据处理
  - 嵌入式系统

### 三者对比

1. 处理能力：
- 树莓派 > BBB > Arduino

2. 实时性能：
- Arduino > BBB > 树莓派

3. 易用性：
- Arduino > 树莓派 > BBB

4. 价格（一般情况）：
- Arduino < BBB < 树莓派

### 适用场景

1. 树莓派适合：
- 需要图形界面的项目
- 需要处理复杂运算
- 需要网络功能
- 多任务处理

2. Arduino适合：
- 简单的控制项目
- LED控制
- 传感器读取
- 需要稳定性的场合

3. BBB适合：
- 工业控制
- 实时数据处理
- 精确运动控制
- 需要Linux但又要求实时性

### 组合使用

很多项目会组合使用这些设备，例如：
```
树莓派 -----> 负责界面和复杂运算
   |
   v
BBB/Arduino -> 负责硬件控制和实时响应
```

这样可以充分发挥各自优势，创建更强大的系统。选择哪种设备主要取决于您的具体需求和项目要求。