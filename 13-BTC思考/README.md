# 13-BTC思考

### 哈希指针

指针只是保存本地计算机的地址，发送到其他计算机上面就没有意义（如何传输的呀）

所谓的哈希指针只是一种形象的说法，实际上只是哈希值，没有指针。

前获取一个指针的内容：(key, value) - levelDB

通过数据库中存储就可以实现哈希指针的功能。

### 区块恋

私钥一分两半，如果一部分没有了，就都没有了。

截断私钥的做法会降低私钥的安全性。

256 位的私钥，很难进行破解。

### 分布式共识

分布式系统中取得共识是不可能的。

比特币系统为什么能跳过分布式共识中的很多不可能？

共识一旦达成之后，就不用再修改了。比特币没有真正的跳过共识。

e.g. 如何判断远程连接的计算机是不是真的死机了？

不可能区分出来的（是死机还是连接缓慢）：异步的情况中不能判断。

**给服务器加一根电话线 - 用于拨号上网 - 进行连接**

- 不要被学术届限制了头脑
- 不要被程序限制了想象力

### 比特币的收益

- 降低成本
- 提高收益
  - 出块奖励
  - 挖矿难度

好的货币需要有一个通货膨胀的功能

### 量子计算

量子计算需要很长时间的发展，同时也会发展出来量子加密的方式。

比特币中并没有直接暴露公钥，而是取哈希之后得到的地址 - 非对称加密体系。

- 可以从私钥推导出公钥
- 不能从公钥推导出私钥
- 额外还有取哈希