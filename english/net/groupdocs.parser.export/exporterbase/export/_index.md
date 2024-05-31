---
title: Export
second_title: GroupDocs.Parser for .NET API Reference
description: Exports the collection of metadata to the stream.
type: docs
weight: 10
url: /net/groupdocs.parser.export/exporterbase/export/
---
## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Exports the collection of metadata to the stream.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| metadata | IEnumerable`1 | The collection of metadata. |
| stream | Stream | The output stream. |

### See Also

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

Exports the collection of metadata to the file.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| metadata | IEnumerable`1 | The collection of metadata. |
| fileName | String | The full path to the output file. |

### See Also

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Exports the document information to the stream.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | IDocumentInfo | The document information. |
| stream | Stream | The output stream. |

### See Also

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

Exports the document information to the file.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | IDocumentInfo | The document information. |
| fileName | String | The full path to the output file. |

### See Also

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Exports the collection of text areas to the stream.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| textAreas | IEnumerable`1 | The collection of the text areas. |
| stream | Stream | The output stream. |

### See Also

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

Exports the collectiob of text areas to the file.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| textAreas | IEnumerable`1 | The collection of text areas. |
| fileName | String | The full path to the output file. |

### See Also

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Exports the collection of tables to the stream.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tables | IEnumerable`1 | The collecton of tables. |
| stream | Stream | The output stream. |

### See Also

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

Exports the collection of tables to the file.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tables | IEnumerable`1 | The collection of tables. |
| fileName | String | The full path to the output file. |

### See Also

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Exports the collection of barcodes to the stream.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| barcodes | IEnumerable`1 | The collection of barcodes. |
| stream | Stream | The output stream. |

### See Also

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

Exports the collection of barcodes to the file.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| barcodes | IEnumerable`1 | The collection of barcodes. |
| fileName | String | The full path to the output file. |

### See Also

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Exports document data to the stream.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documentData | DocumentData | Document data. |
| stream | Stream | The output stream. |

### See Also

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

Exports document data to the file.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| documentData | DocumentData | Document data. |
| fileName | String | The full path to the output file. |

### See Also

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
