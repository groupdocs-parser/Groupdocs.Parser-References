---
title: "JsonExporter"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "JSON फ़ॉर्मेट में डेटा निर्यात करने की कार्यक्षमता प्रदान करता है।"
type: docs
weight: 650
url: /hi/net/groupdocs.parser.export/jsonexporter/
---

## JsonExporter class

JSON फ़ॉर्मेट में डेटा निर्यात करने की कार्यक्षमता प्रदान करता है।

```csharp
public sealed class JsonExporter : ExporterBase
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [JsonExporter](jsonexporter)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export)(DocumentData, Stream) | दस्तावेज़ डेटा को स्ट्रीम में निर्यात करता है। |
| [Export](../../groupdocs.parser.export/exporterbase/export)(DocumentData, string) | दस्तावेज़ डेटा को फ़ाइल में निर्यात करता है। |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_2)(IDocumentInfo, Stream) | दस्तावेज़ जानकारी को स्ट्रीम में निर्यात करता है। |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IDocumentInfo, string) | दस्तावेज़ जानकारी को फ़ाइल में निर्यात करता है। |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_4)(IEnumerable&lt;MetadataItem&gt;, Stream) | मेटाडेटा संग्रह को स्ट्रीम में निर्यात करता है। |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;MetadataItem&gt;, string) | मेटाडेटा संग्रह को फ़ाइल में निर्यात करता है। |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_6)(IEnumerable&lt;PageBarcodeArea&gt;, Stream) | बारकोड संग्रह को स्ट्रीम में निर्यात करता है। |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageBarcodeArea&gt;, string) | बारकोड संग्रह को फ़ाइल में निर्यात करता है। |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_8)(IEnumerable&lt;PageTableArea&gt;, Stream) | टेबल्स संग्रह को स्ट्रीम में निर्यात करता है। |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTableArea&gt;, string) | टेबल्स संग्रह को फ़ाइल में निर्यात करता है। |
| override [Export](../../groupdocs.parser.export/jsonexporter/export#export_10)(IEnumerable&lt;PageTextArea&gt;, Stream) | टेक्स्ट एरिया संग्रह को स्ट्रीम में निर्यात करता है। |
| [Export](../../groupdocs.parser.export/exporterbase/export)(IEnumerable&lt;PageTextArea&gt;, string) | टेक्स्ट एरिया संग्रह को फ़ाइल में निर्यात करता है। |

### संबंधित देखें

* class [ExporterBase](../exporterbase)
* namespace [GroupDocs.Parser.Export](../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
