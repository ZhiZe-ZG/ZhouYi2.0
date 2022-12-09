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

用于标记杂志和报纸等连续出版物，每个出版物一个 8 位编号，其最后一位是校验位。在 IAN 中使用时仅使用其中的前 7 位。

IAN 的杂志编号以 `977` 开头，后接 7 位 ISSN。最后一位是 IAN 校验位，其余两位用于表示额外信息（如版本变种等）。杂志的期号则一般用 IAN 的 additional number 表示。因此记录杂志的 IAN 时要记录 additional number （如果有的话）。

如果不同的杂志对应完全相同的 IAN （即便 additional number 也一致），则这些不同的杂志视为同一本杂志的不同部分。此外不再使用其他区分杂志期号的额外信息。

## ISBN

用于标记图书等出版物。以 `978` 或 `979` 开头。其号码不同分段可以表示地区和出版社等信息，但是没有统一的划分方式。目前可以 [ISBN converter](https://www.isbn.org/ISBN_converter) 的格式化的转换结果为准。

如果没有分册或者额外内容等需要识别， ISBN 码段的 IAN 即便附有 additional number 也可以不记录。

## ISMN

用于标记音频出版物，使用 `979` 开头（与 ISBN 共用）。其不同分段可以表示地区和出版社等信息。如果出版物上没有标注分段，可以参考 [ISMN directory](https://www.ismn-international.org/directory) 标注。

## References

[^IAN]: https://en.wikipedia.org/wiki/International_Article_Number