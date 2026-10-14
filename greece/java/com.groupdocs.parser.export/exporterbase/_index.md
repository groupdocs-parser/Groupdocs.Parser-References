---
title: "ExporterBase"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει τη βασική κλάση για τη λειτουργικότητα εξαγωγής δεδομένων."
type: docs
weight: 10
url: /el/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

Παρέχει τη βασική κλάση για τη λειτουργικότητα εξαγωγής δεδομένων.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | Εξάγει τη συλλογή μεταδεδομένων στη ροή. |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | Εξάγει τη συλλογή μεταδεδομένων στο αρχείο. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | Εξάγει τις πληροφορίες του εγγράφου στη ροή. |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | Εξάγει τις πληροφορίες του εγγράφου στο αρχείο. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | Εξάγει τη συλλογή περιοχών κειμένου στη ροή. |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | Εξάγει τη συλλογή περιοχών κειμένου στο αρχείο. |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | Εξάγει τη συλλογή πινάκων στη ροή. |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | Εξάγει τη συλλογή πινάκων στο αρχείο. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | Εξάγει τη συλλογή γραμμωτών κωδίκων στη ροή. |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | Εξάγει τη συλλογή γραμμωτών κωδίκων στο αρχείο. |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | Εξάγει δεδομένα εγγράφου στη ροή. |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | Εξάγει δεδομένα εγγράφου στο αρχείο. |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


Εξάγει τη συλλογή μεταδεδομένων στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | μεταδεδομένα | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Η συλλογή των μεταδεδομένων. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


Εξάγει τη συλλογή μεταδεδομένων στο αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | μεταδεδομένα | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Η συλλογή των μεταδεδομένων. |
|
|  | fileName | java.lang.String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


Εξάγει τις πληροφορίες του εγγράφου στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Οι πληροφορίες του εγγράφου. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


Εξάγει τις πληροφορίες του εγγράφου στο αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | Οι πληροφορίες του εγγράφου. |
|
|  | fileName | java.lang.String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


Εξάγει τη συλλογή περιοχών κειμένου στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Η συλλογή των περιοχών κειμένου. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


Εξάγει τη συλλογή περιοχών κειμένου στο αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Η συλλογή των περιοχών κειμένου. |
|
|  | fileName | java.lang.String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


Εξάγει τη συλλογή πινάκων στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Η συλλογή των πινάκων. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


Εξάγει τη συλλογή πινάκων στο αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea> | Η συλλογή των πινάκων. |
|
|  | fileName | java.lang.String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


Εξάγει τη συλλογή γραμμωτών κωδίκων στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Η συλλογή των barcode. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


Εξάγει τη συλλογή γραμμωτών κωδίκων στο αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea> | Η συλλογή των barcode. |
|
|  | fileName | java.lang.String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


Εξάγει δεδομένα εγγράφου στη ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Δεδομένα εγγράφου. |
|
|  | outputStream | java.io.OutputStream | Η ροή εξόδου. |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


Εξάγει δεδομένα εγγράφου στο αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | Δεδομένα εγγράφου. |
|
|  | fileName | java.lang.String | Η πλήρης διαδρομή προς το αρχείο εξόδου. |
|

