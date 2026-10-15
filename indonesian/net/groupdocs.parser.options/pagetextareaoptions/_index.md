---
title: "PageTextAreaOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan opsi yang digunakan untuk ekstraksi area teks halaman."
type: docs
weight: 520
url: /id/net/groupdocs.parser.options/pagetextareaoptions/
---

## PageTextAreaOptions class

Menyediakan opsi yang digunakan untuk ekstraksi area teks halaman.

```csharp
public sealed class PageTextAreaOptions : PageAreaOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageTextAreaOptions](pagetextareaoptions#constructor)() | Menginisialisasi sebuah instance baru dari kelas [`PageTextAreaOptions`](../pagetextareaoptions) dengan opsi penggunaan OCR. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_1)(bool) | Menginisialisasi sebuah instance baru dari kelas [`PageTextAreaOptions`](../pagetextareaoptions) dengan opsi penggunaan OCR. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_3)(string) | Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../pagetextareaoptions) dengan ekspresi reguler. Opsi lain diatur secara default (lihat catatan untuk detail). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_2)(bool, OcrOptions) | Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../pagetextareaoptions) dengan kemampuan untuk mengatur opsi OCR. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_6)(string, Rectangle) | Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../pagetextareaoptions) dengan ekspresi reguler dan area persegi panjang. Opsi lain diatur secara default (lihat catatan untuk detail). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_7)(string, Rectangle, double) | Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../pagetextareaoptions) dengan ekspresi reguler, area persegi panjang, dan ukuran batas yang diabaikan. Opsi lain diatur secara default (lihat catatan untuk detail). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_4)(string, bool, bool, bool, Rectangle) | Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../pagetextareaoptions). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_5)(string, bool, bool, bool, Rectangle, double) | Menginisialisasi instance baru dari kelas [`PageTextAreaOptions`](../pagetextareaoptions) dengan ukuran batas yang diabaikan. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Expression](../../groupdocs.parser.options/pagetextareaoptions/expression) { get; set; } | Mendapatkan ekspresi reguler. |
| [IgnoreFormatting](../../groupdocs.parser.options/pagetextareaoptions/ignoreformatting) { get; set; } | Mendapatkan nilai yang menunjukkan apakah pemformatan teks diabaikan. |
| [MatchCase](../../groupdocs.parser.options/pagetextareaoptions/matchcase) { get; set; } | Mendapatkan nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
| [OcrOptions](../../groupdocs.parser.options/pagetextareaoptions/ocroptions) { get; set; } | Mendapatkan opsi tambahan untuk fungsionalitas OCR. |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Mendapatkan area persegi panjang yang berisi area halaman. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Mendapatkan ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. Diukur dengan fraksi tinggi item teks. |
| [UniteSegments](../../groupdocs.parser.options/pagetextareaoptions/unitesegments) { get; set; } | Mendapatkan nilai yang menunjukkan apakah segmen digabungkan. |
| [UseOcr](../../groupdocs.parser.options/pagetextareaoptions/useocr) { get; set; } | Mendapatkan nilai yang menunjukkan apakah fungsi OCR digunakan untuk mengekstrak area teks. |

### Catatan

Sebuah instance dari kelas [`PageTextAreaOptions`](../pagetextareaoptions) digunakan sebagai parameter dalam metode [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) dan [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas). Lihat contoh penggunaan di sana. **Pelajari lebih lanjut:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Lihat Juga

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
