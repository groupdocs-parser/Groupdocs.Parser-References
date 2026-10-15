---
title: "GetAnnotations"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से एनोटेशन निकालता है। नोट करें कि वर्तमान में केवल PDF फ़ॉर्मेट समर्थित है।"
type: docs
weight: 60
url: /hi/net/groupdocs.parser/parser/getannotations/
---

## GetAnnotations() {#getannotations}

दस्तावेज़ से एनोटेशन निकालता है। नोट करें कि वर्तमान में केवल PDF फ़ॉर्मेट समर्थित है।

```csharp
public IEnumerable<AnnotationItem> GetAnnotations()
```

### रिटर्न वैल्यू

एनोटेशन आइटम्स का संग्रह; यदि एनोटेशन निष्कर्षण समर्थित नहीं है तो `null`।

### संबंधित देखें

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetAnnotations(int) {#getannotations_1}

दस्तावेज़ पृष्ठ से एनोटेशन निकालता है। नोट करें कि वर्तमान में केवल PDF फ़ॉर्मेट समर्थित है।

```csharp
public IEnumerable<AnnotationItem> GetAnnotations(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |

### रिटर्न वैल्यू

एनोटेशन आइटम्स का संग्रह; यदि एनोटेशन निष्कर्षण समर्थित नहीं है तो `null`।

### संबंधित देखें

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
