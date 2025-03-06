# 比特币 Runes 深度解析：创建、交易与存储全指南

**关键词：** 比特币、Runes、代币、UTXO、铸币、转账、存储

本文详细介绍了比特币 Runes 协议的工作原理、创建流程及其在比特币生态系统中的应用，帮助您更好地了解如何购买、出售和存储 Runes 代币。

---

## 什么是 Runes 代币？

Runes 是一种基于比特币区块链的可替代性代币创建协议，通过比特币的 UTXO 模型简化代币的创建和管理流程。铸造 Runes 的用户已经支付了约 $4.95 百万美元的手续费来获取最独特的代币，这表明 Runes 协议有望大幅推动比特币手续费经济的发展。

本文将带您深入了解 BTC Runes 代币及其在比特币生态中的使用方式。

---

![Runes Protocol](https://www.jmhbdh.com/wp-content/img/904454735154.webp)

---

## 比特币 Runes 的工作原理

Runes 协议依托以下几个核心组件来实现其功能：

### 1. UTXO 模型

- **UTXO 基础系统：**  
  利用比特币中未花费交易输出 (UTXO) 的基本原理，每一笔未使用的比特币均被记录在区块链上。  
- **代币交易管理：**  
  Runes 协议正是基于此模型来记录代币交易，确保交易的准确性并防止重复使用。

### 2. 铸造蓝图（Etching）

- **定义代币属性：**  
  在铸造过程中，设定代币的名称、符号、小数位和发行上限等基本特性，类似于为代币绘制蓝图。  
- **功能确认：**  
  这一环节确保代币在区块链上能够被正确识别和使用。

### 3. 铸币（Minting）

- **开放铸币机制：**  
  根据铸造蓝图的规则，系统开放给所有参与者进行代币铸造，使得生态更为去中心化。  
- **参与性增强：**  
  广泛的参与和流通为代币生态带来更多活力。

### 4. 代币转账

- **指令操作：**  
  代币的发送与接收通过协议内的特定指令（Edicts）来实现，确保每一笔转账的完整记录。  
- **确保完整性：**  
  这种方法使得交易过程透明且可追溯。

### 5. 利用 OP_RETURN

- **数据嵌入：**  
  Runes 利用比特币中的 OP_RETURN 特性，将代币相关数据安全地嵌入交易中，而不会干扰主要交易数据。  
- **高效运作：**  
  此机制确保数据记录高效而整洁。

---

## 🚀 与 OKX 一起开启您的加密货币之旅！

零手续费交易，使用最先进的 Web3 功能，加入数百万全球交易者的行列。新用户可获得高达 100 USDT 的独家欢迎奖金！今天就与世界领先的数字资产平台一起开始您的交易冒险吧。

👉 OKX 新人限时优惠，最高可领取 100 USDT 奖励 ： [OKX活动页面](https://bit.ly/OKXe) | [国内镜像地址（免翻墙）](https://bit.ly/okX)

---

## 谁创建了比特币 Runes 协议？

Casey Rodarmor（Ordinals 项目开发者）推出了比特币 Runes 协议。他在比特币生态中不断探索创新使用方式，旨在解决以往比特币代币系统中的效率和使用问题。通过与 Ordinals 类似的理念，Rodarmor 希望提升比特币在代币管理方面的功能与效率。

![Casey Rodarmor](https://www.jmhbdh.com/wp-content/img/9777375305002626.webp)

Rodarmor 的工作不仅为比特币带来新的代币化思路，还在一定程度上优化了早期系统在效率和安全性上的不足。

---

## Runes 代币解决的问题

比特币 Runes 的设计初衷是针对比特币代币系统中的种种不足，主要体现在以下方面：

### 主要目的

1. **简化代币应用：**  
   相较于以太坊专为支持复杂合约设计的 ERC-20 和 ERC-721，Runes 允许在比特币网络内直接创建和管理可互换的代币，解决了历史上比特币在多代币处理上的不足。

2. **利用原生比特币功能：**  
   借助比特币内置的安全性和功能，Runes 在无需大幅改动核心协议的情况下实现了代币化功能。

### 待解决问题

- **UTXO 膨胀导致的拥堵：**  
  早期的代币化尝试常因产生大量无用 UTXO 导致区块链臃肿，从而拖慢交易处理速度并增加费用。  
  Runes 通过优化 UTXO 的管理，有效提高了网络效率。

- **系统复杂性与易用性：**  
  传统的比特币代币系统往往依赖链外数据，增加了使用复杂度，Runes 则通过全链上操作大幅提升用户体验。

- **规则的不明确：**  
  在 Runes 出现前，比特币缺乏类似 ERC-20 的代币创建标准，Runes 引入了一整套创建和管理规则，方便开发者和用户操作。

- **安全隐患：**  
  严格遵循比特币原始的设置及安全措施，使得 Runes 在设计上充分保障了交易安全性。

![UTXO 管理](https://www.jmhbdh.com/wp-content/img/1670657129156885.webp)

---

## 比较：BRC-20 与比特币 Runes

下面对 BRC-20 与比特币 Runes 在数据存储、转账机制以及扩展性方面的主要差异进行对比：

### 数据存储方式

- **BRC-20：**
  - **基于账户模型：** 每个代币与特定比特币地址关联。  
  - **公开透明：** 所有代币交易均记录在区块链上，可能引发隐私方面的担忧。

- **比特币 Runes：**
  - **基于 UTXO 模型：** 代币以 satoshi 的形式管理，并将相关信息嵌入 UTXO 中。  
  - **数据封装：** 相关信息更隐蔽，降低了直接暴露的风险。

### 转账机制

- **BRC-20：**
  - **直接地址转账：** 类似于常规加密货币转账操作。  
  - **依赖外部处理：** 需要额外系统支持管理转账操作。

- **比特币 Runes：**
  - **UTXO 操作：** 代币转账直接涉及 UTXO 的所有权变更。  
  - **原生区块链操作：** 利用比特币现有交易功能，无需额外层级支持。

### 扩展性与性能

- **BRC-20：**
  - **网络负载：** 大量 UTXO 可能导致区块链膨胀，从而增加费用并降低性能。  
  - **缺乏 Layer-2 支持：** 不与诸如 Lightning Network 的扩容方案直接兼容。

- **比特币 Runes：**
  - **高效优化：** 通过严格管理 UTXO 空间，降低了对区块链性能的负面影响。  
  - **兼容 Lightning Network：** 提升扩展性和交易速度，适用于高频交易场景。

![模型对比](https://www.jmhbdh.com/wp-content/img/5966019607862.webp)

---

## 如何购买与出售 Runes

比特币 Runes 的交易需要特定工具和要求，以下是简明指南：

### 步骤 1：获取兼容的钱包

由于 Runes 运行于比特币网络，需使用支持该代币的钱包。当前常用的钱包包括 Xverse、Leather 等。

### 步骤 2：购买比特币

为进行 Runes 交易，确保钱包中有足够的比特币以支付代币购买及相关手续费。

### 步骤 3：进入交易平台

可选择 ALEX DeFi 平台或 Magic Eden 平台进行交易，平台提供去中心化交易环境，用户可通过自动做市商系统（AMM）直接进行代币交换。

![交易平台](https://www.jmhbdh.com/wp-content/img/93821993748.webp)

### 步骤 4：交易操作

- **购买 Runes：** 利用平台 AMM 系统，用比特币或其他加密货币交换 Runes。  
- **出售 Runes：** 将手中持有的 Runes 上架出售，根据预设数量和价格完成交易。

---

## 如何发送、接收与存储 Runes

运行于比特币区块链上的 Runes 有其特定的操作方式，了解这些细节对于安全操作至关重要。

### 接收 Runes

- 打开钱包并进入接收界面，复制您的比特币地址（建议使用 Taproot 地址，以 "bc1p" 开头）。  
- 确认钱包支持 Runes 功能。

### 发送 Runes

- 在钱包中选择发送功能，输入对方的比特币地址，并核实地址的正确性。  
- 输入发送数量，注意转账手续费以比特币计付。  
- 确认后发起交易，确保按照网络要求支付足额手续费。

### 存储 Runes

- **硬件钱包：** 提供最强安全性，离线存储私钥。  
- **软件钱包：** 选择经常更新且支持 Runes 功能的钱包，确保流通与安全。

---

## 2024 热门 Runes 代币排行榜

以下为 2024 年交易量前五的比特币 Runes 代币概况：

### 1. SATOSHI•NAKAMOTO

![SATOSHI•NAKAMOTO](https://cdn.prod.website-files.com/6544a962cca0bd7efafca956/6644bd1ae4ab9b3e61933386_40AUGEg63vdwfvQoM0w7lEcZ7x9u2vmd0EMsfJOW_5coHS_TDaqv6X7zHUMETnI7-ASiNeTyz-4C0wW-y8-jtyjrL6ye0V4Lcn5z0Zjia8gINWLkXDUf9lnok-78axsctYuTYppDmXVkdNcxBWVgBEk)

SATOSHI•NAKAMOTO 已铸造 2000 多万代币，现流通量为 20,999,700 个。持有者众多，其中最大持仓者占比约 20%，其余持仓较分散。

### 2. RSIC•GENESIS•RUNE

![RSIC•GENESIS•RUNE](https://cdn.prod.website-files.com/6544a962cca0bd7efafca956/6644bd1ab18395446f25accc_H96lPUOKcZGjV4UblOmKdyeOO7c3KvWtU9k2vWD6gxO4m_u4ospFHj4t2Ia4t14dWlDnHQ6oowUZHJWLxAI0UDesA5kEc7eFKKJwz8Q91m4icwfQIv6kKW1MFnyPRuvdNjBldEbzGR0nz8D6mhFecns)

RSIC•GENESIS•RUNE 的总铸造量为 210 亿个代币，持有者超过 21800 人，代币流通极为活跃，总转账量达到 137.5 亿个。

### 3. WANKO•MANKO•RUNES

![WANKO•MANKO•RUNES](https://cdn.prod.website-files.com/6544a962cca0bd7efafca956/6644bd1a6686b43ff78fca49_5haZKhZEwCZV1A-Z9XfbP9mW0mTPo1DcWGy7VcKkzU0TBpC-094oOD8XDh0Y2XcJKkYmxHwUqI0EDz_ZIXpF-IXp6k8o1O75JvU1_aNqzjAnB9zBXGlz3HLo9idrOVBNeEaaAbYKdaB64U9QoRhSOrc)

总供应量为 10 亿个代币中，目前已铸造超过 7500 万个，约占总体 7.52%。在 2500 多持有者中，最大持仓者占比 3.38%，显示出较为均衡的分布。

### 4. Z•Z•Z•Z•Z•FEHU•Z•Z•Z•Z•Z

![Z•Z•Z•Z•Z•FEHU•Z•Z•Z•Z•Z](https://cdn.prod.website-files.com/6544a962cca0bd7efafca956/6644bd1a4975b0b36a826cb8_i1Jr6u2knMLSM5OzYCmatliVTrHMGsYjXnpRHk_vVkXSPzSJ9HE_IZbbeeLGUZuDHGnrasRMxmSAOxtB9E5BDpY3ZQuGIlJAuZuVWUcoOis-ktc8SkNTGjDOxlG5PFMVj438m3JC3JduiK-BcqsbLg8)

该代币总量为 111.1 万个，流通量已接近最大供应量，持有者超过 20900。此代币可能是首个出现的 Runes 代币，并有望在未来发挥重要作用。

### 5. BITCOIN•PEPE•MATRIX

![BITCOIN•PEPE•MATRIX](https://cdn.prod.website-files.com/6544a962cca0bd7efafca956/6644bd1a540917f965b9455b_HaZd_DWtOqXPeR6GG4lP_JsfCWsUs0zV7LEkyehKHQK5cSqfsss7nla8h950XKDwo94KQh4r_mNyaoYrsLby-D7pfvq3Qk4PMJlxYr0OLCUlyvu91Jxh2FlnuVu3ylvfVg1a4NFrYBPKFPzwbe6Kv1k)

BITCOIN•PEPE•MATRIX 完全铸造了 69 亿个代币，持有者达 16600+，体现出活跃的交易生态。

---

本文介绍了比特币 Runes 协议的基本概念、运作机制及交易方法，同时对市面上热门的几大代币进行了对比分析。通过优化 UTXO 管理、明确代币规则和原生链上操作，Runes 为比特币带来了高效且安全的代币管理新方式，使其在数字资产世界中拥有更广阔的应用前景。