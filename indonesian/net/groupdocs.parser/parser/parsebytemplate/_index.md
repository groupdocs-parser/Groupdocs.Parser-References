---
title: "ParseByTemplate"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menganalisis dokumen dengan templat yang dibuat pengguna."
type: docs
weight: 230
url: /id/net/groupdocs.parser/parser/parsebytemplate/
---

## ParseByTemplate(Template) {#parsebytemplate}

Menganalisis dokumen dengan templat yang dibuat pengguna.

```csharp
public DocumentData ParseByTemplate(Template template)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| template | Templat | Templat yang dibuat pengguna. |

### Nilai Kembali

Sebuah instance kelas [`DocumentData`](../../../groupdocs.parser.data/documentdata) yang berisi data yang diekstrak; `null` jika parsing dengan templat tidak didukung.

### Catatan

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Lihat Juga

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(Template, ParseByTemplateOptions) {#parsebytemplate_1}

Menganalisis dokumen dengan templat yang dibuat pengguna menggunakan opsi kustomisasi.

```csharp
public DocumentData ParseByTemplate(Template template, ParseByTemplateOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| template | Templat | Templat yang dibuat pengguna. |
| options | ParseByTemplateOptions | Opsi kustomisasi. |

### Nilai Kembali

Sebuah instance kelas [`DocumentData`](../../../groupdocs.parser.data/documentdata) yang berisi data yang diekstrak; `null` jika parsing dengan templat tidak didukung.

### Catatan

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Lihat Juga

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(TemplateCollection, ParseByTemplateOptions) {#parsebytemplate_2}

Memilih templat paling cocok dari koleksi yang disediakan dan kemudian menganalisis dokumen dengan templat yang dipilih.

```csharp
public DocumentData ParseByTemplate(TemplateCollection templateCollection, 
    ParseByTemplateOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| templateCollection | TemplateCollection | Koleksi templat. |
| options | ParseByTemplateOptions | Opsi kustomisasi. |

### Nilai Kembali

Sebuah instance kelas [`DocumentData`](../../../groupdocs.parser.data/documentdata) yang berisi data yang diekstrak; `null` jika parsing dengan templat tidak didukung.

### Lihat Juga

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [TemplateCollection](../../../groupdocs.parser.templates/templatecollection)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
