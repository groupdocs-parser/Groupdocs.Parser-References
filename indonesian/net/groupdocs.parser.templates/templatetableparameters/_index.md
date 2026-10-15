---
title: "TemplateTableParameters"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan parameter untuk algoritma deteksi tabel."
type: docs
weight: 180
url: /id/net/groupdocs.parser.templates/templatetableparameters/
---

## TemplateTableParameters class

Menyediakan parameter untuk algoritma deteksi tabel.

```csharp
public sealed class TemplateTableParameters
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TemplateTableParameters](templatetableparameters#constructor)(Rectangle, IEnumerable&lt;double&gt;) | Menginisialisasi instance baru dari kelas [`TemplateTableParameters`](../templatetableparameters). |
| [TemplateTableParameters](templatetableparameters#constructor_1)(Rectangle, IEnumerable&lt;double&gt;, bool?, int?, int?, int?) | Menginisialisasi instance baru dari kelas [`TemplateTableParameters`](../templatetableparameters). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [HasMergedCells](../../groupdocs.parser.templates/templatetableparameters/hasmergedcells) { get; } | Mendapatkan nilai yang menunjukkan apakah tabel memiliki sel yang digabung. |
| [MinColumnCount](../../groupdocs.parser.templates/templatetableparameters/mincolumncount) { get; } | Mendapatkan jumlah minimum kolom tabel. |
| [MinRowCount](../../groupdocs.parser.templates/templatetableparameters/minrowcount) { get; } | Mendapatkan jumlah minimum baris tabel. |
| [MinVerticalSpace](../../groupdocs.parser.templates/templatetableparameters/minverticalspace) { get; } | Mendapatkan jarak minimum antara kolom tabel. |
| [Rectangle](../../groupdocs.parser.templates/templatetableparameters/rectangle) { get; } | Mendapatkan area persegi panjang yang berisi tabel. |
| [VerticalSeparators](../../groupdocs.parser.templates/templatetableparameters/verticalseparators) { get; } | Mendapatkan pemisah kolom tabel. |

### Catatan

Ada dua algoritma untuk mendeteksi tabel:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

Dalam beberapa kasus ketika algoritma tidak dapat mendeteksi tabel atau melakukannya secara tidak akurat, kelas [`TemplateTableLayout`](../templatetablelayout) digunakan.

### Lihat Juga

* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
