# IAN

`IAN` means " International Article Number", (also know as "European Article Number" or "EAN")[^IAN]. It's a 13-digit code for global trade. In  ZhouYi2.0 mainly use the 977, 978, 979 subspaces to identifier magazines, books, music and other publications.

## Syntax

```
IAN:<main number>[:<additional number>]
```

`<main number>` is the IAN 13-digit code of a item.

`<additional number>` is the add-on symbol of a item (if has).

Numbers (both `<main number>` and `<additional number>`) can be seperate by `-` if need according each sub-specification.

## ISSN

介绍指杂志的 ISSN

然后是 GS1 的补充数据区分期刊号

但是后边的补充数据好像是可选的

如果附加数据不能区分具体期刊，考虑 SICI 或 PII （感觉 SICI 更靠谱一点）PII 太简陋， SICI 已经在 2012 召回了，所以干脆对于重复数字不做处理。

或者更好的方法是如果两本杂志的 GS1 连附加值都完全一样，视作一个整体，就像一个 ISBN 的上下册那样

没有条形码的杂志理论上不使用这个系统管理，这个系统只管理实体

https://www.gs1.org/standards/barcodes-epcrfid-id-keys/gs1-general-specifications (最新标准)

https://www.gs1ca.org/files/GS1_General_Specifications_V17.pdf

## ISBN

用于标记图书等出版物。

## 复制标准

这个系统中很多东西不一定是数字化的，可能是印刷品或者载体

其数字版应该是其内容的数字化复制

如果是 CD 等数字载体，则复制其数字内容

如果是 电子书可以复制其文字格式的电子版

没有电子版的书籍和杂志使用扫描件， 模拟记录载体进行数字化翻录

杂志附赠模型等也只能拍照或者采样建模保存

这些翻录不一定能做到完备

## References

[^IAN]: https://en.wikipedia.org/wiki/International_Article_Number