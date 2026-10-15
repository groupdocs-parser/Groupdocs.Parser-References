---
title: "BarcodeOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menginisialisasi instance baru dari kelas BarcodeOptionsgroupdocs.parser.options/barcodeoptions dengan nilai default."
type: docs
weight: 10
url: /id/net/groupdocs.parser.options/barcodeoptions/barcodeoptions/
---

## BarcodeOptions() {#constructor}

Menginisialisasi instance baru dari kelas [`BarcodeOptions`](../../barcodeoptions) dengan nilai default.

```csharp
public BarcodeOptions()
```

### Lihat Juga

* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle) {#constructor_1}

Menginisialisasi instance baru dari kelas [`BarcodeOptions`](../../barcodeoptions) dengan area persegi panjang.

```csharp
public BarcodeOptions(Rectangle rectangle)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| rectangle | Rectangle | Area persegi panjang yang berisi kode batang. |

### Lihat Juga

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(QualityMode, QualityMode, params string[]) {#constructor_3}

Menginisialisasi instance baru dari kelas [`BarcodeOptions`](../../barcodeoptions) dengan pengaturan kualitas dan tipe kode.

```csharp
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, 
    params string[] codeTypes)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| imageQuality | QualityMode | Kualitas gambar sumber. |
| barcodeQuality | QualityMode | Kualitas kode batang sumber. |
| codeTypes | String[] | Tipe kode batang yang akan dibaca. |

### Lihat Juga

* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) {#constructor_2}

Menginisialisasi instance baru dari kelas [`BarcodeOptions`](../../barcodeoptions).

```csharp
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, 
    float? dimension, bool allowIncorrectBarcodes, params string[] codeTypes)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| rectangle | Rectangle | Area persegi panjang yang berisi kode batang. |
| imageQuality | QualityMode | Kualitas gambar sumber. |
| barcodeQuality | QualityMode | Kualitas kode batang sumber. |
| dimension | Nullable`1 | Ukuran minimal dari elemen minimal kode batang. |
| allowIncorrectBarcodes | Boolean | Nilai yang menunjukkan apakah kode batang yang tidak tepat diizinkan. |
| codeTypes | String[] | Tipe kode batang yang akan dibaca. |

### Lihat Juga

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
