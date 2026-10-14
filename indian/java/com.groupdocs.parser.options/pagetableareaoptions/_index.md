---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "पेज टेबल एरिया निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
weight: 31
url: /hi/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

पेज टेबल एरिया निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | नए [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) वर्ग का एक नया उदाहरण आरंभ करता है। |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | एक खोज आयत और बिना स्थिर लेआउट के [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) वर्ग का नया उदाहरण आरंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | पृष्ठ पर तालिका को परिभाषित करने वाले तालिका लेआउट को प्राप्त करता है। |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


नए [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) वर्ग का एक नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | पृष्ठ पर तालिका को परिभाषित करने वाला तालिका लेआउट। |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


एक खोज आयत और बिना स्थिर लेआउट के [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) वर्ग का नया उदाहरण आरंभ करता है।

पृष्ठ के एक क्षेत्र तक स्वचालित रूप से पहचानी गई तालिकाओं को सीमित करने के लिए उपयोगी। C# को प्रतिबिंबित करता है।

new PageTableAreaOptions(null) { Rectangle = ... }
पैटर्न।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | पृष्ठ पर वह आयताकार क्षेत्र जहाँ तालिकाओं का पता लगाया जाना चाहिए; पूरे पृष्ठ को खोजने के लिए  null  पास करें। |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


पृष्ठ पर तालिका को परिभाषित करने वाले तालिका लेआउट को प्राप्त करता है।


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

