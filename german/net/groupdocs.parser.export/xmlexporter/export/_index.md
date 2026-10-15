---
title: "Export"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Exportiert die Metadaten-Sammlung in den Stream."
type: docs
weight: 20
url: /de/net/groupdocs.parser.export/xmlexporter/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Exportiert die Metadaten-Sammlung in den Stream.

```csharp
public override void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Metadaten | IEnumerable`1 | Die Sammlung von Metadaten. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Exportiert die Dokumentinformationen in den Stream.

```csharp
public override void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Die Dokumentinformationen. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Exportiert die Textbereichssammlung in den Stream.

```csharp
public override void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Die Sammlung der Textbereiche. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Exportiert die Tabellensammlung in den Stream.

```csharp
public override void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tables | IEnumerable`1 | Die Sammlung von Tabellen. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Exportiert die Barcode-Sammlung in den Stream.

```csharp
public override void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| barcodes | IEnumerable`1 | Die Sammlung von Barcodes. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Exportiert Dokumentdaten in den Stream.

```csharp
public override void Export(DocumentData documentData, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| documentData | DocumentData | Dokumentdaten. |
| stream | Stream | Der Ausgabestream. |

### Siehe auch

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [XmlExporter](../../xmlexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
