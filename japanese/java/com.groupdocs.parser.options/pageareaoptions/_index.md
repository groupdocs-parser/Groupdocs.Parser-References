---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ページ領域抽出に使用されるオプションを提供します。"
type: docs
weight: 28
url: /ja/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

ページ領域抽出に使用されるオプションを提供します。

パラメータとして [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) クラスのインスタンスが [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-) に使用されます。
および [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-) メソッドです。使用例をご覧ください。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | 無視される境界のサイズを指定して、[PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | 新しい [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | ページ領域を含む矩形領域を取得します。 |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | 矩形領域でキャプチャされる際に無視される境界のサイズを取得します。 |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


無視される境界のサイズを指定して、[PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | ページ領域を含む矩形領域です。 |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


新しい [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | ページ領域を含む矩形領域です。 |
|
|  | rectangleTolerance | double | 矩形領域でキャプチャされる際に無視される境界のサイズです。テキスト項目の高さの割合で測定されます。 |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


ページ領域を含む矩形領域を取得します。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


矩形領域でキャプチャされる際に無視される境界のサイズを取得します。テキスト項目の高さの割合で測定されます。


**Returns:**
double - 0（境界なし）から 1（要素全体を無視）までの double 値です。

