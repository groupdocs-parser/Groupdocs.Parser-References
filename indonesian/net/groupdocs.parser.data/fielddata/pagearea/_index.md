---
title: "PageArea"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mendapatkan nilai bidang."
type: docs
weight: 30
url: /id/net/groupdocs.parser.data/fielddata/pagearea/
---

## FieldData.PageArea property

Mendapatkan nilai bidang.

```csharp
public PageArea PageArea { get; }
```

### Property Value

Sebuah instance dari kelas [`PageArea`](../../pagearea) yang mewakili nilai bidang.

### Contoh

Bergantung pada properti `PageArea` bidang, dapat berisi salah satu turunan dari kelas [`PageArea`](../../pagearea). Misalnya, metode [`ParseForm`](../../../groupdocs.parser/parser/parseform) mengekstrak hanya bidang teks.

```csharp
// Dapatkan data bidang
FieldData field = data[i];
// Periksa apakah data bidang berisi teks
if(field.PageArea is PageTextArea)
{
    // Cetak nilai teks bidang
    Console.WriteLine(field.Text);
}
```

### Lihat Juga

* class [PageArea](../../pagearea)
* class [FieldData](../../fielddata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
