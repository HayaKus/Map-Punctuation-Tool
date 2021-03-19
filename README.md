# <img src="https://github.com/HayaKus/CloudSimSEC/blob/master/graphs/logo/Logo.png" width="10%"/> 地图标点工具 Map Punctuation Tool 
![](https://img.shields.io/badge/release-v1.0-blue)
![](https://img.shields.io/badge/language-JSP%20%7C%20HTML-orange)
[![](https://img.shields.io/badge/platform-windows-orange)](https://www.microsoft.com/windows/)
[![](https://img.shields.io/badge/license-MIT-orange)](/LICENSE)

# 正在修改readme，请稍等


**如果您觉得软件对您有所帮助，点一下右上角的star并推荐给周围的朋友就是对我极大的支持。(●'◡'●)**

## Table of Contents 内容列表

- [Usage 使用说明](#usage-使用说明)
    - [1. the parameters of data center 数据中心的参数](#1-the-parameters-of-data-center-数据中心的参数)
    - [2. the parameters of physical hosts 物理主机的参数](#2-the-parameters-of-physical-hosts-物理主机的参数)
    - [3. the parameters of virtual machines 虚拟机的参数](#3-the-parameters-of-virtual-machines-虚拟机的参数)
    - [4. the parameters of cloud tasks 云任务的参数](#4-the-parameters-of-cloud-tasks-云任务的参数)
    - [5. the parameters of users 用户的参数](#5-the-parameters-of-users-用户的参数)
    - [6. other components 其他组件](#6-other-components-其他组件)
- [Maintainers 维护者](#maintainers-维护者)
- [Contributing 如何贡献](#contributing-如何贡献)
    - [Contributors 贡献者](#contributors-贡献者)
- [License 使用许可](#license-使用许可)

## 使用说明

步骤1：首先将execl文件处理成以下格式，并另存为“.xlsx”格式。

注意：第一行必须分别是longitude（经度）和latitude（维度）。

<div align=center><img src="https://github.com/HayaKus/Map-Punctuation-Tool/blob/main/graphs/step1.png" width="80%"/></div>



Install pack: After the software is installed, click the 'CloudSimSEC' file on the desktop to open the software.  
**安装包：安装完成之后，点击桌面的'CloudSimSEC'文件即可打开软件。**

Source code: Run '/PowerForecast/main/Main.java' through a compiler (e.g., [IDEA](http://www.jetbrains.com/idea/)) to open the software.  
**源代码：通过编译器（例如 [IDEA](http://www.jetbrains.com/idea/)）运行'/PowerForecast/main/Main.java'即可打开软件。**

<div align=center><img src="https://github.com/HayaKus/CloudSimSEC/blob/master/graphs/usage/CloudSimSEC%E9%A6%96%E9%A1%B5.png" width="80%"/></div>

The parameters that can be set in the cloud data centers are mainly divided into five parts, i.e.,  
**云数据中心里可以被设置的参数主要被分为五个部分，即**

### 1. the parameters of data center 数据中心的参数

- "数据中心名称" is the name of the data center.
- **"数据中心名称"是数据中心的名称。**
- "IT系统能耗模型" is the energy consumption model of the IT system in the cloud data center.
- **"IT系统能耗模型"是云数据中心中IT系统的能耗模型。**
- "IT维护系统能耗模型" is the energy consumption model of the system for maintaining IT system operation in the cloud data center.
- **"IT维护系统能耗模型"是云数据中心中用于维护IT系统正常运行的系统的能耗模型。**
- "IT维护系统最大功耗（W）" is the maximum power consumption of the system for maintaining IT system operation in the cloud data center.
- **"IT维护系统最大功耗（W）"是云数据中心中用于维护IT系统正常运行的系统的最大功耗。**
- "消防系统功耗（W）" is the power consumption of the fire fighting linkage control system in the cloud data center.
- **"消防系统功耗（W）"是云数据中心中消防系统的功耗。**
- "基础设施系统功耗（W）" is the power consumption of the infrastructure system in the cloud data center.
- **"基础设施系统功耗（W）"是云数据中心中基础设置系统的功耗。**
- "模拟间隔（s）" is the time interval of the simulator.
- **"模拟间隔（s）"是模拟器每次模拟的时间间隔。**

### 2. the parameters of physical hosts 物理主机的参数

- "主机+number" represents different types of physical hosts.
- **"主机+数字"代表了不同的物理主机种类。**
- "数量" is the number of each physical host.
- **"数量"是每种物理主机的数量。**
- "运算能力（MIPS）" is the computing power of each physical host.
- **"运算能力（MIPS）"是每种物理主机的运算能力。**
- "空闲功耗（W）" is the power consumption of each physical host during idle.
- **"空闲功耗（W）"是每台物理主机在空闲时的功耗。**
- "最大功耗（W）" is the maximum power consumption of each physical host.
- **"最大功耗（W）"是每台物理主机的最大功耗。**
- "内存（MB）" is the memory of each physical host.
- **"内存（MB）"是每台物理主机的内存。**
- "带宽（bit/s）" is the bandwidth of each physical host.
- **"带宽（bit/s）"是每台物理主机的带宽。**
- "存储（GB）" is the storage of each physical host.
- **"存储（GB）"是每台物理主机的存储。**

### 3. the parameters of virtual machines 虚拟机的参数

- "虚拟机+number" represents different types of virtual machines.
- **"虚拟机+数字"代表了不同的虚拟机种类。**
- "运算能力（MIPS）" is the computing power of each virtual machine.
- **"运算能力（MIPS）"是每种虚拟机的运算能力。**
- "内存（MB）" is the memory of each virtual machine.
- **"内存（MB）"是每台虚拟机的内存。**
- "带宽（bit/s）" is the bandwidth of each virtual machine.
- **"带宽（bit/s）"是每台虚拟机的带宽。**
- "存储（GB）" is the storage of each virtual machine.
- **"存储（GB）"是每台虚拟机的存储。**

### 4. the parameters of cloud tasks 云任务的参数

- "云任务+number" represents different types of cloud tasks.
- **"云任务+数字"代表了不同的云任务种类。**
- "云任务量（MI）" is the calculation of the cloud task.
- **"云任务量（MI）"是云任务的计算量。**
- "文件数量" is the number of files for the cloud task.
- **"文件数量"是云任务文件的数量。**
- "输出文件数量" is the number of output files for the cloud task.
- **"输出文件数量"是云任务输出文件的数量。**

### 5. the parameters of users 用户的参数

- "用户数量" is the number of person/people using this cloud data center.
- **"用户数量"是正在使用该云数据中心的人的数量。**
- "虚拟机+number" represents different types of virtual machines.
- **"虚拟机+数字"代表了不同的虚拟机种类。**
- "虚拟机数量" is the number of each virtual machine.
- **"数量"是每种虚拟机的数量。**
- "云任务种类（名称）" is the types of cloud tasks running on their virtual machine, which is set in the "云任务" part.
- **"云任务种类（名称）"是运行在虚拟机上云任务的种类，这可以在"云任务"部分设置。**

### 6. other components 其他组件

- The button "训练模型" records the method for modeling RBF neural networks using MATLAB.
- **"训练模型"按钮记录了使用MATLAB对数据进行RBF神经网络建模的方法。**
- The button "保存结果" helps users to store the simulation results in a local folder.
- **"保存结果"按钮帮助用户把模拟结果存放到本地文件夹中。**
- The button "帮助" records the author's [contact information](https://github.com/HayaKus).
- **"帮助"按钮记录了作者的[联系方式](https://github.com/HayaKus)。**
- The button "清空" clears all the default parameters in the simulator.
- **"清空"按钮会清空模拟器中所有默认的参数。**
- The button "重置" resets all parameters in the simulator to the default parameters.
- **"重置"按钮会将模拟器中所有的参数重置为默认参数。**
- The button "生成结果" collects all parameters and starts to simulate energy consumption.
- **"生成结果"按钮会收集所有的参数并开始模拟能耗。**

## Result 结果说明

The homepage will show the comparison of the energy consumption of the cloud data center without the scheduling algorithm and with RR algorithm, DVFS algorithm, SR algorithm. And some system information of simulation will be shown.  
**主页中会显示云数据中心在没有调度算法、只有RR算法、只有DVFS算法和只有SR算法的情况下的能耗对比情况和一些模拟出的系统信息。**

<div align=center><img src="https://github.com/HayaKus/CloudSimSEC/blob/master/graphs/result/CloudSimSEC%E6%80%BB%E8%83%BD%E8%80%97%E5%AF%B9%E6%AF%94.jpg" width="80%"/></div>

In addition, the average power and average utilization of all physical hosts in the above four cases will be shown.  
**并且，以上四种情况下所有物理主机的平均功率和平均利用率都会被显示。**

<div align=center><img src="https://github.com/HayaKus/CloudSimSEC/blob/master/graphs/result/CloudSimSEC%E6%B7%B7%E5%90%88%E5%AF%B9%E6%AF%94.jpg" width="80%"/></div>

Moreover, the average power and average utilization of every physical host in the above four cases will be shown.  
**此外，以上四种情况下每一台物理主机的平均功率和平均利用率都会被显示。**

<div align=center><img src="https://github.com/HayaKus/CloudSimSEC/blob/master/graphs/result/CloudSimSEC%E6%AF%8F%E5%8F%B0%E4%B8%BB%E6%9C%BA%E6%B7%B7%E5%90%88%E5%AF%B9%E6%AF%94.jpg" width="80%"/></div>

## Maintainers 维护者

<img src="https://github.com/HayaKus/CloudSimSEC/blob/master/graphs/logo/HayaKus.png" width="5%"/> [林皓伟](https://github.com/HayaKus)  

**Website: [twocups.cn](https://twocups.cn)**  

**Gmail：haya.haowei.lin@gmail.com**

**E-Mail: 296329404@qq.com**  


## Contributing 如何贡献

Feel free to dive in! [Open an issue](https://github.com/HayaKus/Map-Punctuation-Tool/issues/new) or submit PRs.  
**非常欢迎你的加入! [提一个Issue](https://github.com/HayaKus/Map-Punctuation-Tool/issues/new) 或者提交一个 Pull Request.**

### Contributors 贡献者

Thanks goes to these wonderful people:  
**感谢以下参与项目的人：**  

<img src="https://github.com/HayaKus/CloudSimSEC/blob/master/graphs/logo/HayaKus.png" width="5%"/> [林皓伟](https://github.com/HayaKus)  

## License 使用许可

[MIT](LICENSE) © 林皓伟