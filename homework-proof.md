---
layout: default
title: 使用 Letax 公式
---

# 使用 Letax 公式完成数学证明

## 1、 Letax 简介

[LaTeX 百度百科](https://baike.baidu.com/item/LaTeX)

[LaTet 数学公式符号速查](http://mohu.org/info/symbols/symbols.htm)

## 2、 数学证明过程 与 Markdown

例如，证明题：

> Sign extension
>
> When turning a two's-complement number with a certain number of bits into one with more bits (e.g., when copying from a 1-byte variable to a 2-byte variable), the most-significant bit must be repeated in all the extra bits.  
> detail see: https://en.wikipedia.org/wiki/Two%27s_complement#Sign_extension

证明思路: 对于正数 x ，显然成立。 对于负数 N(x) = 2^k - x  = 2^m - x where m > k。 因此，当 k 位表示的 N(x) 扩展到 m 位表示时， 它们之间的差是 2^m - 2^k = （2^m -1） - （2^k - 1）。 因式分解 （2^m -1）， 运用位值表示法得知它用 m 位 1 表示， 同理 （2^k - 1） 用 k 位 1 表示， 其差是从 k+1 到 m 位为 1。 负数 N(x) 第一位为符号位，即 1。 将第 k 位符号位重复填充到 m 位，其表示的整数不变。   例如： -42 八位二进制表示是 1101 0110 ，根据上述证明， 十六位二进制表示是 1111 1111 1101 0110。

Proof:

$\because$ Positional Notation $(x)_{k}=\sum_{i=1}^{k}d_{i}R^{i-1}$  


