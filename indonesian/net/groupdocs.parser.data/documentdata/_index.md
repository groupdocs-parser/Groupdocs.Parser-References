---
title: "DocumentData"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mewakili data dokumen. Ini terdiri dari objek FieldData./fielddata yang berisi data bidang dari dokumen."
type: docs
weight: 730
url: /id/net/groupdocs.parser.data/documentdata/
---

## DocumentData class

Mewakili data dokumen. Ini terdiri dari objek [`FieldData`](../fielddata) yang berisi data bidang dari dokumen.

```csharp
public class DocumentData : IEnumerable<FieldData>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Mendapatkan total jumlah data bidang. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Mendapatkan data bidang berdasarkan indeks. |
| [Template](../../groupdocs.parser.data/documentdata/template) { get; } | Mendapatkan templat. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Mengembalikan enumerator untuk data bidang. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Mengembalikan koleksi data bidang dimana namanya sama dengan *fieldName*. |

### Catatan

Sebuah instance dari kelas [`DocumentData`](../documentdata) digunakan sebagai nilai kembali dari metode [`ParseByTemplate`](../../groupdocs.parser/parser/parsebytemplate) dan [`ParseForm`](../../groupdocs.parser/parser/parseform). Lihat contoh penggunaan di sana.

### Lihat Juga

* class [FieldData](../fielddata)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
