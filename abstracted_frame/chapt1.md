### 1.2 接入网

1. DSL 分成不同的速率 如上行和下行
2. 光线电缆 FTTH 



### 1.3 网络核心

- **分组交换中** 端到端对message 传输靠着packet switch 主要为：
  1. router
  2. link-layer switch

- store and forward transmission（储存转发传输）：需要switch完整接受到一份分组 才能开始传输

  ​    端到端一个分组的传输时延：

  ​                             **d=N*(L/R)** ,   where N为#linker N-1个swtich

  

- 排队和分组loss

   存在delay 原因是switch的缓存大小有限 可能会导致packet loss

​    	链路message到达switch的速度大于交换的速率 也会导致排队时延

- forwarding table和protocol

  ​	举不会用地图的司机在问路的例子 来类比ip address



- 电路交换（略）



#### 1.3.3 网络的网络

举例五层网络结构 循序渐进



### 1.4 分组交换网中的时延，丢包（packet loss）和吞吐量（througput）（视频）

![image-20230609174315548](/Users/wujunwei/Desktop/ustc-zheng-cn/image-20230609174315548.png)

#### ***<u>概念与补充</u>***

##### 信道容量

TraceRt测试：RTT round trip time 往返延迟

​		ICMP 协议 控制报文

​		TTL 生存时间 过一个路由器 ttl减一个 为零时候报告原主机

##### UDP TCP和以太网关系

> UDP 和 TCP 都是在以太网上工作的传输层协议，但它们提供不同的特性和功能。TCP 提供可靠性和流控制，适用于那些需要可靠传输的应用，而 UDP 则更适合对实时性要求较高且能容忍丢失一些数据的应用。

----



- 四类分组延时
  1. 节点处理延时 nodal proceeding
  2. 排队延时 queneing
     - 取决于intensity   [0,1]  *公式* 带宽 i=1的时候 延时无限大
  3. 传输延时 transmission
  4. 传播延时 propagation 有时距离短可以忽略不计

- 分组丢弃后怎么办？（缓存满了 也可能 ttl没了）
  1. 上路重新传
  2. 主机重新传
  3. udp（以太网 不可靠）--> 丢了就没了

- 吞吐量 throughput

  瓶颈取决于最小

  

  经过多跳

  

### 1.5 协议层次和分层模型

#### <u>*概念*</u>

大问题--->小问题

模块化 分层思想

PDU 协议数据单元 

---

 









