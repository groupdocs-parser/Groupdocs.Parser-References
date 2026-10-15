---
title: "RawPageCount"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mendapatkan total jumlah halaman mentah dokumen."
type: docs
weight: 40
url: /id/net/groupdocs.parser.options/idocumentinfo/rawpagecount/
---

## IDocumentInfo.RawPageCount property

Mendapatkan total jumlah halaman mentah dokumen.

```csharp
public int RawPageCount { get; }
```

### Property Value

Nilai integer yang mewakili total jumlah halaman mentah.

### Catatan

Gunakan properti `RawPageCount` alih-alih properti [`PageCount`](../pagecount) untuk ekstraksi teks mentah. Beberapa dokumen memiliki nomor halaman yang berbeda dalam mode ekstraksi teks akurat dan mentah. Properti [`PageCount`](../pagecount) dapat melakukan perhitungan tambahan yang memengaruhi kecepatan ekstraksi teks dalam mode mentah.

### Lihat Juga

* interface [IDocumentInfo](../../idocumentinfo)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
