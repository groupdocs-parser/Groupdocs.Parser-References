---
title: "LoadOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "ファイルを開くために使用されるオプションを提供します。"
type: docs
weight: 24
url: /ja/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

ファイルを開くために使用されるオプションを提供します。

このクラスのインスタンスは、[Parser](../../com.groupdocs.parser/parser) クラスのコンストラクタでパラメータとして使用されます:

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

そこにある使用例をご覧ください。

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | 新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを timeout で初期化します。 |
|
|  | [LoadOptions()](#LoadOptions--) | 新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを、空の Password、FileFormat が FileFormat.Unknown に等しい、そしてデフォルトのエンコーディングで初期化します。 |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | 新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを、FileFormat が FileFormat.Unknown に等しく、デフォルトのエンコーディングで初期化します。 |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | 新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを、空の Password とデフォルトのエンコーディングで初期化します。 |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | 新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスをデフォルトのエンコーディングで初期化します。 |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | 新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスをカスタムエンコーディングで初期化します。 |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | 完全にカスタマイズされた [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | 新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを、空の Password とデフォルトのエンコーディングで初期化します。 |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | 新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを password とデフォルトのエンコーディングで初期化します。 |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | 新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスをカスタムエンコーディングで初期化します。 |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | 完全にカスタマイズされた [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | ファイル形式を取得します。 |
|
|  | [getFileType()](#getFileType--) | ファイルタイプを取得します。 |
|
|  | [getPassword()](#getPassword--) | パスワードを取得します。 |
|
|  | [getCharset()](#getCharset--) | ドキュメントのエンコーディングを取得します。 |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | エンコーディング検出に使用されるデフォルトの ANSI エンコーディングを取得します。 |
|
|  | [getTimeout()](#getTimeout--) | 待機時間（ミリ秒）を表す値を取得します。 |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを timeout で初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | timeout | java.time.Duration | 待機時間（ミリ秒）を表す Duration。 |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを、空の Password、FileFormat が FileFormat.Unknown に等しい、そしてデフォルトのエンコーディングで初期化します。


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを、FileFormat が FileFormat.Unknown に等しく、デフォルトのエンコーディングで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | password | java.lang.String | パスワード保護されたファイルを開くための password。 |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを、空の Password とデフォルトのエンコーディングで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | ファイルの format。 |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスをデフォルトのエンコーディングで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | ファイルの format。 |
|
|  | password | java.lang.String | パスワード保護されたファイルを開くための password。 |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスをカスタムエンコーディングで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | ファイルの format。 |
|
|  | password | java.lang.String | パスワード保護されたファイルを開くための password。 |
|
|  | charset | java.nio.charset.Charset | ドキュメントの encoding。 |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | エンコーディング検出に使用されるデフォルトの ANSI encoding。 |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


完全にカスタマイズされた [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | ファイルの format。 |
|
|  | password | java.lang.String | パスワード保護されたファイルを開くための password。 |
|
|  | charset | java.nio.charset.Charset | ドキュメントの encoding。 |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | エンコーディング検出に使用されるデフォルトの ANSI encoding。 |
|
|  | timeout | java.time.Duration | 待機時間（ミリ秒）を表す Duration。 |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを、空の Password とデフォルトのエンコーディングで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | ファイルのタイプ。 |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスを password とデフォルトのエンコーディングで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | ファイルのタイプ。 |
|
|  | password | java.lang.String | パスワード保護されたファイルを開くための password。 |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


新しい [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスのインスタンスをカスタムエンコーディングで初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | ファイルのタイプ。 |
|
|  | password | java.lang.String | パスワード保護されたファイルを開くための password。 |
|
|  | charset | java.nio.charset.Charset | ドキュメントの encoding。 |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | エンコーディング検出に使用されるデフォルトの ANSI encoding。 |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


完全にカスタマイズされた [LoadOptions](../../com.groupdocs.parser.options/loadoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | ファイルのタイプ。 |
|
|  | password | java.lang.String | パスワード保護されたファイルを開くための password。 |
|
|  | charset | java.nio.charset.Charset | ドキュメントの encoding。 |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | エンコーディング検出に使用されるデフォルトの ANSI encoding。 |
|
|  | timeout | java.time.Duration | 待機時間（ミリ秒）を表す Duration。 |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


ファイル形式を取得します。


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


ファイルタイプを取得します。


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


パスワードを取得します。


**Returns:**
java.lang.String - パスワード保護されたファイルを開くためのパスワードを表す文字列値。

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


ドキュメントのエンコーディングを取得します。


**Returns:**
java.nio.charset.Charset - ドキュメントのエンコーディングを表す Charset クラスのインスタンス。設定されていない場合は null。

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


エンコーディング検出に使用されるデフォルトの ANSI エンコーディングを取得します。


**Returns:**
java.nio.charset.Charset - ドキュメントのエンコーディングを表す Charset クラスのインスタンス。設定されていない場合は null。

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


待機時間（ミリ秒）を表す値を取得します。


**Returns:**
java.time.Duration - 待機するミリ秒数を表す Duration のインスタンス。

