---
title: "JsonExporter"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan fungsionalitas untuk mengekspor data dalam format JSON."
type: docs
weight: 650
url: /id/net/groupdocs.parser.export/jsonexporter/
---

## JsonExporter class

Menyediakan fungsionalitas untuk mengekspor data dalam format JSON.

```csharp
public sealed class JsonExporter : ExporterBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [JsonExporter](jsonexporter)() | Konstruktor default. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export)(DocumentData, Stream) | Mengekspor data dokumen ke aliran. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(DocumentData, string) | Mengekspor data dokumen ke file. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_2)(IDocumentInfo, Stream) | Mengekspor informasi dokumen ke aliran. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IDocumentInfo, string) | Mengekspor informasi dokumen ke file. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_4)(IEnumerable&lt;MetadataItem&gt;, Stream) | Mengekspor koleksi metadata ke aliran. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;MetadataItem&gt;, string) | Mengekspor koleksi metadata ke file. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_6)(IEnumerable&lt;PageBarcodeArea&gt;, Stream) | Mengekspor koleksi kode batang ke aliran. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageBarcodeArea&gt;, string) | Mengekspor koleksi kode batang ke file. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_8)(IEnumerable&lt;PageTableArea&gt;, Stream) | Mengekspor koleksi tabel ke aliran. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTableArea&gt;, string) | Mengekspor koleksi tabel ke file. |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_10)(IEnumerable&lt;PageTextArea&gt;, Stream) | Mengekspor koleksi area teks ke aliran. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTextArea&gt;, string) | Mengekspor koleksi area teks ke file. |

### Lihat Juga

* class [ExporterBase](../exporterbase)
* namespace [GroupDocs.Parser.Export](../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
