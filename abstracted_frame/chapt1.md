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



### 1.4 网络的网络

举例五层网络结构 循序渐进



