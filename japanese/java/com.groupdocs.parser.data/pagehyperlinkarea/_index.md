---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ページ上のハイパーリンクを表すために使用されるページ領域を表します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

ページ上のハイパーリンクを表すために使用されるページ領域を表します。

次のメソッドの戻り値として、[PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) クラスのインスタンスが使用されます。

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

そこにある使用例をご覧ください。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getText()](#getText--) | ハイパーリンクのテキストを取得します。 |
|
|  | [getUrl()](#getUrl--) | ハイパーリンクの URL を取得します。 |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


[PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | テキスト | java.lang.String | ハイパーリンクのテキスト。 |
|
|  | url | java.lang.String | ハイパーリンクの URL。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | ハイパーリンクを含むページ。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | ハイパーリンクを含む矩形領域。 |
|

### getText() {#getText--}
```
public String getText()
```


ハイパーリンクのテキストを取得します。


**Returns:**
java.lang.String - ハイパーリンクテキストを表す文字列値。

### getUrl() {#getUrl--}
```
public String getUrl()
```


ハイパーリンクの URL を取得します。


**Returns:**
java.lang.String - ハイパーリンク URL を表す文字列値。

