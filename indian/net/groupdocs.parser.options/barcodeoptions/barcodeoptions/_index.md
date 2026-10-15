---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "डिफ़ॉल्ट मानों के साथ BarcodeOptionsgroupdocs.parser.options/barcodeoptions वर्ग का नया उदाहरण आरंभ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.options/barcodeoptions/barcodeoptions/
---

## BarcodeOptions() {#constructor}

[`BarcodeOptions`](../../barcodeoptions) वर्ग का नया उदाहरण डिफ़ॉल्ट मानों के साथ आरंभ करता है।

```csharp
public BarcodeOptions()
```

### संबंधित देखें

* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle) {#constructor_1}

[`BarcodeOptions`](../../barcodeoptions) वर्ग का नया उदाहरण आयताकार क्षेत्र के साथ आरंभ करता है।

```csharp
public BarcodeOptions(Rectangle rectangle)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rectangle | Rectangle | आयताकार क्षेत्र जिसमें बारकोड होते हैं। |

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(QualityMode, QualityMode, params string[]) {#constructor_3}

एक नया उदाहरण प्रारंभ करता है [`BarcodeOptions`](../../barcodeoptions) क्लास का, गुणवत्ता सेटिंग्स और कोड प्रकारों के साथ।

```csharp
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, 
    params string[] codeTypes)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| imageQuality | QualityMode | स्रोत छवि की गुणवत्ता। |
| barcodeQuality | QualityMode | स्रोत बारकोड की गुणवत्ता। |
| codeTypes | String[] | पढ़ने के लिए बारकोड के प्रकार। |

### संबंधित देखें

* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## BarcodeOptions(Rectangle, QualityMode, QualityMode, float?, bool, params string[]) {#constructor_2}

एक नया उदाहरण प्रारंभ करता है [`BarcodeOptions`](../../barcodeoptions) क्लास का।

```csharp
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, 
    float? dimension, bool allowIncorrectBarcodes, params string[] codeTypes)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| rectangle | Rectangle | आयताकार क्षेत्र जिसमें बारकोड होते हैं। |
| imageQuality | QualityMode | स्रोत छवि की गुणवत्ता। |
| barcodeQuality | QualityMode | स्रोत बारकोड की गुणवत्ता। |
| dimension | Nullable`1 | बारकोड न्यूनतम तत्व का न्यूनतम आकार। |
| allowIncorrectBarcodes | Boolean | वह मान जो दर्शाता है कि गलत बारकोड की अनुमति है या नहीं। |
| codeTypes | String[] | पढ़ने के लिए बारकोड के प्रकार। |

### संबंधित देखें

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* enum [QualityMode](../../qualitymode)
* class [BarcodeOptions](../../barcodeoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
