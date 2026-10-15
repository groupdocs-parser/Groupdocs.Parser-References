---
title: "PageRenderInfo"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mewakili informasi tentang bagaimana sebuah halaman dirender."
type: docs
weight: 500
url: /id/net/groupdocs.parser.options/pagerenderinfo/
---

## PageRenderInfo class

Mewakili informasi tentang bagaimana sebuah halaman dirender.

```csharp
public sealed class PageRenderInfo
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageRenderInfo](pagerenderinfo)(int, int, int) | Menginisialisasi sebuah instance baru dari kelas [`PageRenderInfo`](../pagerenderinfo). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ColumnCount](../../groupdocs.parser.options/pagerenderinfo/columncount) { get; } | Dapatkan total jumlah kolom ubin. |
| [PageNumber](../../groupdocs.parser.options/pagerenderinfo/pagenumber) { get; } | Mendapatkan nomor halaman. |
| [RowCount](../../groupdocs.parser.options/pagerenderinfo/rowcount) { get; } | Dapatkan total jumlah baris ubin. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetColumn](../../groupdocs.parser.options/pagerenderinfo/getcolumn)(int) | Mengembalikan indeks kolom tempat ubin dengan *tileIndex* ditempatkan. |
| [GetRow](../../groupdocs.parser.options/pagerenderinfo/getrow)(int) | Mengembalikan indeks baris tempat ubin dengan *tileIndex* ditempatkan. |

### Catatan

Beberapa dokumen (misalnya spreadsheet) tidak dapat merender halaman sebagai satu gambar tunggal. Untuk dokumen tersebut, halaman dirender sebagai sekumpulan ubin. Ubin-ubin ini ditempatkan dalam tabel persegi panjang.

[`RowCount`](./rowcount) and [`ColumnCount`](./columncount) represent the total number of rows and columns of this table. If document page is rendered to the single image these properties are equal to 1.

### Lihat Juga

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
