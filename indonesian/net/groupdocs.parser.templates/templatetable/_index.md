---
title: "TemplateTable"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan tabel templat."
type: docs
weight: 160
url: /id/net/groupdocs.parser.templates/templatetable/
---

## TemplateTable class

Menyediakan tabel templat.

```csharp
public sealed class TemplateTable : TemplateItem
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TemplateTable](templatetable#constructor)(TemplateTableLayout, string) | Menginisialisasi instance baru dari kelas [`TemplateTable`](../templatetable) dengan nama HURUF BESAR. |
| [TemplateTable](templatetable#constructor_3)(TemplateTableParameters, string) | Menginisialisasi instance baru dari kelas [`TemplateTable`](../templatetable). |
| [TemplateTable](templatetable#constructor_1)(TemplateTableLayout, string, double?) | Menginisialisasi instance baru dari kelas [`TemplateTable`](../templatetable) dengan nama HURUF BESAR. |
| [TemplateTable](templatetable#constructor_4)(TemplateTableParameters, string, double?) | Menginisialisasi instance baru dari kelas [`TemplateTable`](../templatetable). |
| [TemplateTable](templatetable#constructor_2)(TemplateTableLayout, string, double?, bool) | Menginisialisasi instance baru dari kelas [`TemplateTable`](../templatetable). |
| [TemplateTable](templatetable#constructor_5)(TemplateTableParameters, string, double?, bool) | Menginisialisasi instance baru dari kelas [`TemplateTable`](../templatetable). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Layout](../../groupdocs.parser.templates/templatetable/layout) { get; } | Mendapatkan tata letak tabel. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Mendapatkan nama item templat. |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | Mendapatkan lebar halaman yang digunakan untuk membuat item templat. |
| [Parameters](../../groupdocs.parser.templates/templatetable/parameters) { get; } | Mendapatkan parameter untuk mendeteksi tabel dalam mode otomatis. |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | Mendapatkan nilai boolean yang menunjukkan apakah sebuah `Name` telah diubah menjadi HURUF BESAR. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatetable/scale)(double) | Menskalakan item templat ini dengan faktor tertentu. |

### Catatan

Ada dua cara untuk mendefinisikan tabel:

* Using [`TemplateTableLayout`](../templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [`TemplateTableParameters`](../templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [`TemplateTableParameters`](../templatetableparameters) class for more information.

### Lihat Juga

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
