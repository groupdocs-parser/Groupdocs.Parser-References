---
title: "MetadataItem"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "コンテナ項目およびメタデータ抽出機能で使用されるメタデータ項目を表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

コンテナ項目およびメタデータ抽出機能で使用されるメタデータ項目を表します。

インスタンス [MetadataItem](../../com.groupdocs.parser.data/metadataitem) クラスは、[Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--) メソッドの戻り値として使用されます
そして、[ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--) コレクションの項目としても使用されます。使用例はそちらをご覧ください。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | 新しい [MetadataItem](../../com.groupdocs.parser.data/metadataitem) クラスのインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getName()](#getName--) | メタデータ項目の名前を取得します。 |
|
|  | [getValue()](#getValue--) | メタデータ項目の値を取得します。 |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


新しい [MetadataItem](../../com.groupdocs.parser.data/metadataitem) クラスのインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 名前 | java.lang.String | メタデータ項目の名前です。 |
|
|  | 値 | java.lang.String | メタデータ項目の値です。 |
|

### getName() {#getName--}
```
public String getName()
```


メタデータ項目の名前を取得します。


**Returns:**
java.lang.String - メタデータ項目の名前を表す文字列です。

### getValue() {#getValue--}
```
public String getValue()
```


メタデータ項目の値を取得します。


**Returns:**
java.lang.String - メタデータ項目の値を表す文字列です。

