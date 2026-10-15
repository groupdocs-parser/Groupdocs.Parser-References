---
title: "निर्यात"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "मेटाडेटा संग्रह को स्ट्रीम में निर्यात करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

मेटाडेटा संग्रह को स्ट्रीम में निर्यात करता है।

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मेटाडेटा | IEnumerable`1 | मेटाडेटा का संग्रह। |
| स्ट्रीम | Stream | आउटपुट स्ट्रीम। |

### संबंधित देखें

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

मेटाडेटा संग्रह को फ़ाइल में निर्यात करता है।

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मेटाडेटा | IEnumerable`1 | मेटाडेटा का संग्रह। |
| फ़ाइलनाम | स्ट्रिंग | आउटपुट फ़ाइल का पूर्ण पथ। |

### संबंधित देखें

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

दस्तावेज़ जानकारी को स्ट्रीम में निर्यात करता है।

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| documentInfo | IDocumentInfo | दस्तावेज़ जानकारी। |
| स्ट्रीम | Stream | आउटपुट स्ट्रीम। |

### संबंधित देखें

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

दस्तावेज़ जानकारी को फ़ाइल में निर्यात करता है।

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| documentInfo | IDocumentInfo | दस्तावेज़ जानकारी। |
| फ़ाइलनाम | स्ट्रिंग | आउटपुट फ़ाइल का पूर्ण पथ। |

### संबंधित देखें

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

टेक्स्ट एरिया संग्रह को स्ट्रीम में निर्यात करता है।

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| टेक्स्टएरिया | IEnumerable`1 | टेक्स्ट एरिया का संग्रह। |
| स्ट्रीम | Stream | आउटपुट स्ट्रीम। |

### संबंधित देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

टेक्स्ट एरिया संग्रह को फ़ाइल में निर्यात करता है।

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| टेक्स्टएरिया | IEnumerable`1 | टेक्स्ट एरिया का संग्रह। |
| फ़ाइलनाम | स्ट्रिंग | आउटपुट फ़ाइल का पूर्ण पथ। |

### संबंधित देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

टेबल्स संग्रह को स्ट्रीम में निर्यात करता है।

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| टेबल्स | IEnumerable`1 | टेबल्स का संग्रह। |
| स्ट्रीम | Stream | आउटपुट स्ट्रीम। |

### संबंधित देखें

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

टेबल्स संग्रह को फ़ाइल में निर्यात करता है।

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| टेबल्स | IEnumerable`1 | टेबल्स का संग्रह। |
| फ़ाइलनाम | स्ट्रिंग | आउटपुट फ़ाइल का पूर्ण पथ। |

### संबंधित देखें

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

बारकोड संग्रह को स्ट्रीम में निर्यात करता है।

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| बारकोड्स | IEnumerable`1 | बारकोड का संग्रह। |
| स्ट्रीम | Stream | आउटपुट स्ट्रीम। |

### संबंधित देखें

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

बारकोड संग्रह को फ़ाइल में निर्यात करता है।

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| बारकोड्स | IEnumerable`1 | बारकोड का संग्रह। |
| फ़ाइलनाम | स्ट्रिंग | आउटपुट फ़ाइल का पूर्ण पथ। |

### संबंधित देखें

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

दस्तावेज़ डेटा को स्ट्रीम में निर्यात करता है।

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| documentData | DocumentData | दस्तावेज़ डेटा। |
| स्ट्रीम | Stream | आउटपुट स्ट्रीम। |

### संबंधित देखें

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

दस्तावेज़ डेटा को फ़ाइल में निर्यात करता है।

```csharp
public void Export(DocumentData documentData, string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| documentData | DocumentData | दस्तावेज़ डेटा। |
| फ़ाइलनाम | स्ट्रिंग | आउटपुट फ़ाइल का पूर्ण पथ। |

### संबंधित देखें

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
