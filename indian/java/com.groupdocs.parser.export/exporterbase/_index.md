---
title: "ExporterBase"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "डेटा निर्यात कार्यक्षमता के लिए बेस क्लास प्रदान करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.parser.export/exporterbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExporterBase
```

डेटा निर्यात कार्यक्षमता के लिए बेस क्लास प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ExporterBase()](#ExporterBase--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | मेटाडेटा संग्रह को स्ट्रीम में निर्यात करता है। |
|
|  | [exportMetadata(Iterable<MetadataItem> metadata, String fileName)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-) | मेटाडेटा संग्रह को फ़ाइल में निर्यात करता है। |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | दस्तावेज़ जानकारी को स्ट्रीम में निर्यात करता है। |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, String fileName)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-) | दस्तावेज़ जानकारी को फ़ाइल में निर्यात करता है। |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | पाठ क्षेत्रों के संग्रह को स्ट्रीम में निर्यात करता है। |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-) | पाठ क्षेत्रों के संग्रह को फ़ाइल में निर्यात करता है। |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | तालिकाओं के संग्रह को स्ट्रीम में निर्यात करता है। |
|
|  | [exportTables(Iterable<PageTableArea> tables, String fileName)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-) | तालिकाओं के संग्रह को फ़ाइल में निर्यात करता है। |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | बारकोड के संग्रह को स्ट्रीम में निर्यात करता है। |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-) | बारकोड के संग्रह को फ़ाइल में निर्यात करता है। |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | दस्तावेज़ डेटा को स्ट्रीम में निर्यात करता है। |
|
|  | [exportDocumentData(DocumentData documentData, String fileName)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-) | दस्तावेज़ डेटा को फ़ाइल में निर्यात करता है। |
|
### ExporterBase() {#ExporterBase--}
```
public ExporterBase()
```


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public abstract void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


मेटाडेटा संग्रह को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | मेटाडेटा का संग्रह। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportMetadata(Iterable<MetadataItem> metadata, String fileName) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.lang.String-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, String fileName)
```


मेटाडेटा संग्रह को फ़ाइल में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | मेटाडेटा का संग्रह। |
|
|  | fileName | java.lang.String | आउटपुट फ़ाइल का पूरा पथ। |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public abstract void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


दस्तावेज़ जानकारी को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | दस्तावेज़ जानकारी। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportDocumentInfo(IDocumentInfo documentInfo, String fileName) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.lang.String-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, String fileName)
```


दस्तावेज़ जानकारी को फ़ाइल में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | दस्तावेज़ जानकारी। |
|
|  | fileName | java.lang.String | आउटपुट फ़ाइल का पूरा पथ। |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public abstract void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


पाठ क्षेत्रों के संग्रह को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea} | टेक्स्ट क्षेत्रों का संग्रह। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, String fileName) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.lang.String-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, String fileName)
```


पाठ क्षेत्रों के संग्रह को फ़ाइल में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea} | टेक्स्ट क्षेत्रों का संग्रह। |
|
|  | fileName | java.lang.String | आउटपुट फ़ाइल का पूरा पथ। |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public abstract void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


तालिकाओं के संग्रह को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea} | टेबलों का संग्रह। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportTables(Iterable<PageTableArea> tables, String fileName) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.lang.String-}
```
public void exportTables(Iterable<PageTableArea> tables, String fileName)
```


तालिकाओं के संग्रह को फ़ाइल में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea} | टेबलों का संग्रह। |
|
|  | fileName | java.lang.String | आउटपुट फ़ाइल का पूरा पथ। |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public abstract void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


बारकोड के संग्रह को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea} | बारकोड का संग्रह। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.lang.String-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, String fileName)
```


बारकोड के संग्रह को फ़ाइल में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea} | बारकोड का संग्रह। |
|
|  | fileName | java.lang.String | आउटपुट फ़ाइल का पूरा पथ। |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public abstract void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


दस्तावेज़ डेटा को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | दस्तावेज़ डेटा। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportDocumentData(DocumentData documentData, String fileName) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.lang.String-}
```
public void exportDocumentData(DocumentData documentData, String fileName)
```


दस्तावेज़ डेटा को फ़ाइल में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | दस्तावेज़ डेटा। |
|
|  | fileName | java.lang.String | आउटपुट फ़ाइल का पूरा पथ। |
|

