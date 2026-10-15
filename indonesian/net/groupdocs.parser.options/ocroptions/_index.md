---
title: "OcrOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan opsi yang digunakan untuk OCR Connector."
type: docs
weight: 450
url: /id/net/groupdocs.parser.options/ocroptions/
---

## OcrOptions class

Menyediakan opsi yang digunakan untuk OCR Connector.

```csharp
public class OcrOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [OcrOptions](ocroptions#constructor)() | Menginisialisasi instance baru dari kelas [`OcrOptions`](../ocroptions) dengan area persegi panjang. |
| [OcrOptions](ocroptions#constructor_5)(OcrEventHandler) | Menginisialisasi instance baru dari kelas [`OcrOptions`](../ocroptions) dengan objek [`OcrEventHandler`](../ocreventhandler). |
| [OcrOptions](ocroptions#constructor_6)(PagePreviewOptions) | Menginisialisasi instance baru dari kelas [`OcrOptions`](../ocroptions) dengan area persegi panjang. |
| [OcrOptions](ocroptions#constructor_1)(Rectangle) | Menginisialisasi instance baru dari kelas [`OcrOptions`](../ocroptions) dengan area persegi panjang. |
| [OcrOptions](ocroptions#constructor_2)(Rectangle, OcrEventHandler) | Menginisialisasi instance baru dari kelas [`OcrOptions`](../ocroptions) dengan area persegi panjang dan objek [`OcrEventHandler`](../ocreventhandler). |
| [OcrOptions](ocroptions#constructor_3)(Rectangle, OcrEventHandler, PagePreviewOptions, bool) | Menginisialisasi instance baru dari kelas [`OcrOptions`](../ocroptions). |
| [OcrOptions](ocroptions#constructor_4)(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) | Menginisialisasi instance baru dari kelas [`OcrOptions`](../ocroptions). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Handler](../../groupdocs.parser.options/ocroptions/handler) { get; set; } | Mendapatkan penangan peristiwa untuk menangkap peristiwa OCR. |
| [Language](../../groupdocs.parser.options/ocroptions/language) { get; set; } | Mendapatkan atau mengatur bahasa yang digunakan untuk OCR. Menentukan alfabet yang dipakai selama pengenalan. Bahasa Inggris digunakan secara default. |
| [PagePreviewOptions](../../groupdocs.parser.options/ocroptions/pagepreviewoptions) { get; set; } | Mendapatkan opsi pratinjau halaman dokumen. |
| [Rectangle](../../groupdocs.parser.options/ocroptions/rectangle) { get; set; } | Mendapatkan area persegi panjang yang membatasi area halaman yang digunakan untuk pengenalan teks. |
| [UseSpellChecker](../../groupdocs.parser.options/ocroptions/usespellchecker) { get; set; } | Mendapatkan nilai yang menunjukkan apakah pemeriksa ejaan digunakan. |

### Lihat Juga

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
