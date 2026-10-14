---
title: "ContainerItem"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "Zip アーカイブエンティティ、メール添付ファイル、PDF ポートフォリオ項目などのコンテナ項目を表します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Zip アーカイブエンティティ、メール添付ファイル、PDF ポートフォリオ項目などのコンテナ項目を表します。

[ContainerItem](../../com.groupdocs.parser.data/containeritem) クラスのインスタンスが [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--) メソッドの戻り値として使用されます。使用例をご覧ください。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | [ContainerItem](../../com.groupdocs.parser.data/containeritem) をアイテム名とディレクトリで新しいインスタンスとして初期化します。 |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | アイテムの完全パスで [ContainerItem](../../com.groupdocs.parser.data/containeritem) の新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getName()](#getName--) | アイテムの名前を取得します。 |
|
|  | [getDirectory()](#getDirectory--) | アイテムのディレクトリを取得します。 |
|
|  | [getFilePath()](#getFilePath--) | アイテムの完全パスを取得します。 |
|
|  | [getSize()](#getSize--) | アイテムのサイズを取得します。 |
|
|  | [getMetadata()](#getMetadata--) | メタデータ項目のコレクションを取得します。 |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | メタデータの値を取得します。 |
|
|  | [openStream()](#openStream--) | アイテムのコンテンツストリームを開きます。 |
|
|  | [openParser()](#openParser--) | アイテムのコンテンツ用に [Parser](../../com.groupdocs.parser/parser) オブジェクトを作成します。 |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | アイテムのコンテンツ用に [Parser](../../com.groupdocs.parser/parser) オブジェクトを [LoadOptions](../../com.groupdocs.parser.options/loadoptions) と共に作成します。 |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | アイテムのコンテンツ用に [Parser](../../com.groupdocs.parser/parser) オブジェクトを [LoadOptions](../../com.groupdocs.parser.options/loadoptions) と [ParserSettings](../../com.groupdocs.parser.options/parsersettings) と共に作成します。 |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | コンテナアイテムのファイルタイプを検出します。 |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


[ContainerItem](../../com.groupdocs.parser.data/containeritem) をアイテム名とディレクトリで新しいインスタンスとして初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 名前 | java.lang.String | アイテムの名前。 |
|
|  | ディレクトリ | java.lang.String | アイテムのディレクトリ。 |
|
|  | size | long | アイテムのサイズ。 |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | メタデータ項目のコレクション。 |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


アイテムの完全パスで [ContainerItem](../../com.groupdocs.parser.data/containeritem) の新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | アイテムの完全パス。 |
|
|  | size | long | アイテムのサイズ。 |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | メタデータ項目のコレクション。 |
|

### getName() {#getName--}
```
public String getName()
```


アイテムの名前を取得します。


**Returns:**
java.lang.String - アイテムのファイル名（ディレクトリなし）を表す文字列値。

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


アイテムのディレクトリを取得します。


**Returns:**
java.lang.String - アイテムのディレクトリ（ファイル名なし）を表す文字列値。

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


アイテムの完全パスを取得します。


**Returns:**
java.lang.String - アイテムの完全パスを表す文字列値。

### getSize() {#getSize--}
```
public long getSize()
```


アイテムのサイズを取得します。


**Returns:**
long - アイテムのサイズ（バイト単位）を表す整数値。

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


メタデータ項目のコレクションを取得します。


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - [MetadataItem](../../com.groupdocs.parser.data/metadataitem) オブジェクトのコレクション。メタデータが設定されていない場合は空です。

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


メタデータの値を取得します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 名前 | java.lang.String | メタデータの名前。 |
|

**Returns:**
java.lang.String - メタデータ項目の値を表す文字列値。該当する名前のメタデータが見つからない場合は  null  です。

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


アイテムのコンテンツストリームを開きます。


**Returns:**
java.io.InputStream - アイテムのコンテンツを含むストリームです。

### openParser() {#openParser--}
```
public Parser openParser()
```


アイテムのコンテンツ用に [Parser](../../com.groupdocs.parser/parser) オブジェクトを作成します。


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


アイテムのコンテンツ用に [Parser](../../com.groupdocs.parser/parser) オブジェクトを [LoadOptions](../../com.groupdocs.parser.options/loadoptions) と共に作成します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | アイテムのコンテンツを開くためのオプションです。 |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


アイテムのコンテンツ用に [Parser](../../com.groupdocs.parser/parser) オブジェクトを [LoadOptions](../../com.groupdocs.parser.options/loadoptions) と [ParserSettings](../../com.groupdocs.parser.options/parsersettings) と共に作成します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | アイテムのコンテンツを開くためのオプションです。 |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | データ抽出をカスタマイズするために使用されるパーサー設定です。 |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


コンテナアイテムのファイルタイプを検出します。


detectionMode
parameter はファイルタイプ検出を制御する機能を提供します：

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

以下の例は、コンテナアイテムのファイルタイプを検出する方法を示しています：

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Extract attachments from the container
     Iterable attachments = parser.getContainer();
     // Check if container extraction is supported
     if (attachments == null) {
         System.out.println("Container extraction isn't supported");
     }
     // Iterate over attachments
     for (ContainerItem item : attachments) {
         // Detect the file type
         FileType fileType = item.detectFileType(FileTypeDetectionMode.Default);
         // Print the name and file type
         System.out.println(String.format("%s: %s", item.getName(), fileType));
     }
 }
 
````



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | ファイルタイプ検出のモードを定義します。 |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

