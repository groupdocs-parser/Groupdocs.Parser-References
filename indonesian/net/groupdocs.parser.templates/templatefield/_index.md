---
title: "TemplateField"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan bidang teks templat."
type: docs
weight: 80
url: /id/net/groupdocs.parser.templates/templatefield/
---

## TemplateField class

Menyediakan bidang teks templat.

```csharp
public sealed class TemplateField : TemplateItem
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TemplateField](templatefield#constructor)(TemplatePosition, string) | Menginisialisasi instance baru dari kelas [`TemplateField`](../templatefield). |
| [TemplateField](templatefield#constructor_1)(TemplatePosition, string, double?) | Menginisialisasi instance baru dari kelas [`TemplateField`](../templatefield). |
| [TemplateField](templatefield#constructor_2)(TemplatePosition, string, double?, bool) | Menginisialisasi instance baru dari kelas [`TemplateField`](../templatefield). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [IsHidden](../../groupdocs.parser.templates/templatefield/ishidden) { get; set; } | Mendapatkan atau mengatur flag bidang templat tersembunyi. |
| [Name](../../groupdocs.parser.templates/templateitem/name) { get; } | Mendapatkan nama item templat. |
| [PageWidth](../../groupdocs.parser.templates/templateitem/pagewidth) { get; } | Mendapatkan lebar halaman yang digunakan untuk membuat item templat. |
| [Position](../../groupdocs.parser.templates/templatefield/position) { get; } | Mendapatkan nilai yang menjelaskan cara menemukan bidang templat pada halaman dokumen. |
| [UseUpperCaseName](../../groupdocs.parser.templates/templateitem/useuppercasename) { get; } | Mendapatkan nilai boolean yang menunjukkan apakah sebuah `Name` telah diubah menjadi HURUF BESAR. |
| [Value](../../groupdocs.parser.templates/templatefield/value) { get; set; } | Mendapatkan atau mengatur nilai bidang templat. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Scale](../../groupdocs.parser.templates/templatefield/scale)(double) | Menskalakan item templat ini dengan faktor tertentu. |

### Catatan

Bidang teks didefinisikan oleh posisinya pada halaman. Ada tiga cara untuk mendefinisikan bidang teks:

* [`Using the rectangular area`](../templatefixedposition)
* [`Using the regular expression`](../templateregexposition)
* [`Using the linked field`](../templatelinkedposition)

### Lihat Juga

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
