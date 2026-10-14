---
title: "SearchResult"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "検索機能における検索結果を表します。"
type: docs
weight: 27
url: /ja/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

検索機能における検索結果を表します。

SearchResult クラスのインスタンスは、[Parser.search(String)](../../com.groupdocs.parser/parser#search-String-) の戻り値として使用されます。
および [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-) メソッドです。使用例をご覧ください。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | [SearchResult](../../com.groupdocs.parser.data/searchresult) クラスの新しいインスタンスを初期化します。 |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | [SearchResult](../../com.groupdocs.parser.data/searchresult) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getPosition()](#getPosition--) | ドキュメントテキスト内の位置を取得します。 |
|
|  | [getText()](#getText--) | テキストを取得します。 |
|
|  | [getPageIndex()](#getPageIndex--) | テキストが見つかったページインデックスを取得します。 |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | 左側のハイライトを取得します。 |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | 右側のハイライトを取得します。 |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


[SearchResult](../../com.groupdocs.parser.data/searchresult) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 位置 | int | ドキュメントテキスト内の位置です。 |
|
|  | テキスト | java.lang.String | 見つかったテキストです。 |
|
|  | pageIndex | java.lang.Integer | テキストが見つかったページインデックスです。 |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | 左側のハイライトです。 |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | 右側のハイライトです。 |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


[SearchResult](../../com.groupdocs.parser.data/searchresult) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 位置 | int | ドキュメントテキスト内の位置です。 |
|
|  | テキスト | java.lang.String | 見つかったテキストです。 |
|
|  | pageIndex | java.lang.Integer | テキストが見つかったページインデックスです。 |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


ドキュメントテキスト内の位置を取得します。


**Returns:**
int - 検索結果の開始位置のゼロベースインデックスです。

### getText() {#getText--}
```
public String getText()
```


テキストを取得します。


**Returns:**
java.lang.String - 見つかったテキストを表す文字列値です。

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


テキストが見つかったページインデックスを取得します。


**Returns:**
java.lang.Integer - テキストが見つかったページのゼロベースインデックスです。全文書テキストで検索が行われた場合は null です。

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


左側のハイライトを取得します。


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


右側のハイライトを取得します。


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

