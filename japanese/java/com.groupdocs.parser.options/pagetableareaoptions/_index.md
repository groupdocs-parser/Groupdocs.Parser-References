---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ページテーブル領域抽出に使用されるオプションを提供します。"
type: docs
weight: 31
url: /ja/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object、[com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

ページテーブル領域抽出に使用されるオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | 新しい [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) クラスのインスタンスを初期化します。 |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | 検索矩形を指定し、固定レイアウトなしで新しい [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | ページ上のテーブルを定義するテーブルレイアウトを取得します。 |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


新しい [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | ページ上のテーブルを定義するテーブルレイアウトです。 |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


検索矩形を指定し、固定レイアウトなしで新しい [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) クラスのインスタンスを初期化します。

ページの領域に自動検出されたテーブルを制限するのに便利です。C#

new PageTableAreaOptions(null) { Rectangle = ... }
パターン。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | ページ上でテーブルを検出すべき矩形領域です;  null  を渡すとページ全体を検索します。 |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


ページ上のテーブルを定義するテーブルレイアウトを取得します。


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

