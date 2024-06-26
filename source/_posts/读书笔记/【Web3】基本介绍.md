---
title: 【Web3】基本介绍
categories: Web3
tag: Web3
---

## 钱包

### 作用

用硬件或软件的方式，可以访问资金，与去中心化应用程序进行交互，充当无银行金融服务的网关、收集NFT、创建链上身份与社区，并提供比传统钱包更多的用途

### 组成条件

- 公钥：链接到自己可以发售和接收交易的地址
- 私钥：用于签署新交易并允许访问资金，必须保密
- 种子短语：用于生成多个私钥。作为根密钥，可以访问用户钱包中其他密钥和地址，也可以创建新的密钥

### 分类
#### 热钱包（软钱包）
可以存储、发送、接收和查看代币，所以比其他类型的钱包更加方便
- 托管地：可以访问互联网和加密货币网络的设备上
- 实用性：最高
- 安全性：容易收到黑客攻击，因为连接到网络了

#### 桌面钱包
会被作为应用程序下载到电脑上，在本地运行
被认为是可用的，最安全的热钱包类型
- 托管地：电脑

#### 网络钱包
允许通过浏览器界面进行交互和访问，无须在本地设备上下载或者安装任何内容
具有与桌面钱包完全相同的功能，使用相同的区块链和区块浏览器来搜索区块和交易
- 托管地：其他人的计算机或者服务器上

#### 手机钱包
与桌面钱包类似，只是托管地是手机
与桌面钱包相比，手机钱包的功能相对更简单一些

#### 冷钱包
无须连接到互联网，那么这就使得冷钱包是存储加密货币的更安全的替代方案，因为有物理介质可以离线存储密钥
- 安全性：抵抗黑客能力更强，对长期投资者来说很实用

#### 硬件钱包
使用随机生成器生成公钥和私钥的物理电子设备
最适合长期投资和存储使用，因为它们不太容易获得
- 主要用例：确保未分配的、用于持续使用的大笔资金的安全性
- 安全性：最安全的存储方案之一，因为能够在设备中保存公钥和私钥，而无须借助任何互联网连接。这样对加密货币的访问是处于离线状态

#### 纸钱包
由物理打印出的区块链地址和私钥组成，到纸上。这些信息会被打印成二维码，可以通过扫描二维码来汇款
- 托管地：纸
- 缺点；只能一次性发送全部余额，不能多次发送部分

#### 市面上主流钱包

> 以太坊钱包

- metamask

- trust Wallet

- argent

- imToken

> 其他生态

- phantom：Solana生态

- keplr：Cosmos生态

- polkadot：Polkadot生态

- tezos：Temple生态


## 助记词
由于私钥一般情况下，都非常冗长复杂，不适合记忆，为了方便使用，密码学家将其简化成了12或者24位不等的单词或者中文字符，简化之后的就被称为助记词

即：
- 助记词是密钥的另外一种形式

- 通过助记词可以获取相关的多个私钥，但是通过私钥无法获取助记词

## 区块链浏览器

### 定义

区块链浏览器是一种软件，它使用api和区块链节点从区块链中提取各种数据，然后使用数据库来排列搜索到的数据，并以可搜索的格式将数据呈现给用户

### 背景

区块链钱包可以提供不同类型的数据，但仅限于与钱包管理的密钥相关的数据。区块链浏览器用于查看与在给定区块链的所有钱包上执行的交易相关的数据。
特殊之处就是在于透明度，它允许用户检查智能合约地址的余额和支出，如当用户参数首次代币发行时。

### 作用

- 查看任何钱包地址的交易历史
能够审计任何钱包地址并提高区块链的透明度
- 查看接收和更改地址
可以查看交易接收地址、更改地址。将加密货币返回给支出者，以防输入值过多用于交易费用，提高了交易的透明度
- 查看当天最大的交易
- 查看内存池的状态
可以查看区块链上未确认的交易及其详细信息
- 查看双花交易
部门浏览器支持
- 查看孤立和陈旧区块
孤立区块：挖掘之后没有附加到最长的区块链上，并且它们的父区块链是未知的

