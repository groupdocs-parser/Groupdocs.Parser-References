---
title: "Template"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "दस्तावेज़ पृष्ठ टेम्पलेट प्रदान करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

डॉक्यूमेंट पेज टेम्प्लेट प्रदान करता है। यह [TemplateItem](../../com.groupdocs.parser/templates/templateitem) ऑब्जेक्ट्स से बना होता है जो टेम्प्लेट के आइटम्स जैसे पाठ फ़ील्ड और तालिका परिभाषाओं का प्रतिनिधित्व करते हैं।

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | नया उदाहरण प्रारंभ करता है [Template](../../com.groupdocs.parser.templates/template) वर्ग का। |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | नया उदाहरण प्रारंभ करता है [Template](../../com.groupdocs.parser.templates/template) वर्ग का। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getCount()](#getCount--) | टेम्प्लेट आइटम्स की कुल संख्या प्राप्त करता है। |
|
|  | [get(int index)](#get-int-) | इंडेक्स द्वारा टेम्प्लेट आइटम प्राप्त करता है। |
|
|  | [getOptions()](#getOptions--) | टेम्प्लेट विकल्प प्राप्त करता है। |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | फ़ाइल से टेम्प्लेट लोड करता है। |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | स्ट्रीम से टेम्प्लेट लोड करता है। |
|
|  | [save(String filePath)](#save-java.lang.String-) | टेम्प्लेट को फ़ाइल में सहेजता है। |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | टेम्प्लेट को स्ट्रीम में सहेजता है। |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


नया उदाहरण प्रारंभ करता है [Template](../../com.groupdocs.parser.templates/template) वर्ग का।

उपयोग:

````
// Create an array of template fields
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
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(fields));
 
````



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | [TemplateItem](../../com.groupdocs.parser.templates/templateitem) ऑब्जेक्ट्स का संग्रह। |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


नया उदाहरण प्रारंभ करता है [Template](../../com.groupdocs.parser.templates/template) वर्ग का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | [TemplateItem](../../com.groupdocs.parser.templates/templateitem) ऑब्जेक्ट्स का संग्रह। |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | टेम्प्लेट विकल्प। |
|

### getCount() {#getCount--}
```
public int getCount()
```


टेम्प्लेट आइटम्स की कुल संख्या प्राप्त करता है।


**Returns:**
int - एक पूर्णांक जो टेम्प्लेट आइटम्स की कुल संख्या दर्शाता है।

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


इंडेक्स द्वारा टेम्प्लेट आइटम प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इंडेक्स | int | टेम्प्लेट आइटम का शून्य-आधारित इंडेक्स। |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


टेम्प्लेट विकल्प प्राप्त करता है।


**Returns:**
[TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) - An instance of [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) class.

### iterator() {#iterator--}
```
public Iterator<TemplateItem> iterator()
```




**Returns:**
java.util.Iterator<com.groupdocs.parser.templates.TemplateItem>
### load(String filePath) {#load-java.lang.String-}
```
public static Template load(String filePath)
```


फ़ाइल से टेम्प्लेट लोड करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


स्ट्रीम से टेम्प्लेट लोड करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | stream | java.io.InputStream | इनपुट स्ट्रीम। |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


टेम्प्लेट को फ़ाइल में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


टेम्प्लेट को स्ट्रीम में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | stream | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

