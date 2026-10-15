---
title: "Exporter"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Exporte la collection de métadonnées vers le flux."
type: docs
weight: 10
url: /fr/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Exporte la collection de métadonnées vers le flux.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| métadonnées | IEnumerable`1 | La collection de métadonnées. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

Exporte la collection de métadonnées vers le fichier.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| métadonnées | IEnumerable`1 | La collection de métadonnées. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Exporte les informations du document vers le flux.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Les informations du document. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

Exporte les informations du document vers le fichier.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Les informations du document. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Exporte la collection de zones de texte vers le flux.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| textAreas | IEnumerable`1 | La collection des zones de texte. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

Exporte la collection de zones de texte vers le fichier.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| textAreas | IEnumerable`1 | La collection de zones de texte. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Exporte la collection de tableaux vers le flux.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tables | IEnumerable`1 | La collection de tables. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

Exporte la collection de tableaux vers le fichier.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tables | IEnumerable`1 | La collection de tables. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Exporte la collection de codes-barres vers le flux.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| codes-barres | IEnumerable`1 | La collection de codes-barres. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

Exporte la collection de codes-barres vers le fichier.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| codes-barres | IEnumerable`1 | La collection de codes-barres. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Exporte les données du document vers le flux.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentData | DocumentData | Données du document. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

Exporte les données du document vers le fichier.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentData | DocumentData | Données du document. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
