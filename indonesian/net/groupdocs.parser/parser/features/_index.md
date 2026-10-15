---
title: "Fitur"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mendapatkan fitur yang didukung."
type: docs
weight: 20
url: /id/net/groupdocs.parser/parser/features/
---

## Parser.Features property

Mendapatkan fitur yang didukung.

```csharp
public Features Features { get; }
```

### Property Value

Sebuah instance dari kelas [`Features`](../../../groupdocs.parser.options/features) yang mewakili fitur yang didukung.

### Catatan

**Learn more:**

* [Get supported features](https://docs.groupdocs.com/display/parsernet/Get+supported+features)

### Contoh

Jika fitur tidak didukung, metode mengembalikan `null` alih-alih nilai. Beberapa operasi dapat memakan waktu yang signifikan. Jadi tidak optimal memanggil metode hanya untuk memeriksa dukungan fitur. Untuk tujuan ini properti Features digunakan:

```csharp
using(Parser parser = new Parser("doc.zip"))
{
    if(!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported");
        return;
    }
 
    using(TextReader reader = parser.GetText())
    {
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

### Lihat Juga

* class [Features](../../../groupdocs.parser.options/features)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
