---
title: "Templat"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan templat halaman dokumen. Ini terdiri dari objek TemplateItem./templateitem yang mewakili item-item templat seperti bidang teks dan definisi tabel."
type: docs
weight: 50
url: /id/net/groupdocs.parser.templates/template/
---

## Template class

Menyediakan templat halaman dokumen. Ini terdiri dari objek [`TemplateItem`](../templateitem) yang mewakili item-item templat seperti bidang teks dan definisi tabel.

```csharp
public sealed class Template : IEnumerable<TemplateItem>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Template](template#constructor)(IEnumerable&lt;TemplateItem&gt;) | Menginisialisasi instance baru dari kelas [`Template`](../template). |
| [Template](template#constructor_1)(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) | Menginisialisasi instance baru dari kelas [`Template`](../template) dengan opsi templat. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../groupdocs.parser.templates/template/count) { get; } | Mendapatkan total jumlah item templat. |
| [IsOcrCompatible](../../groupdocs.parser.templates/template/isocrcompatible) { get; } | Mendapatkan nilai yang menunjukkan apakah templat kompatibel dengan OCR. |
| [Item](../../groupdocs.parser.templates/template/item) { get; } | Mendapatkan item templat berdasarkan indeks. |
| [Options](../../groupdocs.parser.templates/template/options) { get; } | Mendapatkan opsi templat. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [Load](../../groupdocs.parser.templates/template/load#load)(Stream) | Memuat templat dari aliran. |
| static [Load](../../groupdocs.parser.templates/template/load#load_1)(string) | Memuat templat dari file. |
| [GetEnumerator](../../groupdocs.parser.templates/template/getenumerator)() | Mengembalikan enumerator untuk item templat. |
| [Save](../../groupdocs.parser.templates/template/save#save)(Stream) | Menyimpan templat ke aliran. |
| [Save](../../groupdocs.parser.templates/template/save#save_1)(string) | Menyimpan templat ke file. |

### Catatan

**Learn more:**

* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)

### Lihat Juga

* class [TemplateItem](../templateitem)
* namespace [GroupDocs.Parser.Templates](../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
