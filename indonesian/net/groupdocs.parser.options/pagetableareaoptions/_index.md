---
title: "PageTableAreaOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan opsi yang digunakan untuk ekstraksi area tabel halaman."
type: docs
weight: 510
url: /id/net/groupdocs.parser.options/pagetableareaoptions/
---

## PageTableAreaOptions class

Menyediakan opsi yang digunakan untuk ekstraksi area tabel halaman.

```csharp
public sealed class PageTableAreaOptions : PageAreaOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageTableAreaOptions](pagetableareaoptions)(TemplateTableLayout) | Menginisialisasi instance baru dari kelas [`PageAreaOptions`](../pageareaoptions). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; set; } | Mendapatkan area persegi panjang yang berisi area halaman. |
| [RectangleTolerance](../../groupdocs.parser.options/pageareaoptions/rectangletolerance) { get; set; } | Mendapatkan ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. Diukur dengan fraksi tinggi item teks. |
| [TableLayout](../../groupdocs.parser.options/pagetableareaoptions/tablelayout) { get; } | Mendapatkan tata letak tabel yang mendefinisikan tabel pada halaman. |

### Catatan

Sebuah instance dari kelas [`PageTableAreaOptions`](../pagetableareaoptions) digunakan sebagai parameter dalam metode [`GetTables`](../../groupdocs.parser/parser/gettables) dan [`GetTables`](../../groupdocs.parser/parser/gettables). Lihat contoh penggunaan di sana.

### Lihat Juga

* class [PageAreaOptions](../pageareaoptions)
* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
