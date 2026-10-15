---
title: "Εξαγωγή"
second_title: "GroupDocs.Parser για .NET API Reference"
description: "Εξάγει τη συλλογή των μεταδεδομένων στη ροή."
type: docs
weight: 10
url: /el/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Εξάγει τη συλλογή των μεταδεδομένων στη ροή.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| μεταδεδομένα | IEnumerable`1 | Η συλλογή των μεταδεδομένων. |
| ροή | Stream | Η ροή εξόδου. |

### Δείτε επίσης

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

Εξάγει τη συλλογή των μεταδεδομένων στο αρχείο.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| μεταδεδομένα | IEnumerable`1 | Η συλλογή των μεταδεδομένων. |
| fileName | String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |

### Δείτε επίσης

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Εξάγει τις πληροφορίες του εγγράφου στη ροή.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Οι πληροφορίες του εγγράφου. |
| ροή | Stream | Η ροή εξόδου. |

### Δείτε επίσης

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

Εξάγει τις πληροφορίες του εγγράφου στο αρχείο.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Οι πληροφορίες του εγγράφου. |
| fileName | String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |

### Δείτε επίσης

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Εξάγει τη συλλογή των περιοχών κειμένου στη ροή.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Η συλλογή των περιοχών κειμένου. |
| ροή | Stream | Η ροή εξόδου. |

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

Εξάγει τη συλλογή των περιοχών κειμένου στο αρχείο.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Η συλλογή των περιοχών κειμένου. |
| fileName | String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |

### Δείτε επίσης

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Εξάγει τη συλλογή των πινάκων στη ροή.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| πίνακες | IEnumerable`1 | Η συλλογή των πινάκων. |
| ροή | Stream | Η ροή εξόδου. |

### Δείτε επίσης

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

Εξάγει τη συλλογή των πινάκων στο αρχείο.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| πίνακες | IEnumerable`1 | Η συλλογή των πινάκων. |
| fileName | String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |

### Δείτε επίσης

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Εξάγει τη συλλογή των γραμμωτών κωδίκων στη ροή.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| γραμμωτοί κώδικες | IEnumerable`1 | Η συλλογή των γραμμωτών κωδίκων. |
| ροή | Stream | Η ροή εξόδου. |

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

Εξάγει τη συλλογή των γραμμωτών κωδίκων στο αρχείο.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| γραμμωτοί κώδικες | IEnumerable`1 | Η συλλογή των γραμμωτών κωδίκων. |
| fileName | String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |

### Δείτε επίσης

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Εξάγει τα δεδομένα του εγγράφου στη ροή.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| documentData | DocumentData | Δεδομένα εγγράφου. |
| ροή | Stream | Η ροή εξόδου. |

### Δείτε επίσης

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

Εξάγει τα δεδομένα του εγγράφου στο αρχείο.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| documentData | DocumentData | Δεδομένα εγγράφου. |
| fileName | String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |

### Δείτε επίσης

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
