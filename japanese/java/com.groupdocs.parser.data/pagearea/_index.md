---
title: "PageArea"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレート解析機能でドキュメントページ上のブロックを表すために使用されるページ領域の抽象基底クラスを表します。"
type: docs
weight: 17
url: /ja/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

テンプレート解析機能でドキュメントページ上のブロックを表すために使用されるページ領域の抽象基底クラスを表します。

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 矩形領域を取得します。 |
|
|  | [getPage()](#getPage--) | ページインデックスやページサイズなど、ドキュメントページ情報を取得します。 |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


矩形領域を取得します。


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


ページインデックスやページサイズなど、ドキュメントページ情報を取得します。


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

