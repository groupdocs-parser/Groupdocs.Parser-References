---
title: "Item"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mendapatkan data bidang berdasarkan indeks."
type: docs
weight: 20
url: /id/net/groupdocs.parser.data/documentdata/item/
---

## DocumentData indexer

Mendapatkan data bidang berdasarkan indeks.

```csharp
public FieldData this[int index] { get; }
```

| Parameter | Deskripsi |
| --- | --- |
| indeks | Indeks berbasis nol dari bidang. |

### Nilai Kembali

Sebuah instance dari kelas [`FieldData`](../../fielddata).

### Contoh

Iterasi melalui semua bidang:

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields:

```csharp
// Buat parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak data dari Formulir PDF
    DocumentData data = parser.ParseForm();
    // Iterasi atas bidang yang diekstrak
    for (int i = 0; i < data.Count; i++)
    {
        // Dapatkan bidang yang diekstrak
        FieldData field = data[i];
        // Cetak nama bidang
        Console.Write(field.Name + ": ");
        // Periksa apakah nilai bidang berupa teks dan cetak
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### Lihat Juga

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
