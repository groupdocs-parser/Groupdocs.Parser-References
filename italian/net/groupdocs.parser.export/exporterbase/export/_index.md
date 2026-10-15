---
title: "Esporta"
second_title: "Riferimento API di GroupDocs.Parser per .NET"
description: "Esporta la raccolta di metadati nello stream."
type: docs
weight: 10
url: /it/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Esporta la raccolta di metadati nello stream.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| metadati | IEnumerable`1 | La raccolta di metadati. |
| stream | Stream | Il flusso di output. |

### Vedi anche

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

Esporta la raccolta di metadati nel file.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| metadati | IEnumerable`1 | La raccolta di metadati. |
| fileName | Stringa | Il percorso completo del file di output. |

### Vedi anche

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Esporta le informazioni del documento nello stream.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Le informazioni del documento. |
| stream | Stream | Il flusso di output. |

### Vedi anche

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

Esporta le informazioni del documento nel file.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Le informazioni del documento. |
| fileName | Stringa | Il percorso completo del file di output. |

### Vedi anche

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Esporta la raccolta di aree di testo nello stream.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| textAreas | IEnumerable`1 | La raccolta delle aree di testo. |
| stream | Stream | Il flusso di output. |

### Vedi anche

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

Esporta la raccolta di aree di testo nel file.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| textAreas | IEnumerable`1 | La raccolta di aree di testo. |
| fileName | Stringa | Il percorso completo del file di output. |

### Vedi anche

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Esporta la raccolta di tabelle nello stream.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| tabelle | IEnumerable`1 | La raccolta di tabelle. |
| stream | Stream | Il flusso di output. |

### Vedi anche

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

Esporta la raccolta di tabelle nel file.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| tabelle | IEnumerable`1 | La raccolta di tabelle. |
| fileName | Stringa | Il percorso completo del file di output. |

### Vedi anche

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Esporta la raccolta di codici a barre nello stream.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| codici a barre | IEnumerable`1 | La raccolta di codici a barre. |
| stream | Stream | Il flusso di output. |

### Vedi anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

Esporta la raccolta di codici a barre nel file.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| codici a barre | IEnumerable`1 | La raccolta di codici a barre. |
| fileName | Stringa | Il percorso completo del file di output. |

### Vedi anche

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Esporta i dati del documento nello stream.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documentData | DocumentData | Dati del documento. |
| stream | Stream | Il flusso di output. |

### Vedi anche

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

Esporta i dati del documento nel file.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documentData | DocumentData | Dati del documento. |
| fileName | Stringa | Il percorso completo del file di output. |

### Vedi anche

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
