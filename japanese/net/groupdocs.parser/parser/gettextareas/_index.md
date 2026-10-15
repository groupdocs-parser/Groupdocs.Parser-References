---
title: "GetTextAreas"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントからテキスト領域を抽出します。"
type: docs
weight: 190
url: /ja/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

ドキュメントからテキスト領域を抽出します。

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### 戻り値

テキスト領域抽出がサポートされていない場合は `null`、それ以外は [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) オブジェクトのコレクションです。

### 備考

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 例

次の例はドキュメント全体からすべてのテキスト領域を抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // テキスト領域を抽出
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // テキスト領域抽出がサポートされているか確認
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // ページのテキスト領域を反復処理
    foreach(PageTextArea a in areas)
    {
        // ページインデックス、矩形、テキスト領域の値を出力:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

カスタマイズオプション（正規表現、大小文字の一致など）を使用してドキュメントからテキスト領域を抽出します。

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| options | PageTextAreaOptions | テキスト領域抽出のオプションです。 |

### 戻り値

テキスト領域抽出がサポートされていない場合は `null`、それ以外は [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) オブジェクトのコレクションです。

### 備考

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 例

次の例は左上隅から数字のみを含むテキスト領域を抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // テキスト領域抽出に使用されるオプションを作成
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // ページの左上隅から数字のみを含むテキスト領域を抽出:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // テキスト領域抽出がサポートされているか確認
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // ページのテキスト領域を反復処理
    foreach(PageTextArea a in areas)
    {
        // ページインデックス、矩形、テキスト領域の値を出力:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

ドキュメントページからテキスト領域を抽出します。

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |

### 戻り値

テキスト領域抽出がサポートされていない場合は `null`、それ以外は [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) オブジェクトのコレクションです。

### 備考

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 例

ドキュメントページからテキスト領域を抽出するには、次のメソッドを使用します:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ドキュメントがテキスト領域抽出をサポートしているか確認
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるか確認する
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // ページを反復処理する
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力する
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // ページのテキスト領域を反復処理
        // テキスト領域抽出機能のサポートは既に確認済みなので、null チェックは無視します
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // 矩形とテキスト領域の値を出力:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

カスタマイズオプション（正規表現、大小文字の一致など）を使用してドキュメントページからテキスト領域を抽出します。

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |
| options | PageTextAreaOptions | テキスト領域抽出のオプションです。 |

### 戻り値

テキスト領域抽出がサポートされていない場合は `null`、それ以外は [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) オブジェクトのコレクションです。

### 備考

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
