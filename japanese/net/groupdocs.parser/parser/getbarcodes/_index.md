---
title: "GetBarcodes"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメントからバーコードを抽出します。"
type: docs
weight: 70
url: /ja/net/groupdocs.parser/parser/getbarcodes/
---

## GetBarcodes() {#getbarcodes}

ドキュメントからバーコードを抽出します。

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### 戻り値

[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) オブジェクトのコレクション; バーコード抽出がサポートされていない場合は `null`。

### 例

次の例は、ドキュメントからバーコードを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // ドキュメントからバーコードを抽出する。
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // バーコードを反復処理する
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // ページインデックスを印刷する
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // バーコードの値を出力する
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### 関連項目

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_3}

ドキュメントページからバーコードを抽出します。

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |

### 戻り値

[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) オブジェクトのコレクション; バーコード抽出がサポートされていない場合は `null`。

### 例

次の例は、ドキュメントページからバーコードを抽出する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // 2ページ目のドキュメントからバーコードを抽出する。
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // バーコードを反復処理する
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // ページインデックスを印刷する
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // バーコードの値を出力する
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### 関連項目

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(BarcodeOptions) {#getbarcodes_1}

カスタマイズオプションを使用して、ドキュメントからバーコードを抽出します。

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(BarcodeOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| options | BarcodeOptions | バーコード抽出のオプション。 |

### 戻り値

[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) オブジェクトのコレクション; バーコード抽出がサポートされていない場合は `null`。

### 例

次の例は、右上隅からバーコードを抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using (Parser parser = new Parser(filePath))
{
    // バーコード抽出に使用されるオプションを作成する
    BarcodeOptions options = new BarcodeOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // 右上隅からバーコードを抽出する。
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // バーコードを反復処理する
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // ページインデックスを印刷する
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // バーコードの値を出力する
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### 関連項目

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, BarcodeOptions) {#getbarcodes_4}

カスタマイズオプションを使用して、ドキュメントページからバーコードを抽出します。

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, BarcodeOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | 0 から始まるページインデックスです。 |
| options | BarcodeOptions | バーコード抽出のオプション。 |

### 戻り値

[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) オブジェクトのコレクション; バーコード抽出がサポートされていない場合は `null`。

### 関連項目

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
