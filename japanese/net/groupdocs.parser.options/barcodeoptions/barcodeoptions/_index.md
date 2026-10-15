---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "BarcodeOptionsgroupdocs.parser.options/barcodeoptions クラスの新しいインスタンスをデフォルト値で初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.options/barcodeoptions/barcodeoptions/
---

## BarcodeOptions() {#constructor}

[`BarcodeOptions`](../../barcodeoptions) クラスの新しいインスタンスをデフォルト値で初期化します。

```csharp
public BarcodeOptions()
```

### 関連項目

* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle) {#constructor_1}

[`BarcodeOptions`](../../barcodeoptions) クラスの新しいインスタンスを矩形領域と共に初期化します。

```csharp
public BarcodeOptions(Rectangle rectangle)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| rectangle | 矩形 | バーコードを含む矩形領域です。 |

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(QualityMode, QualityMode, params string[]) {#constructor_3}

[`BarcodeOptions`](../../barcodeoptions) クラスの新しいインスタンスを品質設定とコードタイプと共に初期化します。

```csharp
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, 
    params string[] codeTypes)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| imageQuality | QualityMode | ソース画像の品質です。 |
| barcodeQuality | QualityMode | ソースバーコードの品質。 |
| codeTypes | String[] | 読み取るバーコードのタイプ。 |

### 関連項目

* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) {#constructor_2}

[`BarcodeOptions`](../../barcodeoptions) クラスの新しいインスタンスを初期化します。

```csharp
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, 
    float? dimension, bool allowIncorrectBarcodes, params string[] codeTypes)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| rectangle | 矩形 | バーコードを含む矩形領域です。 |
| imageQuality | QualityMode | ソース画像の品質です。 |
| barcodeQuality | QualityMode | ソースバーコードの品質。 |
| dimension | Nullable`1 | バーコード最小要素の最小サイズ。 |
| allowIncorrectBarcodes | Boolean | 不正なバーコードが許可されているかどうかを示す値。 |
| codeTypes | String[] | 読み取るバーコードのタイプ。 |

### 関連項目

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
