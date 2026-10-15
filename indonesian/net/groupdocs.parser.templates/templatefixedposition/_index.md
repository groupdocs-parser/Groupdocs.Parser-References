---
title: "TemplateFixedPosition"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan posisi bidang templat yang didefinisikan oleh area persegi panjang."
type: docs
weight: 90
url: /id/net/groupdocs.parser.templates/templatefixedposition/
---

## TemplateFixedPosition class

Menyediakan posisi bidang templat yang didefinisikan oleh area persegi panjang.

```csharp
public sealed class TemplateFixedPosition : TemplatePosition
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TemplateFixedPosition](templatefixedposition)(Rectangle) | Menginisialisasi instance baru dari kelas [`TemplateFixedPosition`](../templatefixedposition). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Rectangle](../../groupdocs.parser.templates/templatefixedposition/rectangle) { get; } | Mendapatkan area persegi panjang yang berisi bidang templat. |

### Contoh

Ini adalah cara paling sederhana untuk mendefinisikan posisi bidang. Dibutuhkan penetapan area persegi panjang pada halaman yang membatasi nilai bidang. Semua teks yang terkandung (bahkan sebagian) dalam area persegi panjang akan diekstrak sebagai nilai:

```csharp
// Buat bidang templat tetap dengan nama "Address" yang dibatasi oleh persegi panjang pada posisi (35, 160) dan dengan ukuran (110, 20)
TemplateField templateField = new TemplateField(
    new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
    "Address");
```

### Lihat Juga

* class [TemplatePosition](../templateposition)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
