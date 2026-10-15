---
title: "टेम्पलेट"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "Templategroupdocs.parser.templates/template क्लास का एक नया उदाहरण आरंभ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.templates/template/template/
---

## Template(IEnumerable&lt;TemplateItem&gt;) {#constructor}

[`Template`](../../template) क्लास का एक नया उदाहरण आरंभ करता है।

```csharp
public Template(IEnumerable<TemplateItem> items)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| items | IEnumerable`1 | [`TemplateItem`](../../templateitem) ऑब्जेक्ट्स का संग्रह। |

### Examples

उपयोग:

```csharp
// टेम्प्लेट फ़ील्ड्स की एक एरे बनाएं
TemplateItem[] fields = new TemplateItem[]
{
   new TemplateField(new TemplateRegexPosition("From"), "From", 0),
   new TemplateField(
       new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromCompany",
       0),
   new TemplateField(
       new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
       "FromAddress",
       0)
};

// एक दस्तावेज़ टेम्प्लेट बनाएं
Template template = new Template(fields);
```

### संबंधित देखें

* class [TemplateItem](../../templateitem)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Template(IEnumerable&lt;TemplateItem&gt;, TemplateOptions) {#constructor_1}

[`Template`](../../template) क्लास का एक नया उदाहरण टेम्प्लेट विकल्पों के साथ आरंभ करता है।

```csharp
public Template(IEnumerable<TemplateItem> items, TemplateOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| items | IEnumerable`1 | [`TemplateItem`](../../templateitem) ऑब्जेक्ट्स का संग्रह। |
| options | TemplateOptions | टेम्प्लेट विकल्प। |

### संबंधित देखें

* class [TemplateItem](../../templateitem)
* class [TemplateOptions](../../templateoptions)
* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
