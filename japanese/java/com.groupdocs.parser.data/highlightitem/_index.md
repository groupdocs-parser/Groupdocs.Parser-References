---
title: "HighlightItem"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "検索機能で見つかったテキストの文脈を説明するために通常使用される、テキストの一部をハイライトすることを表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

検索機能で見つかったテキストのコンテキストを説明するために通常使用される、テキストの一部であるハイライトを表します。

インスタンス [HighlightItem](../../com.groupdocs.parser.data/highlightitem) クラスは、[Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) メソッドの戻り値として使用されます、
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | 新しい [HighlightItem](../../com.groupdocs.parser.data/highlightitem) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getPosition()](#getPosition--) | ドキュメントテキスト内の位置を取得します。 |
|
|  | [getText()](#getText--) | ハイライトのテキストを取得します。 |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


新しい [HighlightItem](../../com.groupdocs.parser.data/highlightitem) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 位置 | int | ドキュメントテキスト内の位置です。 |
|
|  | テキスト | java.lang.String | ハイライトのテキストです。 |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


ドキュメントテキスト内の位置を取得します。


**Returns:**
int - ハイライトの開始位置のゼロベースインデックスです。

### getText() {#getText--}
```
public String getText()
```


ハイライトのテキストを取得します。


**Returns:**
java.lang.String - ハイライトのテキストを表す文字列値です。

