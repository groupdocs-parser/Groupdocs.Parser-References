---
title: TemplateRegexPosition
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Memberikan posisi bidang template yang menggunakan ekspresi reguler.
type: docs
weight: 730
url: /id/net/groupdocs.parser.templates/templateregexposition/
---
## TemplateRegexPosition class

Memberikan posisi bidang template yang menggunakan ekspresi reguler.

```csharp
public sealed class TemplateRegexPosition : TemplatePosition
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [TemplateRegexPosition](templateregexposition#constructor)(string) | Menginisialisasi instance baru dari[`TemplateRegexPosition`](../templateregexposition) kelas. |
| [TemplateRegexPosition](templateregexposition#constructor_1)(string, bool) | Menginisialisasi instance baru dari[`TemplateRegexPosition`](../templateregexposition) kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Expression](../../groupdocs.parser.templates/templateregexposition/expression) { get; } | Mendapatkan ekspresi reguler. |
| [MatchCase](../../groupdocs.parser.templates/templateregexposition/matchcase) { get; } | Mendapat nilai yang menunjukkan apakah kasus teks tidak diabaikan. |

### Contoh

Contoh berikut menunjukkan situasi jika dokumen berisi "Nomor Faktur INV-12345" maka bidang template dapat ditentukan dengan cara berikut:

Dalam hal ini sebagai nilai, seluruh string diekstraksi. Untuk mengekstrak hanya sebagian dari string, "nilai" grup ekspresi reguler digunakan:

Dalam hal ini sebagai nilai string "INV-3337" diekstraksi.

```csharp
// Buat bidang template regex dengan nama "InvoiceNumber".
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
    "InvoiceNumber");
```

```csharp
// Buat bidang template regex dengan nama "InvoiceNumber" dengan grup "value".
TemplateField templateField = new TemplateField(
    new TemplateRegexPosition("Invoice Number\\s+(?<value>[A-Z0-9\\-]+)"),
    "InvoiceNumber");
```

### Lihat juga

* class [TemplatePosition](../templateposition)
* ruang nama [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* perakitan [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->