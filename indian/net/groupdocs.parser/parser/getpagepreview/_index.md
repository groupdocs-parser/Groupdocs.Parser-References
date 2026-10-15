---
title: "GetPagePreview"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ पृष्ठ का पूर्वावलोकन बनाता है।"
type: docs
weight: 150
url: /hi/net/groupdocs.parser/parser/getpagepreview/
---

## GetPagePreview(int) {#getpagepreview}

दस्तावेज़ पृष्ठ का पूर्वावलोकन बनाता है।

```csharp
public Stream GetPagePreview(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |

### रिटर्न वैल्यू

एक Stream का उदाहरण जिसमें दस्तावेज़ पृष्ठ की छवि होती है; `null` यदि पृष्ठ पूर्वावलोकन निर्माण समर्थित नहीं है।

### संबंधित देखें

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetPagePreview(int, PagePreviewOptions) {#getpagepreview_1}

कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ का पूर्वावलोकन बनाता है।

```csharp
public Stream GetPagePreview(int pageIndex, PagePreviewOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |
| options | PagePreviewOptions | पूर्वावलोकन निर्माण को अनुकूलित करने के विकल्प। |

### रिटर्न वैल्यू

एक Stream का उदाहरण जिसमें दस्तावेज़ पृष्ठ की छवि होती है; `null` यदि पृष्ठ पूर्वावलोकन निर्माण समर्थित नहीं है।

### संबंधित देखें

* class [PagePreviewOptions](../../../groupdocs.parser.options/pagepreviewoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
