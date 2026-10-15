---
title: "FromExtension"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Memetakan ekstensi berkas ke tipe berkas."
type: docs
weight: 930
url: /id/net/groupdocs.parser.options/filetype/fromextension/
---

## FileType.FromExtension method

Memetakan ekstensi berkas ke tipe berkas.

```csharp
public static FileType FromExtension(string extension)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| extension | String | Ekstensi file (termasuk titik "."). |

### Nilai Kembali

Ketika tipe file didukung, mengembalikannya; jika tidak, mengembalikan tipe file default [`Unknown`](../unknown).

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Dilemparkan ketika *extension* bernilai null atau string kosong. |

### Lihat Juga

* class [FileType](../../filetype)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
