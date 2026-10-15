---
title: "DocumentPageData"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mewakili data halaman dokumen. Terdiri dari objek FieldData./fielddata yang berisi data bidang dari halaman dokumen."
type: docs
weight: 740
url: /id/net/groupdocs.parser.data/documentpagedata/
---

## DocumentPageData class

Mewakili data halaman dokumen. Terdiri dari objek [`FieldData`](../fielddata) yang berisi data bidang dari halaman dokumen.

```csharp
public sealed class DocumentPageData : DocumentData
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Mendapatkan total jumlah data bidang. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Mendapatkan data bidang berdasarkan indeks. |
| [PageIndex](../../groupdocs.parser.data/documentpagedata/pageindex) { get; } | Mendapatkan indeks halaman. |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | Mendapatkan templat. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Mengembalikan enumerator untuk data bidang. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Mengembalikan koleksi data bidang dimana namanya sama dengan *fieldName*. |

### Lihat Juga

* class [DocumentData](../documentdata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
