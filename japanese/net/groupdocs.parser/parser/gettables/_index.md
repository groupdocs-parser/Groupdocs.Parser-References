---
title: "GetTables"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントからテーブルを抽出します。"
type: docs
weight: 170
url: /ja/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

ドキュメントからテーブルを抽出します。

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| options | PageTableAreaOptions | テーブル抽出のオプションです。 |

### 戻り値

テーブル抽出がサポートされていない場合は `null` になる、[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) オブジェクトのコレクションです。

### 例

次の例は、ドキュメント全体からテーブルを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがテーブル抽出をサポートしているか確認する
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // テーブルのレイアウトを作成する
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // テーブル抽出のオプションを作成する
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // ドキュメントからテーブルを抽出する
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // テーブルを反復処理する
    foreach (PageTableArea t in tables)
    {
        // 行を反復処理する
        for (int row = 0; row < t.RowCount; row++)
        {
            // 列を反復処理する
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // テーブルセルを取得する
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // テーブルセルのテキストを出力する
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### 関連項目

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

ドキュメントページからテーブルを抽出します。

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |
| options | PageTableAreaOptions | テーブル抽出のオプションです。 |

### 戻り値

テーブル抽出がサポートされていない場合は `null` になる、[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) オブジェクトのコレクションです。

### 例

次の例は、ドキュメントページからテーブルを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがテーブル抽出をサポートしているか確認する
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // テーブルのレイアウトを作成する
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // テーブル抽出のオプションを作成する
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるか確認する
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // ページを反復処理する
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力する
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // ドキュメントページからテーブルを抽出する
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // テーブルを反復処理する
        foreach (PageTableArea t in tables)
        {
            // 行を反復処理する
            for (int row = 0; row < t.RowCount; row++)
            {
                // 列を反復処理する
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // テーブルセルを取得する
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // テーブルセルのテキストを出力する
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### 関連項目

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

ドキュメントからテーブルを抽出します。

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### 戻り値

テーブル抽出がサポートされていない場合は `null` になる、[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) オブジェクトのコレクションです。

### 例

次の例は、ドキュメント全体からテーブルを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがテーブル抽出をサポートしているか確認する
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // ドキュメントからテーブルを抽出する
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // テーブルを反復処理する
    foreach (PageTableArea t in tables)
    {
        // 行を反復処理する
        for (int row = 0; row < t.RowCount; row++)
        {
            // 列を反復処理する
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // テーブルセルを取得する
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // テーブルセルのテキストを出力する
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### 関連項目

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

ドキュメントページからテーブルを抽出します。

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |

### 戻り値

テーブル抽出がサポートされていない場合は `null` になる、[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) オブジェクトのコレクションです。

### 例

次の例は、ドキュメントページからテーブルを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントがテーブル抽出をサポートしているか確認する
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるか確認する
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // ページを反復処理する
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力する
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // ドキュメントページからテーブルを抽出する
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // テーブルを反復処理する
        foreach (PageTableArea t in tables)
        {
            // 行を反復処理する
            for (int row = 0; row < t.RowCount; row++)
            {
                // 列を反復処理する
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // テーブルセルを取得する
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // テーブルセルのテキストを出力する
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### 関連項目

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
