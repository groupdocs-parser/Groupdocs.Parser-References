---
title: "TextOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan opsi yang digunakan untuk ekstraksi teks."
type: docs
weight: 610
url: /id/net/groupdocs.parser.options/textoptions/
---

## TextOptions class

Menyediakan opsi yang digunakan untuk ekstraksi teks.

```csharp
public sealed class TextOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TextOptions](textoptions#constructor)() | Menginisialisasi instance baru dari kelas [`TextOptions`](../textoptions). |
| [TextOptions](textoptions#constructor_1)(bool) | Menginisialisasi instance baru dari kelas [`TextOptions`](../textoptions). |
| [TextOptions](textoptions#constructor_2)(bool, bool) | Menginisialisasi instance baru dari kelas [`TextOptions`](../textoptions) dengan opsi penggunaan OCR. |
| [TextOptions](textoptions#constructor_3)(bool, bool, OcrOptions) | Menginisialisasi instance baru dari kelas [`TextOptions`](../textoptions) dengan kemampuan untuk mengatur opsi OCR. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [IncludeAnnotations](../../groupdocs.parser.options/textoptions/includeannotations) { get; set; } | Mendapatkan nilai yang menunjukkan apakah anotasi disertakan. Nilai default adalah `false`. |
| [OcrOptions](../../groupdocs.parser.options/textoptions/ocroptions) { get; set; } | Mendapatkan opsi tambahan untuk fungsionalitas OCR. |
| [UseOcr](../../groupdocs.parser.options/textoptions/useocr) { get; set; } | Mendapatkan nilai yang menunjukkan apakah OCR Connector digunakan untuk mengekstrak teks. |
| [UseRawModeIfPossible](../../groupdocs.parser.options/textoptions/userawmodeifpossible) { get; set; } | Mendapatkan nilai yang menunjukkan apakah mode mentah digunakan. |

### Catatan

Sebuah instance dari kelas [`TextOptions`](../textoptions) digunakan sebagai parameter dalam metode [`GetText`](../../groupdocs.parser/parser/gettext) dan [`GetText`](../../groupdocs.parser/parser/gettext). Lihat contoh penggunaan di sana.

Ini digunakan untuk menentukan mode mentah ekstraksi teks. Teks dalam mode ini diekstrak secara tidak akurat tetapi lebih cepat dibandingkan mode standar. Jika mode mentah tidak mendukung format dokumen, maka parameter ini diabaikan dan mode standar digunakan.

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Lihat Juga

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
