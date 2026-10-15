---
title: "Templat"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menginisialisasi instance baru dari kelas Templategroupdocs.parser.templates/template."
type: docs
weight: 10
url: /id/net/groupdocs.parser.templates/template/template/
---

## Template(IEnumerable&lt;TemplateItem&gt;) {#constructor}

Menginisialisasi instance baru dari kelas [`Template`](../../template).

```csharp
public Template(IEnumerable<TemplateItem> items)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| items | IEnumerable`1 | Koleksi objek [`TemplateItem`](../../templateitem). |

### Contoh

Penggunaan:

```csharp
// Buat array bidang templat
TemplateItem[] fields = new TemplateItem[]
{
   new TemplateField(new TemplateRegexPosition("From"), "From", 0),
   new TemplateField(
       new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromCompany",
       0),
   new TemplateField(
       new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromAddress",
       0)
};

// Buat templat dokumen
Template template = new Template(fields);
```

### Lihat Juga

* class [TemplateItem](../../templateitem)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Template(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) {#constructor_1}

Menginisialisasi instance baru dari kelas [`Template`](../../template) dengan opsi templat.

```csharp
public Template(IEnumerable<TemplateItem> items, TemplateOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| items | IEnumerable`1 | Koleksi objek [`TemplateItem`](../../templateitem). |
| options | TemplateOptions | Opsi templat. |

### Lihat Juga

* class [TemplateItem](../../templateitem)
* class [TemplateOptions](../../templateoptions)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
