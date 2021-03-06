---
title: 常见问题
description: 
published: true
date: 2020-11-14T06:56:55.893Z
tags: 
editor: markdown
dateCreated: 2020-09-06T08:00:45.742Z
---

# 常见问题

- Q1. FARM 代币的总量是多少？
- A1. FARM 代币总量最大值为 690,420，目前流通量为302,466.823。代币通过4年非线性释放，每周释放量会根据市场进行调节。

- Q2 . 现在我可以在哪里可以交易 FARM 代币？
- A2 . 目前你可以在 Uniswap 上的 FARM-USDC 交易对获取 FARM，你也可以在 Hotbit.io 买到 FARM，目前已经开通了 FARM/ETH 和 FARM/ USDT 交易对。

- Q3 . 那我要怎么用稳定币转成可赚取 FARM 收益的`f-稳定币`呢？
- A3 . 你可以在 [Harvest](https://harvest.finance/) 的首页上进行该项操作。

- Q4 . 要怎么才能把如何将 `f-稳定币`换回常规的稳定币？
- A4 . 请查看我们的提款说明页面

- Q5 . 只是持有 FARM 代币是否就可以获得 Harvest 的收益？
- A5 . 不是的，**你必须把 FARM Stake 在 [利润分享池](https://harvest.finance/earn) 中，以赚取农业收益**

- Q6 . 加入利润分享池子可以分享多少收益性利润收入？
- A6 . **30%的首页挖矿利润** 。支付的时候会使用7天移动平均收益值，不过收益农业的收入取决于可用收益农业机会的获利能力以及 Harvest 可用于农业的总资产。

- Q7 . 那剩下的 70％ 的耕作农业收入利润怎么分配呢？
- A7 . **会用来支付给将资产存入 Harvest 进行耕种的用户**。同时随着时间增加，Harvest 的 f稳定币代币的持有者（如fDAI，fUSDC和fUSDT）在赎回的时候也将获得更多的基础稳定币。


# 技术相关资料

-Q 1. 代码是开源的吗？
-A 1. [智能合约](https://github.com/harvest-finance/harvest) 是开源的；**为了防止被人抄袭，我们的前端用户界面没有开源**。

-Q 2. 为什么存入和提取稳定币的费用如此之高？
-A 2. 因为在某些情况下，**[提款必须从收益中的耕种策略中赎回稳定币](/ stakedrop＃从农业中删除代币) ** ;可以等网络没那么拥堵的时候，再来进行赎回，能够有效的降低网络交易费。

-Q 3. 我想看你们是怎么将农业收益利润收入的 5% 支付给 FARM 的质押者的。
-A 3. [一个收益农作交易的范例](https://etherscan.io/tx/0xabd90485e1c558a25b1f8a7f04f338bc5d32151aaa72a2468b739dcf5442d07e)。 [在利润分享合约中的 DAI 流入和流出交易](https://etherscan.io/token/0x6b175474e89094c44da98b954eedeac495271d0f?a=0xae024f29c26d6f71ec71658b1980189956b0546d)。

-Q 4. 我想看看存在 Harvest 的资金是怎么用于收益农业的。
-A 4. 很会就会出相关内容

-Q 5. 我想知道通过收获农作，Harvest fStablecoins 的价值是怎么正在变化的？
-A 5. 查看 [fDAI](https://etherscan.io/address/0xe85c8581e60d7cd32bbfd86303d2a4fa6a951dac#readContract)，[fUSDC](https://etherscan.io/address/0xc3f7ffb5d5869b3ade9448d094d81b0521e8326f#readContract)或[fUSDT](https://etherscan.io/address/0xc7ee21406bb581e741fbb8b21f213188433d9f2f#readContract) **合约**。从 f-稳定币 转换为稳定币的值是`getPricePerFullShare`。它与基础稳定币具有相同的小数位数，并且如果收益性耕种有利可图，它将随着时间的推移而增加。

-Q 6. 现在有策略时间锁吗？
-A 6. 目前的策略都有12小时的时间锁，意味着每次调整新的策略，都需要等待12小时才会生效。

-Q 7. 那我能怎么为社区贡献呢？
-A 7. 欢迎加入我们的 [Discord](https://discord.gg/R5SeTVR)，或者编辑这个 Wiki 来做贡献！

# 风险

>在Defi项目存入资金，风险自负。 Harvest或Harvest集成的协议如果出现问题可能会导致部分或全部资金损失。这不是保本的项目。DYOR，量力而行。
{.is-warning}

## 智能合约风险
Harvest的智能合约是开源的，可读的并包含我们的测试结果。并不是直接Fork现有项目的。 目前已经完成了两份审计报告，但是已有的审计报告不能保证未来新策略以及关联的项目的安全性（Curve，Swerve，Uniswap，Cream，Compound, Aave等等）。

## 组合性风险
Harvest的合约通过与其他很多合约交互来处理不同资产。合约的可组合性使得Harvest从中获利，但如果其中一个合约如果发生错误，则与多个合约进行交互会带来风险。 Harvest团队会尽最大努力来和评估合约风险，但是存款本身会因为策略的不同导致固有的风险不同。建议大家研究存款的策略，以了解实际风险。

## 资产风险

>稳定币不一定真的稳定！稳定币和合成物可能偏离锚定的价格，最终导致投资亏损。请仔细评估所有所谓的“稳定”资产的风险！
{.is-danger}

Harvest接受了很多稳定币和其他合成资产（如比特币，以太坊）。这些资产可能依赖于其他数字资产（DAI，sUSD，sBTC）的抵押，或者可能是非债务性负债，只能通过中心化的第三方（USDC，USDT，wBTC）赎回的基础资产。如果发行人将非债务性资产列入黑名单，或者合成资产抵押不足，则持有与这些资产交互的头寸可能会失去价值，甚至变得一文不值。

##自动做市商风险

>Harvest 有在Uniswap上的FARM-USDC的二池。在AMM上提供流动性是一个专业的操作，会有多种风险。使用时需要风险自负！
{.is-warning}

无常损失与在流动资金池做市有关。流动性池用于诸如Uniswap，Curve和Sushiswap之类的去中心化交易所中，流动性资金池为资产交易创造了可能性。

如果你在AMM中成为做市商存入资金提供流动性，那么做市商期间你提供的资产可能会发生资产价格的相对变化，你可能会损失部分或全部的钱。只要池子中一个资产归零，那么无论你最开始提供的是什么，都将满手的归零币。

如果你向某个池子提供流动性，而且你是赚的来自于别人更多的资金流入，那么你可能永远赚不到钱，因为这个可能是一个资金盘。在提供流动性之前，了解无常损失背后的数学原理至关重要！

许多Defi挖矿策略，包括Harvest开发并使用的策略，很多都是为了给AMM提供流动性。 **他们提供的挖矿奖励并不能保证提供流动性就能赚钱**。**

有关无常损失和AMM风险的进一步阅读：

-[关于无常损失的入门指南（https://blog.bancor.network/beginners-guide-to-getting-rekt-by-impermanent-loss-7c9510cb2f22）
-[Uniswap：对于流动性提供者来说是一笔划算的交易吗？]（https://medium.com/@pintail/uniswap-a-good-deal-for-liquidity-providers-104c0b6816f2）
-[计算Balancer池的价值，无常损失和滑点]（https://medium.com/balancer-protocol/calculating-value-impermanent-loss-and-slippage-for-balancer-pools-4371a21f1a86）
-[什么是无常损失？ DEFI解释-Uniswap，Curve，Balancer，Bancor]（https://www.youtube.com/watch?v=8XJ1MSTEuU0）

## 流动性和市场影响

>许多新的DeFi资产的流动性非常差，在交易时，由于市场影响，你可能会遭受重大损失。当价格迅速变化时，流动性可能瞬间消失。因此你可能会陷入流动性困境导致无法卖出资产。千万要仔细评估你持有的资产的流动性状况！
{.is-warning}

当交易量达到足以改变在其交易的资产的价格时，就会发生市场影响（即价格影响）。在高波动时期，当流动性下降时，市场影响会增加。

Harvest的一些策略可能涉及通过AMM支持的单个资产存入和退出Curve，Swerve，Balancer，Uniswap上的自动做市商LP头寸。当价格波动影响你存入的资产的流动性时，**那么当你提款时可能会遭受市场冲击损失。 这些损失可能显示为您的存款余额减少。** 如果资产的流动性状况有所改善，那么显示的余额也可能会改善。

