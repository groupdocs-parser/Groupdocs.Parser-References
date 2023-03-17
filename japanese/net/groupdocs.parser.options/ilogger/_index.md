---
title: ILogger
second_title: GroupDocs.Parser for .NET API リファレンス
description: データ抽出中にイベントとエラーを記録するために使用されるロガーのインターフェイスを定義します
type: docs
weight: 440
url: /ja/net/groupdocs.parser.options/ilogger/
---
## ILogger interface

データ抽出中にイベントとエラーを記録するために使用されるロガーのインターフェイスを定義します。

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

**もっと詳しく知る：**

* [ロギング](https://docs.groupdocs.com/display/parsernet/Logging)

### 関連項目

* 名前空間 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 組み立て [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->