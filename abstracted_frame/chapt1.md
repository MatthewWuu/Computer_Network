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

概念：信道容量

​		ICMP 协议

​		TTL 生成时间

- 四类分组延时

  1. 节点处理延时 nodal proceeding
  2. 排队延时 queneing
     - 取决于intensity   [0,1]  公式 带宽 i=1的时候 延时无限大
  3. 传输延时 transmission
  4. 传播延时 propagation 有时距离短可以忽略不计

  

