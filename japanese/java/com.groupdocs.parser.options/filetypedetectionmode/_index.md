---
title: "FileTypeDetectionMode"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ファイルタイプ検出のモードを定義します。"
type: docs
weight: 44
url: /ja/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

ファイルタイプ検出のモードを定義します。

## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [Default](#Default) | ファイルタイプはファイル拡張子で検出されます。拡張子が認識されない場合は、ファイルコンテンツで検出されます。 |
|
|  | [Extension](#Extension) | ファイルタイプはファイル拡張子のみで検出されます。 |
|
|  | [Content](#Content) | ファイルタイプはファイルコンテンツのみで検出されます。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


ファイルタイプはファイル拡張子で検出されます。拡張子が認識されない場合は、ファイルコンテンツで検出されます。


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


ファイルタイプはファイル拡張子のみで検出されます。


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


ファイルタイプはファイルコンテンツのみで検出されます。


### values() {#values--}
```
public static FileTypeDetectionMode[] values()
```




**Returns:**
com.groupdocs.parser.options.FileTypeDetectionMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static FileTypeDetectionMode valueOf(String name)
```




**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)
