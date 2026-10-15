---
title: "TemplateLinkedPosition"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan posisi bidang templat yang menggunakan bidang yang ditautkan."
type: docs
weight: 110
url: /id/net/groupdocs.parser.templates/templatelinkedposition/
---

## TemplateLinkedPosition class

Menyediakan posisi bidang templat yang menggunakan bidang yang ditautkan.

```csharp
public sealed class TemplateLinkedPosition : TemplatePosition
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TemplateLinkedPosition](templatelinkedposition#constructor)(string, Size, TemplateLinkedPositionEdges) | Menginisialisasi instance baru dari kelas [`TemplateLinkedPosition`](../templatelinkedposition). |
| [TemplateLinkedPosition](templatelinkedposition#constructor_1)(string, Size, TemplateLinkedPositionEdges, bool) | Menginisialisasi instance baru dari kelas [`TemplateLinkedPosition`](../templatelinkedposition) dengan nama bidang tertaut HURUF BESAR. |
| [TemplateLinkedPosition](templatelinkedposition#constructor_2)(string, Size, TemplateLinkedPositionEdges, bool, bool) | Menginisialisasi instance baru dari kelas [`TemplateLinkedPosition`](../templatelinkedposition). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AutoScale](../../groupdocs.parser.templates/templatelinkedposition/autoscale) { get; } | Mendapatkan nilai yang menunjukkan apakah [`SearchArea`](./searcharea) diskalakan oleh ukuran bidang tertaut. |
| [Edges](../../groupdocs.parser.templates/templatelinkedposition/edges) { get; } | Mendapatkan tepi bidang tertaut tempat bidang dicari. |
| [LinkedFieldName](../../groupdocs.parser.templates/templatelinkedposition/linkedfieldname) { get; } | Mendapatkan nama bidang tertaut. |
| [SearchArea](../../groupdocs.parser.templates/templatelinkedposition/searcharea) { get; } | Mendapatkan ukuran area tempat bidang dicari. |

### Contoh

Contoh berikut menunjukkan kode untuk situasi jika diketahui bahwa bidang dengan nomor faktur ditempatkan di sebelah kanan string "Invoice number", kode berikut digunakan:

```csharp
// Buat bidang templat regex untuk menemukan teks "Invoice Number"
TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

// Buat bidang templat terkait yang berhubungan dengan bidang "Invoice" dan ekstrak nilai di sebelah kanannya
TemplateField invoiceNumber = new TemplateField(
    new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
    "InvoiceNumber");
```

### Lihat Juga

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
