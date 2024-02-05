## GMP需要仿真的各外设及功能

![image-20240205153336958](C:\Users\24583\AppData\Roaming\Typora\typora-user-images\image-20240205153336958.png)

#### FT2000A/2

* 功能：双核分别运行不同的软件，核1是图像处理，核0是应用软件，核间通信Mipc是天脉1的API，也需要运行天脉1；

#### RGMII

* 连接交换机

#### 网卡

* 功能：外连交换机(JEM5396)，接收来自维护数据设备(MDE)/防护型综合记录器(ISR)上的数据将其转发到便携式维修辅助设备(PMA);解析1394B上的数据包，按照以太网的协议格式发送给PMA

#### PCIE

* 功能：连接FPGA

#### FPGA(JFM7K325T-AS)上海复旦微电子---对标Xilinx(XC7K325T)

![image-20240205145637448](C:\Users\24583\AppData\Roaming\Typora\typora-user-images\image-20240205145637448.png)

* 功能：将cpu1的画面数据进行时序重建生成LVDS信号(新版的需要生成一路DVI信号)

#### LB(Local BUS)

* 连接NDB子卡

#### NDB子卡

* 通过1394总线连接外围设备

#### RS232

* 与显示器进行数据交换，控制显示器的亮度等

#### RS485

* 与外界进行数据交换

#### RS422 

* 新版GMP取消了此接口，作用是与ICP进行数据通信

#### CPLD

* 与看门狗和一些逻辑器件连接，负责控制复位等功能

#### 看门狗

* 监控CPU状态，设置周期喂狗(500ms)

#### FLASH(深圳国微)SM29GL512M

#### RAM(深圳国微)SM41J256M16M

#### NVRAM(深圳国微)SM14CA8-NF45

