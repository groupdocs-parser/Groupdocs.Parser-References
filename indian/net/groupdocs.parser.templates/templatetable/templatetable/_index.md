---
title: "TemplateTable"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "UPPER CASE नाम के साथ TemplateTablegroupdocs.parser.templates/templatetable क्लास का नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

UPPER CASE नाम के साथ [`TemplateTable`](../../templatetable) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| layout | TemplateTableLayout | टेबल लेआउट। |
| name | स्ट्रिंग | टेबल का नाम। |

### Examples

यदि टेबल को स्वचालित रूप से पता नहीं लगाया जा सकता, तो टेबल लेआउट द्वारा टेम्प्लेट टेबल सेट किया जाता है:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// एक दस्तावेज़ टेम्प्लेट बनाएं
Template template = new Template(new TemplateItem[] { table });
```

### संबंधित देखें

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

UPPER CASE नाम के साथ [`TemplateTable`](../../templatetable) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| layout | TemplateTableLayout | टेबल लेआउट। |
| name | स्ट्रिंग | टेबल का नाम। |
| pageWidth | Nullable`1 | टेम्प्लेट आइटम बनाने के लिए उपयोग किए गए पृष्ठ की चौड़ाई। |

### Examples

यदि टेबल को स्वचालित रूप से पता नहीं लगाया जा सकता, तो टेबल लेआउट द्वारा टेम्प्लेट टेबल सेट किया जाता है:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// एक दस्तावेज़ टेम्प्लेट बनाएं
Template template = new Template(new TemplateItem[] { table });
```

### संबंधित देखें

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

नया उदाहरण प्रारंभ करता है [`TemplateTable`](../../templatetable) क्लास का।

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| layout | TemplateTableLayout | टेबल लेआउट। |
| name | स्ट्रिंग | टेबल का नाम। |
| pageWidth | Nullable`1 | टेम्प्लेट आइटम बनाने के लिए उपयोग किए गए पृष्ठ की चौड़ाई। |
| useUpperCaseName | Boolean | वह मान जो दर्शाता है कि `name` को UPPER CASE में बदला गया है। |

### Examples

यदि टेबल को स्वचालित रूप से पता नहीं लगाया जा सकता, तो टेबल लेआउट द्वारा टेम्प्लेट टेबल सेट किया जाता है:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// एक दस्तावेज़ टेम्प्लेट बनाएं
Template template = new Template(new TemplateItem[] { table });
```

### संबंधित देखें

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

नया उदाहरण प्रारंभ करता है [`TemplateTable`](../../templatetable) क्लास का।

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| पैरामीटर | TemplateTableParameters | स्वचालित मोड में तालिका का पता लगाने के लिए पैरामीटर। |
| name | स्ट्रिंग | टेबल का नाम। |

### Examples

यदि डिटेक्टर पैरामीटर द्वारा टेम्प्लेट टेबल सेट किया गया है, तो टेबल स्वचालित रूप से पता लगाई जाती है:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// एक दस्तावेज़ टेम्प्लेट बनाएं
Template template = new Template(new TemplateItem[] { table });
```

### संबंधित देखें

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

नया उदाहरण प्रारंभ करता है [`TemplateTable`](../../templatetable) क्लास का।

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| पैरामीटर | TemplateTableParameters | स्वचालित मोड में तालिका का पता लगाने के लिए पैरामीटर। |
| name | स्ट्रिंग | टेबल का नाम। |
| pageWidth | Nullable`1 | टेम्प्लेट आइटम बनाने के लिए उपयोग किए गए पृष्ठ की चौड़ाई। |

### Examples

यदि डिटेक्टर पैरामीटर द्वारा टेम्प्लेट टेबल सेट किया गया है, तो टेबल स्वचालित रूप से पता लगाई जाती है:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// एक दस्तावेज़ टेम्प्लेट बनाएं
Template template = new Template(new TemplateItem[] { table });
```

### संबंधित देखें

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

नया उदाहरण प्रारंभ करता है [`TemplateTable`](../../templatetable) क्लास का।

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| पैरामीटर | TemplateTableParameters | स्वचालित मोड में तालिका का पता लगाने के लिए पैरामीटर। |
| name | स्ट्रिंग | टेबल का नाम। |
| pageWidth | Nullable`1 | टेम्प्लेट आइटम बनाने के लिए उपयोग किए गए पृष्ठ की चौड़ाई। |
| useUpperCaseName | Boolean | वह मान जो दर्शाता है कि `name` को UPPER CASE में बदला गया है। |

### Examples

यदि डिटेक्टर पैरामीटर द्वारा टेम्प्लेट टेबल सेट किया गया है, तो टेबल स्वचालित रूप से पता लगाई जाती है:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// एक दस्तावेज़ टेम्प्लेट बनाएं
Template template = new Template(new TemplateItem[] { table });
```

### संबंधित देखें

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
