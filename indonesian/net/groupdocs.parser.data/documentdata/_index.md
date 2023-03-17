---
title: DocumentData
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Mewakili data dokumen. Terdiri dariFieldData./fielddataobjek yang berisi data lapangan dari dokumen.
type: docs
weight: 20
url: /id/net/groupdocs.parser.data/documentdata/
---
## DocumentData class

Mewakili data dokumen. Terdiri dari[`FieldData`](../fielddata)objek yang berisi data lapangan dari dokumen.

```csharp
public class DocumentData : IEnumerable<FieldData>
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [DocumentData](documentdata)(IEnumerable&lt;FieldData&gt;) | Menginisialisasi instance baru dari[`FieldData`](../fielddata) kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Count](../../groupdocs.parser.data/documentdata/count) { get; } | Mendapat jumlah total data bidang. |
| [Item](../../groupdocs.parser.data/documentdata/item) { get; } | Mendapatkan data lapangan dengan indeks. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [GetEnumerator](../../groupdocs.parser.data/documentdata/getenumerator)() | Mengembalikan pencacah untuk data bidang. |
| [GetFieldsByName](../../groupdocs.parser.data/documentdata/getfieldsbyname)(string) | Mengembalikan kumpulan data bidang yang namanya sama dengan*fieldName* . |

### Perkataan

Contoh dari[`DocumentData`](../documentdata) kelas digunakan sebagai nilai kembalian dari[`ParseByTemplate`](../../groupdocs.parser/parser/parsebytemplate) Dan[`ParseForm`](../../groupdocs.parser/parser/parseform) metode. Lihat contoh penggunaan di sana.

### Lihat juga

* class [FieldData](../fielddata)
* ruang nama [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* perakitan [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->