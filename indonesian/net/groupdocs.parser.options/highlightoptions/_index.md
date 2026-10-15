---
title: "HighlightOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan opsi yang digunakan untuk mengekstrak sorotan sebuah blok teks di sekitar teks yang ditemukan dalam skenario pencarian."
type: docs
weight: 360
url: /id/net/groupdocs.parser.options/highlightoptions/
---

## HighlightOptions class

Menyediakan opsi yang digunakan untuk mengekstrak sorotan (sebuah blok teks di sekitar teks yang ditemukan dalam skenario pencarian).

```csharp
public sealed class HighlightOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [HighlightOptions](highlightoptions#constructor)() | Menginisialisasi sebuah instance baru dari kelas [`HighlightOptions`](../highlightoptions) yang digunakan untuk mengekstrak sorotan dengan panjang tetap. |
| [HighlightOptions](highlightoptions#constructor_1)(int) | Menginisialisasi sebuah instance baru dari kelas [`HighlightOptions`](../highlightoptions) yang digunakan untuk mengekstrak sorotan dengan panjang tetap. |
| [HighlightOptions](highlightoptions#constructor_2)(int?, bool) | Menginisialisasi sebuah instance baru dari kelas [`HighlightOptions`](../highlightoptions) yang digunakan untuk mengekstrak sorotan dengan batas baris. |
| [HighlightOptions](highlightoptions#constructor_3)(int?, int) | Menginisialisasi sebuah instance baru dari kelas [`HighlightOptions`](../highlightoptions) yang digunakan untuk mengekstrak sorotan dengan jumlah kata tetap. |
| [HighlightOptions](highlightoptions#constructor_4)(int?, int?, bool) | Menginisialisasi sebuah instance baru dari kelas [`HighlightOptions`](../highlightoptions). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [IsLineLimited](../../groupdocs.parser.options/highlightoptions/islinelimited) { get; set; } | Mendapatkan nilai yang menunjukkan apakah ekstraksi sorotan dibatasi oleh awal (atau akhir) baris teks. |
| [MaxLength](../../groupdocs.parser.options/highlightoptions/maxlength) { get; set; } | Mendapatkan panjang teks maksimum. |
| [WordCount](../../groupdocs.parser.options/highlightoptions/wordcount) { get; set; } | Mendapatkan jumlah kata maksimum. |

### Catatan

Sebuah instance dari kelas [`HighlightOptions`](../highlightoptions) digunakan sebagai parameter dalam metode [`GetHighlight`](../../groupdocs.parser/parser/gethighlight). Lihat contoh penggunaan di sana.

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### Lihat Juga

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
