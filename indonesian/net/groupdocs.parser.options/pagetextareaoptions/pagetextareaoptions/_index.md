---
title: "PageTextAreaOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menginisialisasi instance baru dari kelas PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions dengan opsi penggunaan OCR."
type: docs
weight: 10
url: /id/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../../pagetextareaoptions) dengan opsi penggunaan OCR.

```csharp
public PageTextAreaOptions()
```

### Lihat Juga

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../../pagetextareaoptions) dengan opsi penggunaan OCR.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| useOcr | Boolean | Nilai yang menunjukkan apakah fungsi OCR digunakan untuk mengekstrak area teks. |

### Lihat Juga

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../../pagetextareaoptions) dengan kemampuan mengatur opsi OCR.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| useOcr | Boolean | Nilai yang menunjukkan apakah fungsi OCR digunakan untuk mengekstrak area teks. |
| ocrOptions | OcrOptions | Opsi tambahan untuk fungsi OCR. |

### Lihat Juga

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../../pagetextareaoptions) dengan ekspresi reguler. Opsi lain diatur secara default (lihat catatan untuk detail).

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| expression | String | Ekspresi reguler. |

### Catatan

Properti berikut memiliki nilai default:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### Lihat Juga

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../../pagetextareaoptions) dengan ekspresi reguler dan area persegi panjang. Opsi lain diatur secara default (lihat catatan untuk detail).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| expression | String | Ekspresi reguler. |
| rectangle | Rectangle | Area persegi panjang yang berisi area halaman. |

### Catatan

Properti berikut memiliki nilai default:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### Lihat Juga

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../../pagetextareaoptions) dengan ekspresi reguler, area persegi panjang, dan ukuran batas yang diabaikan. Opsi lain diatur secara default (lihat catatan untuk detail).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| expression | String | Ekspresi reguler. |
| rectangle | Rectangle | Area persegi panjang yang berisi area halaman. |
| rectangleTolerance | Double | Ukuran batas yang diabaikan saat ditangkap oleh area persegi panjang. Diukur sebagai fraksi dari tinggi item teks. |

### Lihat Juga

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../../pagetextareaoptions).

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| expression | String | Ekspresi reguler. |
| matchCase | Boolean | Nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| uniteSegments | Boolean | Nilai yang menunjukkan apakah segmen digabungkan. |
| ignoreFormatting | Boolean | Nilai yang menunjukkan apakah pemformatan teks diabaikan. |
| rectangle | Rectangle | Area persegi panjang yang berisi area halaman. |

### Lihat Juga

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../../pagetextareaoptions) dengan ukuran batas yang diabaikan.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| expression | String | Ekspresi reguler. |
| matchCase | Boolean | Nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| uniteSegments | Boolean | Nilai yang menunjukkan apakah segmen digabungkan. |
| ignoreFormatting | Boolean | Nilai yang menunjukkan apakah pemformatan teks diabaikan. |
| rectangle | Rectangle | Area persegi panjang yang berisi area halaman. |
| rectangleTolerance | Double | Ukuran batas yang diabaikan saat ditangkap oleh area persegi panjang. Diukur sebagai fraksi dari tinggi item teks. |

### Lihat Juga

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
