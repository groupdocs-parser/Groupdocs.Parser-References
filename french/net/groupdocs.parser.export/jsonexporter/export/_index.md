---
title: "Exporter"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Exporte la collection de métadonnées vers le flux."
type: docs
weight: 20
url: /fr/net/groupdocs.parser.export/jsonexporter/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Exporte la collection de métadonnées vers le flux.

```csharp
public override void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| métadonnées | IEnumerable`1 | La collection de métadonnées. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [JsonExporter](../../jsonexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Exporte les informations du document vers le flux.

```csharp
public override void Export(IDocumentInfo documentInfo, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Les informations du document. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [JsonExporter](../../jsonexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Exporte la collection de zones de texte vers le flux.

```csharp
public override void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| textAreas | IEnumerable`1 | La collection des zones de texte. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [JsonExporter](../../jsonexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Exporte la collection de tableaux vers le flux.

```csharp
public override void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tables | IEnumerable`1 | La collection de tables. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [JsonExporter](../../jsonexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Exporte la collection de codes-barres vers le flux.

```csharp
public override void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| codes-barres | IEnumerable`1 | La collection de codes-barres. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [JsonExporter](../../jsonexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Exporte les données du document vers le flux.

```csharp
public override void Export(DocumentData documentData, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentData | DocumentData | Données du document. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [JsonExporter](../../jsonexporter)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
