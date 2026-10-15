---
title: "Экспорт"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Экспортирует коллекцию метаданных в поток."
type: docs
weight: 20
url: /ru/net/groupdocs.parser.export/xmlexporter/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Экспортирует коллекцию метаданных в поток.

```csharp
public override void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| метаданные | IEnumerable`1 | Коллекция метаданных. |
| поток | Stream | Выходной поток. |

### См. также

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Экспортирует информацию о документе в поток.

```csharp
public override void Export(IDocumentInfo documentInfo, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Информация о документе. |
| поток | Stream | Выходной поток. |

### См. также

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Экспортирует коллекцию текстовых областей в поток.

```csharp
public override void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Коллекция текстовых областей. |
| поток | Stream | Выходной поток. |

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Экспортирует коллекцию таблиц в поток.

```csharp
public override void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| таблицы | IEnumerable`1 | Коллекция таблиц. |
| поток | Stream | Выходной поток. |

### См. также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Экспортирует коллекцию штрихкодов в поток.

```csharp
public override void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| штрихкоды | IEnumerable`1 | Коллекция штрих‑кодов. |
| поток | Stream | Выходной поток. |

### См. также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Экспортирует данные документа в поток.

```csharp
public override void Export(DocumentData documentData, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentData | DocumentData | Данные документа. |
| поток | Stream | Выходной поток. |

### См. также

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
