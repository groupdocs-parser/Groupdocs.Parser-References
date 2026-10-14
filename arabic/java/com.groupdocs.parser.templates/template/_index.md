---
title: "Template"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر قالب صفحة المستند."
type: docs
weight: 10
url: /ar/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

يوفر قالب صفحة المستند. يتكون من كائنات [TemplateItem](../../com.groupdocs.parser.templates/templateitem) التي تمثل عناصر القالب مثل حقول النص وتعريفات الجداول.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | يقوم بتهيئة نسخة جديدة من الفئة [Template](../../com.groupdocs.parser.templates/template). |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | يقوم بتهيئة نسخة جديدة من الفئة [Template](../../com.groupdocs.parser.templates/template). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getCount()](#getCount--) | يحصل على العدد الإجمالي لعناصر القالب. |
|
|  | [get(int index)](#get-int-) | يحصل على عنصر القالب بواسطة الفهرس. |
|
|  | [getOptions()](#getOptions--) | يحصل على خيارات القالب. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | يقوم بتحميل قالب من ملف. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | يقوم بتحميل قالب من تدفق. |
|
|  | [save(String filePath)](#save-java.lang.String-) | يقوم بحفظ قالب إلى ملف. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | يقوم بحفظ قالب إلى تدفق. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


يقوم بتهيئة نسخة جديدة من الفئة [Template](../../com.groupdocs.parser.templates/template).

الاستخدام:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | مجموعة كائنات [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


يقوم بتهيئة نسخة جديدة من الفئة [Template](../../com.groupdocs.parser.templates/template).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | مجموعة كائنات [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | خيارات القالب. |
|

### getCount() {#getCount--}
```
public int getCount()
```


يحصل على العدد الإجمالي لعناصر القالب.


**Returns:**
int - عدد صحيح يمثل العدد الإجمالي لعناصر القالب.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


يحصل على عنصر القالب بواسطة الفهرس.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الفهرس | int | الفهرس الصفري لعنصر القالب. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


يحصل على خيارات القالب.


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


يقوم بتحميل قالب من ملف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


يقوم بتحميل قالب من تدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | stream | java.io.InputStream | تدفق الإدخال. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


يقوم بحفظ قالب إلى ملف.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار إلى الملف. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


يقوم بحفظ قالب إلى تدفق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | stream | java.io.OutputStream | دفق الإخراج. |
|

