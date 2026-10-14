---
title: "FileInfo"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ファイル情報を表します。"
type: docs
weight: 19
url: /ja/java/com.groupdocs.parser.options/fileinfo/
---
**Inheritance:**
java.lang.Object
```
public class FileInfo
```

ファイル情報を表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [FileInfo(FileType fileType, long size, boolean encrypted)](#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFileType()](#getFileType--) | ドキュメントのタイプを取得します。 |
|
|  | [getSize()](#getSize--) | ドキュメントのサイズ（バイト単位）を取得します。 |
|
|  | [isEncrypted()](#isEncrypted--) | ファイルがパスワードで保護されているかどうかを示す値を取得します。 |
|
### FileInfo(FileType fileType, long size, boolean encrypted) {#FileInfo-com.groupdocs.parser.options.FileType-long-boolean-}
```
public FileInfo(FileType fileType, long size, boolean encrypted)
```


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| fileType | [FileType](../../com.groupdocs.parser.options/filetype) |  |
| size | long |  |
| 暗号化された | boolean |  |

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


ドキュメントのタイプを取得します。


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getSize() {#getSize--}
```
public long getSize()
```


ドキュメントのサイズ（バイト単位）を取得します。


**Returns:**
long - ドキュメントのサイズ（バイト単位）を表す整数値です。

### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


ファイルがパスワードで保護されているかどうかを示す値を取得します。


**Returns:**
boolean - ファイルがパスワードで保護されている場合は true、そうでない場合は false のブール値です。

