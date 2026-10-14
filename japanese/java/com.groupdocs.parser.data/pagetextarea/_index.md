---
title: "PageTextArea"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレート解析またはフォーム解析機能でテキスト値を表すために使用されるページテキスト領域を表します。"
type: docs
weight: 24
url: /ja/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

テンプレート解析またはフォーム解析機能でテキスト値を表すために使用されるページテキスト領域を表します。

次のメソッドの戻り値として、[PageTextArea](../../com.groupdocs.parser.data/pagetextarea) クラスのインスタンスが使用されます:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

また、[PageTextArea](../../com.groupdocs.parser.data/pagetextarea) クラスのインスタンスが [PageArea](../../com.groupdocs.parser.data/pagearea) プロパティの値として使用されます。
\*

そこにある使用例をご覧ください。

テキスト領域は単一または複合にすることができます。最初の場合、矩形領域で囲まれたテキストを含みます。
2番目の場合、他のテキスト領域を含みます。テキストおよびテーブルのプロパティは子テキスト領域によって計算されます。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 新しい [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) クラスのインスタンスを初期化します。 |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 新しい [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) クラスのインスタンスを初期化します。 |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | 新しい [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getText()](#getText--) | テキストを取得します。 |
|
|  | [getBaseLine()](#getBaseLine--) | ベースラインを取得します。 |
|
|  | [getTextStyle()](#getTextStyle--) | フォントサイズ、フォント名などのテキストスタイルを取得します。 |
|
|  | [getAreas()](#getAreas--) | 子テキストページ領域のコレクションを取得します。 |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


新しい [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | テキスト | java.lang.String | テキストの値。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | テキスト領域を含むページ。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テキスト領域を含む矩形領域。 |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


新しい [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | テキスト | java.lang.String | テキストの値。 |
|
|  | baseLine | java.lang.Double | テキストのベースライン。 |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | テキストのスタイル。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | テキスト領域を含むページ。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | テキスト領域を含む矩形領域。 |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


新しい [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | 子テキストページ領域のコレクション。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | テキスト領域を含むページ。 |
|

### getText() {#getText--}
```
public String getText()
```


テキストを取得します。


**Returns:**
java.lang.String - テキストページ領域の値を表す文字列です。

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


ベースラインを取得します。


**Returns:**
double - ベースラインを表す double 値です。

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


フォントサイズ、フォント名などのテキストスタイルを取得します。


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


子テキストページ領域のコレクションを取得します。


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - 子テキストページ領域のコレクションです。子がいない場合は空です。

