---
title: "ParseByTemplate"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "उपयोगकर्ता‑जनित टेम्प्लेट द्वारा दस्तावेज़ को पार्स करता है।"
type: docs
weight: 230
url: /hi/net/groupdocs.parser/parser/parsebytemplate/
---

## ParseByTemplate(Template) {#parsebytemplate}

उपयोगकर्ता-निर्मित टेम्पलेट द्वारा दस्तावेज़ को पार्स करता है।

```csharp
public DocumentData ParseByTemplate(Template template)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| template | टेम्पलेट | उपयोगकर्ता‑जनित टेम्प्लेट। |

### रिटर्न वैल्यू

[`DocumentData`](../../../groupdocs.parser.data/documentdata) वर्ग का एक उदाहरण जो निकाले गए डेटा को रखता है; `null` यदि टेम्प्लेट द्वारा पार्सिंग समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### संबंधित देखें

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(Template, ParseByTemplateOptions) {#parsebytemplate_1}

उपयोगकर्ता-निर्मित टेम्पलेट द्वारा दस्तावेज़ को पार्स करता है, अनुकूलन विकल्पों का उपयोग करके।

```csharp
public DocumentData ParseByTemplate(Template template, ParseByTemplateOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| template | टेम्पलेट | उपयोगकर्ता‑जनित टेम्प्लेट। |
| options | ParseByTemplateOptions | कस्टमाइज़ेशन विकल्प। |

### रिटर्न वैल्यू

[`DocumentData`](../../../groupdocs.parser.data/documentdata) वर्ग का एक उदाहरण जो निकाले गए डेटा को रखता है; `null` यदि टेम्प्लेट द्वारा पार्सिंग समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### संबंधित देखें

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(TemplateCollection, ParseByTemplateOptions) {#parsebytemplate_2}

प्रदान किए गए संग्रह से सबसे उपयुक्त टेम्पलेट चुनता है और फिर चयनित टेम्पलेट के विरुद्ध दस्तावेज़ को पार्स करता है।

```csharp
public DocumentData ParseByTemplate(TemplateCollection templateCollection, 
    ParseByTemplateOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| templateCollection | TemplateCollection | टेम्प्लेट संग्रह। |
| options | ParseByTemplateOptions | कस्टमाइज़ेशन विकल्प। |

### रिटर्न वैल्यू

[`DocumentData`](../../../groupdocs.parser.data/documentdata) वर्ग का एक उदाहरण जो निकाले गए डेटा को रखता है; `null` यदि टेम्प्लेट द्वारा पार्सिंग समर्थित नहीं है।

### संबंधित देखें

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [TemplateCollection](../../../groupdocs.parser.templates/templatecollection)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
