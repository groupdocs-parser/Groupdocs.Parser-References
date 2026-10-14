---
title: "XmlExporter"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τη λειτουργικότητα εξαγωγής δεδομένων σε μορφή XML."
type: docs
weight: 11
url: /el/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

Παρέχει τη λειτουργικότητα εξαγωγής δεδομένων σε μορφή XML.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XmlExporter](../../com.groupdocs.parser.export/xmlexporter). |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Εξάγει τη συλλογή μεταδεδομένων στη ροή. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Εξάγει τις πληροφορίες του εγγράφου στη ροή. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Εξάγει τη συλλογή περιοχών κειμένου στη ροή. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Εξάγει τη συλλογή πινάκων στη ροή. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Εξάγει τη συλλογή γραμμωτών κωδίκων στη ροή. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Εξάγει δεδομένα εγγράφου στη ροή. |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XmlExporter](../../com.groupdocs.parser.export/xmlexporter).


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Εξάγει τη συλλογή μεταδεδομένων στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | μεταδεδομένα | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Η συλλογή των μεταδεδομένων. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Εξάγει τις πληροφορίες του εγγράφου στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Οι πληροφορίες του εγγράφου. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Εξάγει τη συλλογή περιοχών κειμένου στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Η συλλογή των περιοχών κειμένου. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Εξάγει τη συλλογή πινάκων στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Η συλλογή των πινάκων. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Εξάγει τη συλλογή γραμμωτών κωδίκων στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Η συλλογή των barcode. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Εξάγει δεδομένα εγγράφου στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Δεδομένα εγγράφου. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

