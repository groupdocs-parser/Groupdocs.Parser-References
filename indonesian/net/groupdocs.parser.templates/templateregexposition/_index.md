---
title: "TemplateRegexPosition"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan posisi bidang templat yang menggunakan ekspresi reguler."
type: docs
weight: 150
url: /id/net/groupdocs.parser.templates/templateregexposition/
---

## TemplateRegexPosition class

Menyediakan posisi bidang templat yang menggunakan ekspresi reguler.

```csharp
public sealed class TemplateRegexPosition : TemplatePosition
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TemplateRegexPosition](templateregexposition#constructor)(string) | Menginisialisasi instance baru dari kelas [`TemplateRegexPosition`](../templateregexposition). |
| [TemplateRegexPosition](templateregexposition#constructor_1)(string, bool) | Menginisialisasi instance baru dari kelas [`TemplateRegexPosition`](../templateregexposition). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Expression](../../groupdocs.parser.templates/templateregexposition/expression) { get; } | Mendapatkan ekspresi reguler. |
| [MatchCase](../../groupdocs.parser.templates/templateregexposition/matchcase) { get; } | Mendapatkan nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |

### Contoh

Contoh berikut menunjukkan situasi jika dokumen berisi "Invoice Number INV-12345" maka bidang templat dapat didefinisikan dengan cara berikut:

```csharp
// Buat bidang templat regex dengan nama "InvoiceNumber"
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
    "InvoiceNumber");
```

Dalam kasus ini, nilai yang diambil adalah seluruh string. Untuk mengekstrak hanya sebagian string, grup ekspresi reguler "value" digunakan:

```csharp
// Buat bidang templat regex dengan nama "InvoiceNumber" dengan grup "value"
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+(?<value>[A-Z0-9\\-]+)"),
    "InvoiceNumber");
```

Dalam kasus ini, string "INV-3337" diambil sebagai nilai.

### Lihat Juga

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
