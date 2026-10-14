---
title: "DocumentInfo"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ドキュメント情報を表します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

ドキュメント情報を表します。

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFileType()](#getFileType--) | ドキュメントのタイプを取得します。 |
|
|  | [getPageCount()](#getPageCount--) | ドキュメントの総ページ数を取得します。 |
|
|  | [getRawPageCount()](#getRawPageCount--) | ドキュメントの生ページ総数を取得します。 |
|
|  | [getSize()](#getSize--) | ドキュメントのサイズ（バイト単位）を取得します。 |
|
|  | [getPages()](#getPages--) | ページのインデックスやサイズなどの情報を取得します。 |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


ドキュメントのタイプを取得します。


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


ドキュメントの総ページ数を取得します。


**Returns:**
int - 総ページ数を表す整数値です。

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


ドキュメントの生ページ総数を取得します。

生テキスト抽出のために、[getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) プロパティの代わりに [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) プロパティを使用してください。
一部のドキュメントでは、正確なテキスト抽出モードと生テキスト抽出モードでページ番号が異なる場合があります。
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - 生ページ総数を表す整数値です。

### getSize() {#getSize--}
```
public abstract long getSize()
```


ドキュメントのサイズ（バイト単位）を取得します。


**Returns:**
long - ドキュメントのサイズ（バイト単位）を表す整数値です。

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


ページのインデックスやサイズなどの情報を取得します。


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - [PageInfo](../../com.groupdocs.parser.options/pageinfo) クラスのインスタンスのコレクションです。

