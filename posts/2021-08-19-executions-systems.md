---
title: CH5-交易执行系统
description: Executions Systems
author: 王一刀
layout: post
toc: true
comments: true
categories: [量化交易]
---

## 自动交易系统能为你做什么

> An automated trading system will retrieve up-to-date market data from your brokerage or other data vendors, run a trading algorithm to generate orders, and submit those orders to your brokerage for execution.

自动交易系统从经纪商或其他供应商获取市场数据，运行交易算法形成指令，提交指令给经纪商执行。

全自动交易系统代价高昂，对于低频量化交易策略，半自动交易系统即可。

* 半自动交易系统
* 全自动交易系统

## 雇佣编程顾问

这里有个策略保密的问题，其他的讨论不值一提，但是有个方法挺好的，就是把策略拆分雇佣不同的程序员，没人实现一部分，最后再合并。

## 最小化交易成本

* 可以通过避免交易低价股票来降低佣金
* 根据股票的流动性来限制指令规模以减小市场冲击成本。警惕成交量小的股票，购买量不要超过其每日成交量的1%。
* 根据股票市值来调整下单量也是减少市场冲击的方法

  但是不要按线性比率来调整下单量，因为公司市值差别巨大，按照固定比例会让下公司的下单量为0

* 如果是超大单，分批次下单，以减少市场冲击。独立交易者通常不需要。

## 用仿真交易测试交易系统

## 为什么实际业绩偏离预期

* 自动交易软件是否有bug
* 自动交易系统产生的交易和回测程序产生的交易是否一致
* 交易成本是否比预期的高很多
* 是否交易了流动性差的股票产生了市场冲击
* 数据迁就偏差
* 状态变更影响，市场结构和宏观经济环境发生巨变





