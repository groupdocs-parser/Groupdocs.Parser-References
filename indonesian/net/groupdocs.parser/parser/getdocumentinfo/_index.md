---
title: "GetDocumentInfo"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengembalikan informasi umum tentang dokumen."
type: docs
weight: 90
url: /id/net/groupdocs.parser/parser/getdocumentinfo/
---

## Parser.GetDocumentInfo method

Mengembalikan informasi umum tentang dokumen.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Nilai Kembali

Sebuah instance dari kelas yang mengimplementasikan antarmuka [`IDocumentInfo`](../../../groupdocs.parser.options/idocumentinfo).

### Catatan

**Learn more:**

* [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Contoh

Contoh berikut menunjukkan cara mendapatkan info dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Dapatkan informasi dokumen
    IDocumentInfo info = parser.GetDocumentInfo();

    Console.WriteLine(string.Format("FileType: {0}", info.FileType));
    Console.WriteLine(string.Format("PageCount: {0}", info.PageCount));
    Console.WriteLine(string.Format("Size: {0}", info.Size));
}
```

### Lihat Juga

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
