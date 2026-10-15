---
title: "SearchOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan opsi yang digunakan untuk pencarian teks."
type: docs
weight: 590
url: /id/net/groupdocs.parser.options/searchoptions/
---

## SearchOptions class

Menyediakan opsi yang digunakan untuk pencarian teks.

```csharp
public sealed class SearchOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [SearchOptions](searchoptions#constructor)() | Menginisialisasi instance baru dari kelas [`SearchOptions`](../searchoptions) dengan nilai default. Lihat catatan untuk detail. |
| [SearchOptions](searchoptions#constructor_1)(bool, bool, bool) | Menginisialisasi instance baru dari kelas [`SearchOptions`](../searchoptions) yang digunakan untuk mencari tanpa ekstraksi penyorotan. |
| [SearchOptions](searchoptions#constructor_2)(bool, bool, bool, bool) | Menginisialisasi instance baru dari kelas [`SearchOptions`](../searchoptions) yang digunakan untuk mencari berdasarkan halaman dan tanpa ekstraksi penyorotan. |
| [SearchOptions](searchoptions#constructor_4)(bool, bool, bool, HighlightOptions) | Menginisialisasi instance baru dari kelas [`SearchOptions`](../searchoptions) yang digunakan untuk mencari dengan opsi penyorotan yang sama untuk ekstraksi penyorotan kiri dan kanan. |
| [SearchOptions](searchoptions#constructor_5)(bool, bool, bool, HighlightOptions, HighlightOptions) | Menginisialisasi instance baru dari kelas [`SearchOptions`](../searchoptions) yang digunakan untuk mencari dengan opsi penyorotan untuk ekstraksi penyorotan kiri dan kanan. |
| [SearchOptions](searchoptions#constructor_3)(bool, bool, bool, bool, HighlightOptions, HighlightOptions) | Menginisialisasi instance baru dari kelas [`SearchOptions`](../searchoptions). |
| [SearchOptions](searchoptions#constructor_6)(bool, bool, bool, int, HighlightOptions, HighlightOptions) | Menginisialisasi instance baru dari kelas [`SearchOptions`](../searchoptions) dengan batas halaman. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [LeftHighlightOptions](../../groupdocs.parser.options/searchoptions/lefthighlightoptions) { get; set; } | Mendapatkan opsi untuk penyorotan kiri. |
| [MatchCase](../../groupdocs.parser.options/searchoptions/matchcase) { get; set; } | Mendapatkan nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| [MatchWholeWord](../../groupdocs.parser.options/searchoptions/matchwholeword) { get; set; } | Mendapatkan nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
| [MaxPageIndex](../../groupdocs.parser.options/searchoptions/maxpageindex) { get; set; } | Mendapatkan nilai yang mewakili indeks maksimum halaman yang akan dicari. |
| [RightHighlightOptions](../../groupdocs.parser.options/searchoptions/righthighlightoptions) { get; set; } | Mendapatkan opsi untuk penyorotan kanan. |
| [SearchByPages](../../groupdocs.parser.options/searchoptions/searchbypages) { get; set; } | Mendapatkan nilai yang menunjukkan apakah pencarian dilakukan per halaman. |
| [UseRegularExpression](../../groupdocs.parser.options/searchoptions/useregularexpression) { get; set; } | Mendapatkan nilai yang menunjukkan apakah ekspresi reguler digunakan. |

### Catatan

Sebuah instance dari kelas [`SearchOptions`](../searchoptions) digunakan sebagai parameter dalam metode [`Search`](../../groupdocs.parser/parser/search). Lihat contoh penggunaan di sana.

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Lihat Juga

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
