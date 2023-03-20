---
title: SearchOptions
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Menginisialisasi instance baru dariSearchOptionsgroupdocs.parser.options/searchoptions kelas.
type: docs
weight: 10
url: /id/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Menginisialisasi instance baru dari[`SearchOptions`](../../searchoptions) kelas.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kasus teks diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh seluruh kata. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
| searchByPages | Boolean | Nilai yang menunjukkan apakah penelusuran dilakukan oleh laman. |
| leftHighlightOptions | HighlightOptions | Opsi untuk sorotan kiri. |
| rightHighlightOptions | HighlightOptions | Opsi untuk sorotan yang tepat. |

### Lihat juga

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* ruang nama [GroupDocs.Parser.Options](../../searchoptions)
* perakitan [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Menginisialisasi instance baru dari[`SearchOptions`](../../searchoptions) kelas yang digunakan untuk mencari dengan opsi sorotan untuk ekstraksi sorotan kiri dan kanan.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kasus teks diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh seluruh kata. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
| leftHighlightOptions | HighlightOptions | Opsi untuk sorotan kiri. |
| rightHighlightOptions | HighlightOptions | Opsi untuk sorotan yang tepat. |

### Lihat juga

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* ruang nama [GroupDocs.Parser.Options](../../searchoptions)
* perakitan [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Menginisialisasi instance baru dari[`SearchOptions`](../../searchoptions) kelas yang digunakan untuk mencari dengan opsi sorotan yang sama untuk ekstraksi sorotan kiri dan kanan.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kasus teks diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh seluruh kata. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
| highlightOptions | HighlightOptions | Opsi untuk kedua highlight. |

### Lihat juga

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* ruang nama [GroupDocs.Parser.Options](../../searchoptions)
* perakitan [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Menginisialisasi instance baru dari[`SearchOptions`](../../searchoptions) kelas yang digunakan untuk mencari tanpa menyorot ekstraksi.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kasus teks diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh seluruh kata. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |

### Lihat juga

* class [SearchOptions](../../searchoptions)
* ruang nama [GroupDocs.Parser.Options](../../searchoptions)
* perakitan [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Menginisialisasi instance baru dari[`SearchOptions`](../../searchoptions)kelas yang digunakan untuk mencari berdasarkan halaman dan tanpa ekstraksi sorot.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| matchCase | Boolean | Nilai yang menunjukkan apakah kasus teks diabaikan. |
| matchWholeWord | Boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh seluruh kata. |
| useRegularExpression | Boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
| searchByPages | Boolean | Nilai yang menunjukkan apakah penelusuran dilakukan oleh laman. |

### Lihat juga

* class [SearchOptions](../../searchoptions)
* ruang nama [GroupDocs.Parser.Options](../../searchoptions)
* perakitan [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Menginisialisasi instance baru dari[`SearchOptions`](../../searchoptions) kelas dengan nilai default. Lihat komentar untuk detailnya.

```csharp
public SearchOptions()
```

### Perkataan

Properti berikut memiliki nilai default:

**[`MatchCase`](../matchcase)**

`PALSU`

**[`MatchWholeWord`](../matchwholeword)**

`PALSU`

**[`UseRegularExpression`](../useregularexpression)**

`PALSU`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`batal`

**[`RightHighlightOptions`](../righthighlightoptions)**

`batal`

### Lihat juga

* class [SearchOptions](../../searchoptions)
* ruang nama [GroupDocs.Parser.Options](../../searchoptions)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
