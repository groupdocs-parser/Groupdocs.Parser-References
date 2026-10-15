---
title: "GetFieldsByName"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengembalikan koleksi data bidang dimana namanya sama dengan fieldName."
type: docs
weight: 50
url: /id/net/groupdocs.parser.data/documentdata/getfieldsbyname/
---

## DocumentData.GetFieldsByName method

Mengembalikan koleksi data bidang dimana namanya sama dengan *fieldName*.

```csharp
public IList<FieldData> GetFieldsByName(string fieldName)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| fieldName | String | Nama bidang. |

### Nilai Kembali

Koleksi objek [`FieldData`](../../fielddata); koleksi kosong jika tidak ada data bidang yang ditemukan.

### Contoh

Temukan bidang berdasarkan nama bidang:

```csharp
// Dapatkan semua bidang dengan nama "Address" 
IList<FieldData> addressFields = data.GetFieldsByName("Address");
if(addressFields.Count == 0) {
    Console.WriteLine("Address not found");
}
else {
    Console.WriteLine("Address");
    // Iterasi atas koleksi bidang
    for (int i = 0; i < addressFields.Count; i++) {
        PageTextArea area = addressFields[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);       
         
        // Jika itu bidang terkait:
        if(addressFields[i].LinkedField != null) {
            Console.Write("Linked to ");
            PageTextArea linkedArea = addressFields[i].LinkedField.PageArea as PageTextArea;
            Console.WriteLine(area == null ? "Not a template field" : area.Text);           
        }
    }
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields.

### Lihat Juga

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
