---
title: "XmlExporter"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет возможность экспорта данных в формате XML."
type: docs
weight: 660
url: /ru/net/groupdocs.parser.export/xmlexporter/
---

## XmlExporter class

Предоставляет возможность экспорта данных в формате XML.

```csharp
public sealed class XmlExporter : ExporterBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [XmlExporter](xmlexporter)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export)(DocumentData, Stream) | Экспортирует данные документа в поток. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(DocumentData, string) | Экспортирует данные документа в файл. |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_2)(IDocumentInfo, Stream) | Экспортирует информацию о документе в поток. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IDocumentInfo, string) | Экспортирует информацию о документе в файл. |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_4)(IEnumerable&lt;MetadataItem&gt;, Stream) | Экспортирует коллекцию метаданных в поток. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;MetadataItem&gt;, string) | Экспортирует коллекцию метаданных в файл. |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_6)(IEnumerable&lt;PageBarcodeArea&gt;, Stream) | Экспортирует коллекцию штрихкодов в поток. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageBarcodeArea&gt;, string) | Экспортирует коллекцию штрихкодов в файл. |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_8)(IEnumerable&lt;PageTableArea&gt;, Stream) | Экспортирует коллекцию таблиц в поток. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTableArea&gt;, string) | Экспортирует коллекцию таблиц в файл. |
| override [Export](../../groupdocs.parser.export/xmlexporter/export#export_10)(IEnumerable&lt;PageTextArea&gt;, Stream) | Экспортирует коллекцию текстовых областей в поток. |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTextArea&gt;, string) | Экспортирует коллекцию текстовых областей в файл. |

### См. также

* class [ExporterBase](../exporterbase)
* namespace [GroupDocs.Parser.Export](../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
