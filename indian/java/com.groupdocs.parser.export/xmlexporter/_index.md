---
title: "XmlExporter"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "डेटा को XML फ़ॉर्मेट में निर्यात करने की कार्यक्षमता प्रदान करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.parser.export/xmlexporter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.export.ExporterBase](../../com.groupdocs.parser.export/exporterbase)
```
public final class XmlExporter extends ExporterBase
```

डेटा को XML फ़ॉर्मेट में निर्यात करने की कार्यक्षमता प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [XmlExporter()](#XmlExporter--) | एक नया उदाहरण प्रारंभ करता है [XmlExporter](../../com.groupdocs.parser.export/xmlexporter) क्लास का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)](#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-) | मेटाडेटा संग्रह को स्ट्रीम में निर्यात करता है। |
|
|  | [exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)](#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-) | दस्तावेज़ जानकारी को स्ट्रीम में निर्यात करता है। |
|
|  | [exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)](#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-) | पाठ क्षेत्रों के संग्रह को स्ट्रीम में निर्यात करता है। |
|
|  | [exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)](#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-) | तालिकाओं के संग्रह को स्ट्रीम में निर्यात करता है। |
|
|  | [exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)](#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-) | बारकोड के संग्रह को स्ट्रीम में निर्यात करता है। |
|
|  | [exportDocumentData(DocumentData documentData, OutputStream outputStream)](#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-) | दस्तावेज़ डेटा को स्ट्रीम में निर्यात करता है। |
|
### XmlExporter() {#XmlExporter--}
```
public XmlExporter()
```


एक नया उदाहरण प्रारंभ करता है [XmlExporter](../../com.groupdocs.parser.export/xmlexporter) क्लास का।


### exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream) {#exportMetadata-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--java.io.OutputStream-}
```
public void exportMetadata(Iterable<MetadataItem> metadata, OutputStream outputStream)
```


मेटाडेटा संग्रह को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | मेटाडेटा का संग्रह। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream) {#exportDocumentInfo-com.groupdocs.parser.options.IDocumentInfo-java.io.OutputStream-}
```
public void exportDocumentInfo(IDocumentInfo documentInfo, OutputStream outputStream)
```


दस्तावेज़ जानकारी को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentInfo | [IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo) | दस्तावेज़ जानकारी। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream) {#exportTextAreas-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--java.io.OutputStream-}
```
public void exportTextAreas(Iterable<PageTextArea> textAreas, OutputStream outputStream)
```


पाठ क्षेत्रों के संग्रह को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | textAreas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea} | टेक्स्ट क्षेत्रों का संग्रह। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportTables(Iterable<PageTableArea> tables, OutputStream outputStream) {#exportTables-java.lang.Iterable-com.groupdocs.parser.data.PageTableArea--java.io.OutputStream-}
```
public void exportTables(Iterable<PageTableArea> tables, OutputStream outputStream)
```


तालिकाओं के संग्रह को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | tables | java.lang.Iterable<com.groupdocs.parser.data.PageTableArea} | टेबलों का संग्रह। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream) {#exportBarcodes-java.lang.Iterable-com.groupdocs.parser.data.PageBarcodeArea--java.io.OutputStream-}
```
public void exportBarcodes(Iterable<PageBarcodeArea> barcodes, OutputStream outputStream)
```


बारकोड के संग्रह को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | barcodes | java.lang.Iterable<com.groupdocs.parser.data.PageBarcodeArea} | बारकोड का संग्रह। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### exportDocumentData(DocumentData documentData, OutputStream outputStream) {#exportDocumentData-com.groupdocs.parser.data.DocumentData-java.io.OutputStream-}
```
public void exportDocumentData(DocumentData documentData, OutputStream outputStream)
```


दस्तावेज़ डेटा को स्ट्रीम में निर्यात करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentData | [DocumentData](../../com.groupdocs.parser.data/documentdata) | दस्तावेज़ डेटा। |
|
|  | outputStream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

