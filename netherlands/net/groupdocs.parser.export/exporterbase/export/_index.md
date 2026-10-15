---
title: "Exporteren"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Exporteert de verzameling metadata naar de stream."
type: docs
weight: 10
url: /nl/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Exporteert de verzameling metadata naar de stream.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| metadata | IEnumerable`1 | De verzameling metadata. |
| stream | Stream | De uitvoerstream. |

### Zie ook

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

Exporteert de verzameling metadata naar het bestand.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| metadata | IEnumerable`1 | De verzameling metadata. |
| fileName | String | Het volledige pad naar het uitvoerbestand. |

### Zie ook

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Exporteert de documentinformatie naar de stream.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| documentInfo | IDocumentInfo | De documentinformatie. |
| stream | Stream | De uitvoerstream. |

### Zie ook

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

Exporteert de documentinformatie naar het bestand.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| documentInfo | IDocumentInfo | De documentinformatie. |
| fileName | String | Het volledige pad naar het uitvoerbestand. |

### Zie ook

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Exporteert de verzameling tekstgebieden naar de stream.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| textAreas | IEnumerable`1 | De collectie van de tekstgebieden. |
| stream | Stream | De uitvoerstream. |

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

Exporteert de verzameling tekstgebieden naar het bestand.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| textAreas | IEnumerable`1 | De collectie van tekstgebieden. |
| fileName | String | Het volledige pad naar het uitvoerbestand. |

### Zie ook

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Exporteert de verzameling tabellen naar de stream.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tabellen | IEnumerable`1 | De collectie van tabellen. |
| stream | Stream | De uitvoerstream. |

### Zie ook

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

Exporteert de verzameling tabellen naar het bestand.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tabellen | IEnumerable`1 | De collectie van tabellen. |
| fileName | String | Het volledige pad naar het uitvoerbestand. |

### Zie ook

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Exporteert de verzameling barcodes naar de stream.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| barcodes | IEnumerable`1 | De verzameling van barcodes. |
| stream | Stream | De uitvoerstream. |

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

Exporteert de verzameling barcodes naar het bestand.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| barcodes | IEnumerable`1 | De verzameling van barcodes. |
| fileName | String | Het volledige pad naar het uitvoerbestand. |

### Zie ook

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Exporteert documentgegevens naar de stream.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| documentData | DocumentData | Documentgegevens. |
| stream | Stream | De uitvoerstream. |

### Zie ook

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

Exporteert documentgegevens naar het bestand.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| documentData | DocumentData | Documentgegevens. |
| fileName | String | Het volledige pad naar het uitvoerbestand. |

### Zie ook

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
