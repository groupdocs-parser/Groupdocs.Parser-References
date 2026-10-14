---
title: "PageGroupArea"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テンプレート解析機能でドキュメントページのさまざまなタイプのブロックをグループ化するために使用されるページ領域のグループを表します。"
type: docs
weight: 19
url: /ja/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

テンプレート解析機能でドキュメントページのさまざまなタイプのブロックをグループ化するために使用されるページ領域のグループを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getAreas()](#getAreas--) | グループ化されたページ領域のコレクションを取得します。 |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


[PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | グループ化されるページ領域のコレクションです。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 領域を含むページです。 |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


グループ化されたページ領域のコレクションを取得します。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - [PageArea](../../com.groupdocs.parser.data/pagearea) オブジェクトのコレクションです。

