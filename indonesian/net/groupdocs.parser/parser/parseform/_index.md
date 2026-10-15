---
title: "ParseForm"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menganalisis formulir dokumen."
type: docs
weight: 240
url: /id/net/groupdocs.parser/parser/parseform/
---

## Parser.ParseForm method

Menganalisis formulir dokumen.

```csharp
public DocumentData ParseForm()
```

### Nilai Kembali

Sebuah instance kelas [`DocumentData`](../../../groupdocs.parser.data/documentdata) yang berisi data yang diekstrak; `null` jika parsing dengan templat tidak didukung.

### Catatan

**Learn more:**

* [Extract data from PDF forms](https://docs.groupdocs.com/display/parsernet/Extract+data+from+PDF+forms)
* [Working with extracted data](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Contoh

Contoh berikut menunjukkan cara mengurai sebuah formulir dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak data dari dokumen PDF
    DocumentData data = parser.ParseForm();
    // Iterasi atas data yang diekstrak
    for (int i = 0; i<data.Count; i++)
    {
        Console.Write(data[i].Name + ": ");
        PageTextArea area = data[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### Lihat Juga

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
