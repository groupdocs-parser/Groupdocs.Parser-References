---
title: "LoadOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "LoadOptionsgroupdocs.parser.options/loadoptions クラスの新しいインスタンスを、Passwordgroupdocs.parser.options/loadoptions/password が空で、FileFormatgroupdocs.parser.options/loadoptions/fileformat が Unknown に等しく、デフォルトのエンコーディングで初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

空の [`Password`](../password) と、[`FileFormat`](../fileformat) が Unknown に等しい状態で、[`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions()
```

### 関連項目

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

*timeout* を使用して、[`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(TimeSpan timeout)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| timeout | TimeSpan | 待機するミリ秒数を表す TimeSpan です。 |

### 関連項目

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

[`FileFormat`](../fileformat) が Unknown に等しく、デフォルトのエンコーディングで、[`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(string password)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| パスワード | 文字列 | パスワード保護されたファイルを開くためのパスワードです。 |

### 関連項目

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

空の [`Password`](../password) とデフォルトのエンコーディングで、[`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| fileFormat | FileFormat | ファイルの形式です。 |

### 関連項目

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

パスワードとデフォルトのエンコーディングで、[`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| fileFormat | FileFormat | ファイルの形式です。 |
| パスワード | 文字列 | パスワード保護されたファイルを開くためのパスワードです。 |

### 関連項目

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

カスタムエンコーディングで、[`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| fileFormat | FileFormat | ファイルの形式です。 |
| パスワード | 文字列 | パスワード保護されたファイルを開くためのパスワードです。 |
| encoding | Encoding | ドキュメントのエンコーディングです。 |
| defaultAnsiEncoding | Encoding | エンコーディング検出に使用されるデフォルトの ANSI エンコーディングです。 |

### 関連項目

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

完全にカスタマイズされた [`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| fileFormat | FileFormat | ファイルの形式です。 |
| パスワード | 文字列 | パスワード保護されたファイルを開くためのパスワードです。 |
| encoding | Encoding | ドキュメントのエンコーディングです。 |
| defaultAnsiEncoding | Encoding | エンコーディング検出に使用されるデフォルトの ANSI エンコーディングです。 |
| timeout | TimeSpan | 待機するミリ秒数を表す TimeSpan です。 |

### 関連項目

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

空の [`Password`](../password) とデフォルトのエンコーディングで、[`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(FileType fileType)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| fileType | FileType | ファイルのタイプです。 |

### 関連項目

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

パスワードとデフォルトのエンコーディングで、[`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(FileType fileType, string password)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| fileType | FileType | ファイルのタイプです。 |
| パスワード | 文字列 | パスワード保護されたファイルを開くためのパスワードです。 |

### 関連項目

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

カスタムエンコーディングで、[`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| fileType | FileType | ファイルのタイプです。 |
| パスワード | 文字列 | パスワード保護されたファイルを開くためのパスワードです。 |
| encoding | Encoding | ドキュメントのエンコーディングです。 |
| defaultAnsiEncoding | Encoding | エンコーディング検出に使用されるデフォルトの ANSI エンコーディングです。 |

### 関連項目

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

完全にカスタマイズされた [`LoadOptions`](../../loadoptions) クラスの新しいインスタンスを初期化します。

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| fileType | FileType | ファイルのタイプです。 |
| パスワード | 文字列 | パスワード保護されたファイルを開くためのパスワードです。 |
| encoding | Encoding | ドキュメントのエンコーディングです。 |
| defaultAnsiEncoding | Encoding | エンコーディング検出に使用されるデフォルトの ANSI エンコーディングです。 |
| timeout | TimeSpan | 待機するミリ秒数を表す TimeSpan です。 |

### 関連項目

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
