---
title: "TextDocumentInfo"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テキストドキュメント情報を表します。"
type: docs
weight: 36
url: /ja/java/com.groupdocs.parser.options/textdocumentinfo/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.DocumentInfo](../../com.groupdocs.parser.options/documentinfo)
```
public abstract class TextDocumentInfo extends DocumentInfo
```

テキストドキュメント情報を表します。

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [TextDocumentInfo()](#TextDocumentInfo--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCharset()](#getCharset--) | テキストドキュメントの検出されたエンコーディングを取得します。 |
|
### TextDocumentInfo() {#TextDocumentInfo--}
```
public TextDocumentInfo()
```


### getCharset() {#getCharset--}
```
public abstract Charset getCharset()
```


テキストドキュメントの検出されたエンコーディングを取得します。


**Returns:**
java.nio.charset.Charset - Charset クラスのインスタンスです。