陈旧区块：已知父区块链，但未链接到已知最长链的区块

- 查看发现或开采特点区块的个人或矿池

- 查看创世区块

- 允许用户查看交易费用、区块链难度、哈希率和其他数据

### 优势

- 将加密货币发送给某人之前会检查钱包地址是否对区块链有效

- 检查加密货币是否已经发送给目标个人。所有者可以检查他们的钱包余额

- 可以帮助解释尚未通过或确认的交易出现的问题以及查看确认jieduan

- 帮助用户了解交易或Gas当前的成本，从而帮助计划未来的Gas支出

- 帮助用户了解某个组是不是挖掘交易的人，并有助于决定是否为未来的挖掘活动投入更多的计算资源

- 可以帮助正在开发钱包的人，如果它可以进行正常的工作（发送、接收、存储和加密货币）

- 与其他软件一起使用，可以证实数据和信息

### 工作流程

- 资源管理器首先使用节点接口提取给定区块链中的所有数据，一旦它导出数据，就会将其存储在可搜索的表格中

- 将收集最新的交易和区块，根据定义的可搜索类别进行排列。它为用户提供了一个界面用于搜索。在技术方面，资源管理器可以使用关系数据库、sql数据库和api

每个区块链节点都可以直接读取区块链上的数据，获取最新交易和挖掘区块等数据等详细信息，然后将其发送到数据库，其中数据以可搜索表格的形式排列，使得资源管理器可以快速使用这些数据。

大部分的区块链使用表格，每一行都有唯一的id或者键用于区分

## 域名系统

在区块链中，域名系统和网络中的域名概念不同。区块链中，域名指向的是钱包地址，是一种身份的关联和映射，解决了ip或钱包地址过长的问题

### ENS域名系统

#### 含义

ens由两个以太坊智能合约组成：记录域名的ens注册表和将域名与机器的可读地址互相转换的解析器

#### 获取

在ens app上注册

### DAS域名账户系统

#### 含义

das是web3的去中心化身份认证系统，和ens类似，允许用户将个人域名绑定都适用所有链的人类可读地址。

## 预言机

预言机充当区块链上的app接口，通过查询可以获取智能合约的相关信息。预言机也可以向真实世界发送数据

### 背景
大多数区块链都有用于转移价值、启用协议操作或促进治理的本地加密货币，一些区块链支持智能合约，而智能合约可以在没有第三方的情况下执行，并且可以设计为执行几乎任何可以想象得到的合约。

区块链和链上智能合约需要一种方法来利用外部的链下数据，以便智能合约执行影响现实世界的app，因此预言机就需要被用到

### 分类

- 软件预言机

提供来自网站、服务器或数据库等数字源的数据。可以提供实时信息

- 硬件预言机

提供来自现实世界的数据，可以传递和中继来自项目运动传感器

- 集中式预言机

它由单个实体控制，并充当智能合约的唯一数据提供者。它要求合同参与者对一个实体给予极大的信任；它还代表单点故障，这可能会威胁到智能合约的安全性，如果预言机被破坏，智能合约也会被破坏。智能合约的准确性和有效性在很大程度上取决于所提供数据的质量，因此预言机对智能合约有很大的权利。

预言机问题：预言机可以使智能合约在去信任方之间执行，但当他变得过度中心化时，可能会有它试图成为中间人的风险。

- 去中心化预言机

去中心化预言机试图实现依赖因果关系而不是个人关系的去信任和确定性结果。它以与区块链网络相同的方式实现这些结果，在许多网络参与者之间分配信任。通过利用许多不同的数据源并实施不受单个实体控制的预言机系统，去中心化的预言机网络可能成为为智能合约提供更高级别的安全性和公平性。

### 实例

Chainlink

