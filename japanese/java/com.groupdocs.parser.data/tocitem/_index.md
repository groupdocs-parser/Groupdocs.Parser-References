---
title: "TocItem"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "目次抽出機能で使用される項目を表します。"
type: docs
weight: 31
url: /ja/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

目次抽出機能で使用される項目を表します。

[TocItem](../../com.groupdocs.parser.data/tocitem) クラスのインスタンスは、[Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) メソッドの戻り値として使用されます。使用例をご覧ください。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | TocItem クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDepth()](#getDepth--) | 深さレベルを取得します。 |
|
|  | [getText()](#getText--) | テキストを取得します。 |
|
|  | [getPageIndex()](#getPageIndex--) | ページインデックスを取得します。 |
|
|  | [extractText()](#extractText--) | TocItem オブジェクトが参照するドキュメントからテキストを抽出します。 |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


TocItem クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 深さ | int | 項目の深さレベルです。 |
|
|  | テキスト | java.lang.String | 項目のテキストです。 |
|
|  | pageIndex | java.lang.Integer | 項目が参照するページのインデックス |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


深さレベルを取得します。


**Returns:**
int - 項目の深さレベルを表す整数値です。

### getText() {#getText--}
```
public String getText()
```


テキストを取得します。


**Returns:**
java.lang.String - 項目のテキストを表す文字列です。

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


ページインデックスを取得します。


**Returns:**
java.lang.Integer - 項目が参照するページのインデックスを表す整数値です。設定されていない場合は  null  です。

### extractText() {#extractText--}
```
public TextReader extractText()
```


TocItem オブジェクトが参照するドキュメントからテキストを抽出します。

次の例は目次項目からテキストを抽出する方法です。

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.

