---
title: "Export"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Exportiert die Metadaten-Sammlung in den Stream."
type: docs
weight: 10
url: /de/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Exportiert die Metadaten-Sammlung in den Stream.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Metadaten | IEnumerable`1 | Die Sammlung von Metadaten. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

Exportiert die Metadaten-Sammlung in die Datei.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Metadaten | IEnumerable`1 | Die Sammlung von Metadaten. |
| fileName | String | Der vollständige Pfad zur Ausgabedatei. |

### Siehe auch

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Exportiert die Dokumentinformationen in den Stream.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Die Dokumentinformationen. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

Exportiert die Dokumentinformationen in die Datei.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Die Dokumentinformationen. |
| fileName | String | Der vollständige Pfad zur Ausgabedatei. |

### Siehe auch

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Exportiert die Textbereichssammlung in den Stream.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Die Sammlung der Textbereiche. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

Exportiert die Textbereichssammlung in die Datei.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Die Sammlung von Textbereichen. |
| fileName | String | Der vollständige Pfad zur Ausgabedatei. |

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Exportiert die Tabellensammlung in den Stream.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tables | IEnumerable`1 | Die Sammlung von Tabellen. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

Exportiert die Tabellensammlung in die Datei.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tables | IEnumerable`1 | Die Sammlung von Tabellen. |
| fileName | String | Der vollständige Pfad zur Ausgabedatei. |

### Siehe auch

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Exportiert die Barcode-Sammlung in den Stream.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| barcodes | IEnumerable`1 | Die Sammlung von Barcodes. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

Exportiert die Barcode-Sammlung in die Datei.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| barcodes | IEnumerable`1 | Die Sammlung von Barcodes. |
| fileName | String | Der vollständige Pfad zur Ausgabedatei. |

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Exportiert Dokumentdaten in den Stream.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| documentData | DocumentData | Dokumentdaten. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

Exportiert Dokumentdaten in die Datei.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| documentData | DocumentData | Dokumentdaten. |
| fileName | String | Der vollständige Pfad zur Ausgabedatei. |

### Siehe auch

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
