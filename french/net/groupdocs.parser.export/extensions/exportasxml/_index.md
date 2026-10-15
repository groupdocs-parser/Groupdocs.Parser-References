---
title: "ExportAsXml"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Exporte la collection de métadonnées vers le flux au format XML."
type: docs
weight: 20
url: /fr/net/groupdocs.parser.export/extensions/exportasxml/
---

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, Stream) {#exportasxml_4}

Exporte la collection de métadonnées vers le flux au format XML.

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| métadonnées | IEnumerable`1 | La collection de métadonnées. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, string) {#exportasxml_5}

Exporte la collection de métadonnées vers le fichier au format XML.

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| métadonnées | IEnumerable`1 | La collection de métadonnées. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IDocumentInfo, Stream) {#exportasxml_2}

Exporte les informations du document vers le flux au format XML.

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Les informations du document. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IDocumentInfo, string) {#exportasxml_3}

Exporte les informations du document vers le fichier au format XML.

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Les informations du document. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, Stream) {#exportasxml_10}

Exporte la collection de zones de texte vers le flux au format XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| textAreas | IEnumerable`1 | La collection des zones de texte. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, string) {#exportasxml_11}

Exporte la collectiob de zones de texte vers le fichier au format XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| textAreas | IEnumerable`1 | La collection de zones de texte. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, Stream) {#exportasxml_8}

Exporte la collection de tables vers le flux au format XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tables | IEnumerable`1 | La collection de tables. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, string) {#exportasxml_9}

Exporte la collection de tables vers le fichier au format XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tables | IEnumerable`1 | La collection de tables. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#exportasxml_6}

Exporte la collection de codes-barres vers le flux au format XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| codes-barres | IEnumerable`1 | La collection de codes-barres. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, string) {#exportasxml_7}

Exporte la collection de codes-barres vers le fichier au format XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| codes-barres | IEnumerable`1 | La collection de codes-barres. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this DocumentData, Stream) {#exportasxml}

Exporte les données du document vers le flux au format XML.

```csharp
public static void ExportAsXml(this DocumentData documentData, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentData | DocumentData | Données du document. |
| flux | Stream | Le flux de sortie. |

### Voir aussi

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this DocumentData, string) {#exportasxml_1}

Exporte les données du document vers le fichier au format XML.

```csharp
public static void ExportAsXml(this DocumentData documentData, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentData | DocumentData | Données du document. |
| fileName | Chaîne | Le chemin complet du fichier de sortie. |

### Voir aussi

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
