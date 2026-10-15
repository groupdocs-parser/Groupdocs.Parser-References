---
title: "SearchOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menginisialisasi sebuah instansi baru dari kelas SearchOptionsgroupdocs.parser.options/searchoptions."
type: docs
weight: 10
url: /id/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Menginisialisasi sebuah instansi baru dari kelas [`SearchOptions`](../../searchoptions).

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
| searchByPages | Boolean | Nilai yang menunjukkan apakah pencarian dilakukan per halaman. |
| leftHighlightOptions | HighlightOptions | Opsi untuk penyorotan kiri. |
| rightHighlightOptions | HighlightOptions | Opsi untuk penyorotan kanan. |

### Lihat Juga

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

Menginisialisasi instance baru dari kelas [`SearchOptions`](../../searchoptions) dengan batas halaman.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
| maxPageIndex | Int32 | Nilai yang menunjukkan apakah pencarian dilakukan per halaman. |
| leftHighlightOptions | HighlightOptions | Opsi untuk penyorotan kiri. |
| rightHighlightOptions | HighlightOptions | Opsi untuk penyorotan kanan. |

### Lihat Juga

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Menginisialisasi instance baru dari kelas [`SearchOptions`](../../searchoptions) yang digunakan untuk mencari dengan opsi penyorotan untuk ekstraksi penyorotan kiri dan kanan.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
| leftHighlightOptions | HighlightOptions | Opsi untuk penyorotan kiri. |
| rightHighlightOptions | HighlightOptions | Opsi untuk penyorotan kanan. |

### Lihat Juga

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Menginisialisasi instance baru dari kelas [`SearchOptions`](../../searchoptions) yang digunakan untuk mencari dengan opsi penyorotan yang sama untuk ekstraksi penyorotan kiri dan kanan.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
| highlightOptions | HighlightOptions | Opsi untuk kedua penyorotan. |

### Lihat Juga

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Menginisialisasi instance baru dari kelas [`SearchOptions`](../../searchoptions) yang digunakan untuk mencari tanpa ekstraksi penyorotan.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |

### Lihat Juga

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Menginisialisasi instance baru dari kelas [`SearchOptions`](../../searchoptions) yang digunakan untuk mencari per halaman dan tanpa ekstraksi penyorotan.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
| searchByPages | Boolean | Nilai yang menunjukkan apakah pencarian dilakukan per halaman. |

### Lihat Juga

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Menginisialisasi instance baru dari kelas [`SearchOptions`](../../searchoptions) dengan nilai default. Lihat catatan untuk detail.

```csharp
public SearchOptions()
```

### Catatan

Properti berikut memiliki nilai default:

**[`MatchCase`](../matchcase)**

`false`

**[`MatchWholeWord`](../matchwholeword)**

`false`

**[`UseRegularExpression`](../useregularexpression)**

`false`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### Lihat Juga

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
