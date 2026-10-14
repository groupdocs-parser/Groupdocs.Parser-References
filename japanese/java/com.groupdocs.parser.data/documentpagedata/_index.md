---
title: "DocumentPageData"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ドキュメントページのデータを表します。"
type: docs
weight: 12
url: /ja/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

ドキュメントページのデータを表します。これは、ドキュメントページからのフィールドデータを含む [FieldData](../../com.groupdocs.parser.data/fielddata) オブジェクトで構成されています。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | ページインデックスを取得します。 |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


[DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | フィールド | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | フィールドデータのコレクションです。 |
|
|  | pageIndex | int | ゼロベースのページインデックス。 |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


ページインデックスを取得します。


**Returns:**
int - ページのゼロベースインデックスです。

