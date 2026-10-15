---
title: "GetFileInfo"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ファイルに関する一般情報を返します。"
type: docs
weight: 260
url: /ja/net/groupdocs.parser/parser/getfileinfo/
---

## GetFileInfo(string) {#getfileinfo_2}

ファイルに関する一般情報を返します。

```csharp
public static FileInfo GetFileInfo(string filePath)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ファイルへのパス。 |

### 戻り値

[`FileInfo`](../../../groupdocs.parser.options/fileinfo) クラスのインスタンスです。

### 例

次のコードは、ファイルがパスワードで保護されているかどうかを確認する方法を示しています。

```csharp
// ファイル情報を取得する
Options.FileInfo info = Parser.GetFileInfo(filePath);
// IsEncrypted プロパティを確認する
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### 関連項目

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(string, LoadOptions) {#getfileinfo_3}

ファイルに関する一般情報を返します。

```csharp
public static FileInfo GetFileInfo(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| filePath | 文字列 | ファイルへのパス。 |
| loadOptions | LoadOptions | ファイルを開くためのオプションです。 |

### 戻り値

[`FileInfo`](../../../groupdocs.parser.options/fileinfo) クラスのインスタンスです。

### 例

次のコードは、パスワードで保護されたドキュメントのファイルタイプを確認する方法を示しています。

```csharp
// ファイル情報を取得する
Options.FileInfo info = Parser.GetFileInfo(filePath, new LoadOptions("password"));
// IsEncrypted プロパティを確認する
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// ファイルタイプを出力する
Console.WriteLine(info.FileType.ToString());
```

### 関連項目

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream) {#getfileinfo}

ファイルに関する一般情報を返します。

```csharp
public static FileInfo GetFileInfo(Stream document)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| ドキュメント | Stream | ソース入力ストリームです。 |

### 戻り値

[`FileInfo`](../../../groupdocs.parser.options/fileinfo) クラスのインスタンスです。

### 例

次のコードは、ファイルがパスワードで保護されているかどうかを確認する方法を示しています。

```csharp
// ファイル情報を取得する
Options.FileInfo info = Parser.GetFileInfo(document);
// IsEncrypted プロパティを確認する
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### 関連項目

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream, LoadOptions) {#getfileinfo_1}

ファイルに関する一般情報を返します。

```csharp
public static FileInfo GetFileInfo(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| ドキュメント | Stream | ソース入力ストリームです。 |
| loadOptions | LoadOptions | ファイルを開くためのオプションです。 |

### 戻り値

[`FileInfo`](../../../groupdocs.parser.options/fileinfo) クラスのインスタンスです。

### 例

次のコードは、パスワードで保護されたドキュメントのファイルタイプを確認する方法を示しています。

```csharp
// ファイル情報を取得する
Options.FileInfo info = Parser.GetFileInfo(document);
// IsEncrypted プロパティを確認する
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// ファイルタイプを出力する
Console.WriteLine(info.FileType.ToString());
```

### 関連項目

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
