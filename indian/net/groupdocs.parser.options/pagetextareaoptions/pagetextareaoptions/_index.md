---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "OCR उपयोग विकल्प के साथ PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions क्लास का एक नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

OCR उपयोग विकल्प के साथ [`PageTextAreaOptions`](../../pagetextareaoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public PageTextAreaOptions()
```

### संबंधित देखें

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

OCR उपयोग विकल्प के साथ [`PageTextAreaOptions`](../../pagetextareaoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public PageTextAreaOptions(bool useOcr)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| useOcr | Boolean | वह मान जो दर्शाता है कि टेक्स्ट एरिया निकालने के लिए OCR कार्यक्षमता उपयोग की गई है या नहीं। |

### संबंधित देखें

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

OCR विकल्प सेट करने की क्षमता के साथ [`PageTextAreaOptions`](../../pagetextareaoptions) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| useOcr | Boolean | वह मान जो दर्शाता है कि टेक्स्ट एरिया निकालने के लिए OCR कार्यक्षमता उपयोग की गई है या नहीं। |
| ocrOptions | OcrOptions | OCR कार्यक्षमता के अतिरिक्त विकल्प। |

### संबंधित देखें

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

नियमित अभिव्यक्ति के साथ [`PageTextAreaOptions`](../../pagetextareaoptions) क्लास का एक नया उदाहरण प्रारंभ करता है। अन्य विकल्प डिफ़ॉल्ट रूप से सेट होते हैं (विवरण के लिए टिप्पणी देखें)।

```csharp
public PageTextAreaOptions(string expression)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| expression | स्ट्रिंग | नियमित अभिव्यक्ति। |

### टिप्पणियाँ

निम्नलिखित गुणों के डिफ़ॉल्ट मान हैं:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### संबंधित देखें

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

नियमित अभिव्यक्ति और आयताकार क्षेत्र के साथ [`PageTextAreaOptions`](../../pagetextareaoptions) वर्ग का नया उदाहरण आरंभ करता है। अन्य विकल्प डिफ़ॉल्ट रूप से सेट होते हैं (विवरण के लिए टिप्पणी देखें)।

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| expression | स्ट्रिंग | नियमित अभिव्यक्ति। |
| rectangle | Rectangle | पृष्ठ क्षेत्रों को समाहित करने वाला आयताकार क्षेत्र। |

### टिप्पणियाँ

निम्नलिखित गुणों के डिफ़ॉल्ट मान हैं:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

नियमित अभिव्यक्ति, आयताकार क्षेत्र और अनदेखी सीमा के आकार के साथ [`PageTextAreaOptions`](../../pagetextareaoptions) वर्ग का नया उदाहरण आरंभ करता है। अन्य विकल्प डिफ़ॉल्ट रूप से सेट होते हैं (विवरण के लिए टिप्पणी देखें)।

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| expression | स्ट्रिंग | नियमित अभिव्यक्ति। |
| rectangle | Rectangle | पृष्ठ क्षेत्रों को समाहित करने वाला आयताकार क्षेत्र। |
| rectangleTolerance | Double | आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखा किए जाने वाले बॉर्डर का आकार। यह पाठ आइटम की ऊँचाई के अंश द्वारा मापा जाता है। |

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

[`PageTextAreaOptions`](../../pagetextareaoptions) वर्ग का नया उदाहरण आरंभ करता है।

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| expression | स्ट्रिंग | नियमित अभिव्यक्ति। |
| matchCase | Boolean | वह मान जो दर्शाता है कि क्या पाठ केस को अनदेखा नहीं किया जाता है। |
| uniteSegments | Boolean | वह मान जो दर्शाता है कि क्या खंडों को मिलाया गया है। |
| ignoreFormatting | Boolean | वह मान जो दर्शाता है कि क्या पाठ स्वरूपण को अनदेखा किया जाता है। |
| rectangle | Rectangle | पृष्ठ क्षेत्रों को समाहित करने वाला आयताकार क्षेत्र। |

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

अनदेखी सीमा के आकार के साथ [`PageTextAreaOptions`](../../pagetextareaoptions) वर्ग का नया उदाहरण आरंभ करता है।

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| expression | स्ट्रिंग | नियमित अभिव्यक्ति। |
| matchCase | Boolean | वह मान जो दर्शाता है कि क्या पाठ केस को अनदेखा नहीं किया जाता है। |
| uniteSegments | Boolean | वह मान जो दर्शाता है कि क्या खंडों को मिलाया गया है। |
| ignoreFormatting | Boolean | वह मान जो दर्शाता है कि क्या पाठ स्वरूपण को अनदेखा किया जाता है। |
| rectangle | Rectangle | पृष्ठ क्षेत्रों को समाहित करने वाला आयताकार क्षेत्र। |
| rectangleTolerance | Double | आयताकार क्षेत्र द्वारा कैप्चर किए जाने पर अनदेखा किए जाने वाले बॉर्डर का आकार। यह पाठ आइटम की ऊँचाई के अंश द्वारा मापा जाता है। |

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
