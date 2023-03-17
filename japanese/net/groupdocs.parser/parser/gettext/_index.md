---
title: GetText
second_title: GroupDocs.Parser for .NET API リファレンス
description: ドキュメントからテキストを抽出します
type: docs
weight: 150
url: /ja/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

ドキュメントからテキストを抽出します。

```csharp
public TextReader GetText()
```

### 戻り値

のインスタンスTextReader抽出されたテキストを持つクラス; `ヌル`テキスト抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [ドキュメントからテキストを抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [正確なモードでテキストを抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 例

次の例は、ドキュメントからテキストを抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // テキストをリーダーに抽出します
    using(TextReader reader = parser.GetText())
    {
        // ドキュメントからテキストを出力します
        // テキスト抽出がサポートされていない場合、リーダーは null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 関連項目

* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

テキスト オプションを使用してドキュメントからテキスト ページを抽出します (生の高速テキスト抽出モードを有効にするため)。

```csharp
public TextReader GetText(TextOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| options | TextOptions | テキスト抽出オプション。 |

### 戻り値

のインスタンスTextReader抽出されたテキストを持つクラス; `ヌル`テキスト抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [正確なモードでテキストを抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Raw モードでテキストを抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 例

次の例は、ドキュメントから生のテキストを抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // 生のテキストをリーダーに抽出します
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // ドキュメントからテキストを出力します
        // テキスト抽出がサポートされていない場合、リーダーは null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 関連項目

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

ドキュメント ページからテキストを抽出します。

```csharp
public TextReader GetText(int pageIndex)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | ゼロベースのページ インデックス。 |

### 戻り値

のインスタンスTextReader抽出されたテキストを持つクラス; `ヌル`テキスト ページの抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [正確なモードでテキストを抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 例

次の例は、ドキュメント ページからテキストを抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ドキュメントがテキスト抽出をサポートしているかどうかを確認します
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるかどうかを確認します
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // ページを繰り返す
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // ページ番号を出力 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // テキストをリーダーに抽出します
        using(TextReader reader = parser.GetText(p))
        {
            // ドキュメントからテキストを出力します
            // テキスト抽出機能のサポートを以前に確認したため、null チェックは無視します
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 関連項目

* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

テキスト オプションを使用してドキュメント ページからテキストを抽出します (生の高速テキスト抽出モードを有効にするため)。

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | ゼロベースのページ インデックス。 |
| options | TextOptions | テキスト抽出オプション。 |

### 戻り値

のインスタンスTextReader抽出されたテキストを持つクラス; `ヌル`テキスト ページの抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [正確なモードでテキストを抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Raw モードでテキストを抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 例

次の例は、ドキュメント ページから未加工のテキストを抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ドキュメントがテキスト抽出をサポートしているかどうかを確認します
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // ドキュメント情報を取得する
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // ドキュメントにページがあるかどうかを確認します
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // ページを繰り返す
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // ページ番号を出力 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // テキストをリーダーに抽出します
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // ドキュメントからテキストを出力します
            // テキスト抽出機能のサポートを以前に確認したため、null チェックは無視します
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 関連項目

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
