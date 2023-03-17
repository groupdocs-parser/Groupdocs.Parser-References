---
title: PageTextAreaOptions
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Menginisialisasi instance baru dariPageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions kelas dengan opsi penggunaan OCR.
type: docs
weight: 10
url: /id/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---
## PageTextAreaOptions(bool) {#constructor}

Menginisialisasi instance baru dari[`PageTextAreaOptions`](../../pagetextareaoptions) kelas dengan opsi penggunaan OCR.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| useOcr | Boolean | Nilai yang menunjukkan apakah fungsionalitas OCR digunakan untuk mengekstrak area teks. |

### Lihat juga

* class [PageTextAreaOptions](../../pagetextareaoptions)
* ruang nama [GroupDocs.Parser.Options](../../pagetextareaoptions)
* perakitan [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_1}

Menginisialisasi instance baru dari[`PageTextAreaOptions`](../../pagetextareaoptions) kelas dengan kemampuan untuk menyetel opsi OCR.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| useOcr | Boolean | Nilai yang menunjukkan apakah fungsionalitas OCR digunakan untuk mengekstrak area teks. |
| ocrOptions | OcrOptions | Opsi tambahan untuk fungsionalitas OCR. |

### Lihat juga

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* ruang nama [GroupDocs.Parser.Options](../../pagetextareaoptions)
* perakitan [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_2}

Menginisialisasi instance baru dari[`PageTextAreaOptions`](../../pagetextareaoptions) kelas dengan ekspresi reguler. Opsi lain diatur secara default (lihat komentar untuk detailnya).

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| expression | String | Ekspresi reguler. |

### Perkataan

Properti berikut memiliki nilai default:

**[`MatchCase`](../matchcase)**

`PALSU`

**[`UniteSegments`](../unitesegments)**

`PALSU`

**[`IgnoreFormatting`](../ignoreformatting)**

`PALSU`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`batal`

### Lihat juga

* class [PageTextAreaOptions](../../pagetextareaoptions)
* ruang nama [GroupDocs.Parser.Options](../../pagetextareaoptions)
* perakitan [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_4}

Menginisialisasi instance baru dari[`PageTextAreaOptions`](../../pagetextareaoptions) class dengan ekspresi reguler dan area persegi panjang. Opsi lain diatur secara default (lihat komentar untuk detailnya).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| expression | String | Ekspresi reguler. |
| rectangle | Rectangle | Area persegi panjang yang berisi area halaman. |

### Perkataan

Properti berikut memiliki nilai default:

**[`MatchCase`](../matchcase)**

`PALSU`

**[`UniteSegments`](../unitesegments)**

`PALSU`

**[`IgnoreFormatting`](../ignoreformatting)**

`PALSU`

### Lihat juga

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* ruang nama [GroupDocs.Parser.Options](../../pagetextareaoptions)
* perakitan [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_3}

Menginisialisasi instance baru dari[`PageTextAreaOptions`](../../pagetextareaoptions) kelas.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| expression | String | Ekspresi reguler. |
| matchCase | Boolean | Nilai yang menunjukkan apakah kasus teks diabaikan. |
| uniteSegments | Boolean | Nilai yang menunjukkan apakah segmen bersatu. |
| ignoreFormatting | Boolean | Nilai yang menunjukkan apakah pemformatan teks diabaikan. |
| rectangle | Rectangle | Area persegi panjang yang berisi area halaman. |

### Lihat juga

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* ruang nama [GroupDocs.Parser.Options](../../pagetextareaoptions)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->