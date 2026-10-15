---
title: "ILogger"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "データ抽出中のイベントやエラーのロギングに使用されるロガーのインターフェイスを定義します。"
type: docs
weight: 380
url: /ja/net/groupdocs.parser.options/ilogger/
---

## ILogger interface

データ抽出中のイベントやエラーのロギングに使用されるロガーのインターフェイスを定義します。

```csharp
public interface ILogger
```

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Error](../../groupdocs.parser.options/ilogger/error)(string, Exception) | データ抽出中に発生したエラーを記録します。 |
| [Trace](../../groupdocs.parser.options/ilogger/trace)(string) | データ抽出中に発生したイベントを記録します。 |
| [Warning](../../groupdocs.parser.options/ilogger/warning)(string) | データ抽出中に発生した警告を記録します。 |

### 備考

**Learn more:**

* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
