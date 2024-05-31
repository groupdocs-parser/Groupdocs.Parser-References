---
title: Export
second_title: GroupDocs.Parser for .NET API Reference
description: Exports the collection of metadata to the stream.
type: docs
weight: 20
url: /net/groupdocs.parser.export/xmlexporter/export/
---
## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Exports the collection of metadata to the stream.

```csharp
public override void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| metadata | IEnumerable`1 | The collection of metadata. |
| stream | Stream | The output stream. |

### See Also

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Exports the document information to the stream.

```csharp
public override void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | IDocumentInfo | The document information. |
| stream | Stream | The output stream. |

### See Also

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Exports the collection of text areas to the stream.

```csharp
public override void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| textAreas | IEnumerable`1 | The collection of the text areas. |
| stream | Stream | The output stream. |

### See Also

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Exports the collection of tables to the stream.

```csharp
public override void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tables | IEnumerable`1 | The collecton of tables. |
| stream | Stream | The output stream. |

### See Also

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Exports the collection of barcodes to the stream.

```csharp
public override void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| barcodes | IEnumerable`1 | The collection of barcodes. |
| stream | Stream | The output stream. |

### See Also

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Exports document data to the stream.

```csharp
public override void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documentData | DocumentData | Document data. |
| stream | Stream | The output stream. |

### See Also

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->