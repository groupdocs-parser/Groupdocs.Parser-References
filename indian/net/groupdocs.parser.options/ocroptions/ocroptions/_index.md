---
title: "OcrOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "आयताकार क्षेत्र के साथ OcrOptionsgroupdocs.parser.options/ocroptions क्लास का एक नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.options/ocroptions/ocroptions/
---

## OcrOptions() {#constructor}

[`OcrOptions`](../../ocroptions) क्लास का एक नया उदाहरण आयताकार क्षेत्र के साथ प्रारंभ करता है।

```csharp
public OcrOptions()
```

### संबंधित देखें

* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(PagePreviewOptions) {#constructor_6}

[`OcrOptions`](../../ocroptions) क्लास का एक नया उदाहरण आयताकार क्षेत्र के साथ प्रारंभ करता है।

```csharp
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pagePreviewOptions | PagePreviewOptions | [`PagePreviewOptions`](../pagepreviewoptions) क्लास का एक उदाहरण जो दस्तावेज़ पृष्ठ पूर्वावलोकन निर्माण के लिए गुण सेट करता है। |

### संबंधित देखें

* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle) {#constructor_1}

[`OcrOptions`](../../ocroptions) क्लास का एक नया उदाहरण आयताकार क्षेत्र के साथ प्रारंभ करता है।

```csharp
public OcrOptions(Rectangle rectangle)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rectangle | Rectangle | आयताकार क्षेत्र जो पृष्ठ क्षेत्र को सीमित करता है जिसका उपयोग पाठ पहचान के लिए किया जाता है। |

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(OcrEventHandler) {#constructor_5}

[`OcrOptions`](../../ocroptions) क्लास का एक नया उदाहरण [`OcrEventHandler`](../../ocreventhandler) ऑब्जेक्ट के साथ प्रारंभ करता है।

```csharp
public OcrOptions(OcrEventHandler handler)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| handler | OcrEventHandler | OCR घटनाओं को पकड़ने के लिए [`OcrEventHandler`](../../ocreventhandler) का एक उदाहरण। |

### संबंधित देखें

* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler) {#constructor_2}

`[`OcrOptions`](../../ocroptions)` वर्ग का एक नया उदाहरण आयताकार क्षेत्र और [`OcrEventHandler`](../../ocreventhandler) ऑब्जेक्ट के साथ प्रारंभ करता है।

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rectangle | Rectangle | आयताकार क्षेत्र जो पृष्ठ क्षेत्र को सीमित करता है जिसका उपयोग पाठ पहचान के लिए किया जाता है। |
| handler | OcrEventHandler | OCR घटनाओं को पकड़ने के लिए [`OcrEventHandler`](../../ocreventhandler) का एक उदाहरण। |

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool) {#constructor_3}

`[`OcrOptions`](../../ocroptions)` वर्ग का एक नया उदाहरण प्रारंभ करता है।

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rectangle | Rectangle | आयताकार क्षेत्र जो पृष्ठ क्षेत्र को सीमित करता है जिसका उपयोग पाठ पहचान के लिए किया जाता है। |
| handler | OcrEventHandler | OCR घटनाओं को पकड़ने के लिए [`OcrEventHandler`](../../ocreventhandler) का एक उदाहरण। |
| pagePreviewOptions | PagePreviewOptions | [`PagePreviewOptions`](../pagepreviewoptions) क्लास का एक उदाहरण जो दस्तावेज़ पृष्ठ पूर्वावलोकन निर्माण के लिए गुण सेट करता है। |
| useSpellCheker | Boolean | वह मान जो दर्शाता है कि स्पेल चेकर उपयोग किया गया है या नहीं। |

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) {#constructor_4}

`[`OcrOptions`](../../ocroptions)` वर्ग का एक नया उदाहरण प्रारंभ करता है।

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker, Language language)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rectangle | Rectangle | आयताकार क्षेत्र जो पृष्ठ क्षेत्र को सीमित करता है जिसका उपयोग पाठ पहचान के लिए किया जाता है। |
| handler | OcrEventHandler | OCR घटनाओं को पकड़ने के लिए [`OcrEventHandler`](../../ocreventhandler) का एक उदाहरण। |
| pagePreviewOptions | PagePreviewOptions | [`PagePreviewOptions`](../pagepreviewoptions) क्लास का एक उदाहरण जो दस्तावेज़ पृष्ठ पूर्वावलोकन निर्माण के लिए गुण सेट करता है। |
| useSpellCheker | Boolean | वह मान जो दर्शाता है कि स्पेल चेकर उपयोग किया गया है या नहीं। |
| language | भाषा | OCR के लिए उपयोग की गई भाषा। |

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* enum [Language](../../language)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
