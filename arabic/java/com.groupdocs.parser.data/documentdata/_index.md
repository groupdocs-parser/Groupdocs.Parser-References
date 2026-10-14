---
title: "DocumentData"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل بيانات المستند."
type: docs
weight: 11
url: /ar/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

يمثل بيانات المستند. يتكون من كائنات [FieldData](../../com.groupdocs.parser.data/fielddata) التي تحتوي على بيانات الحقول من المستند. يتم استخدام نسخة من فئة [DocumentData](../../com.groupdocs.parser.data/documentdata) كقيمة إرجاع لطرق [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) و [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) . راجع أمثلة الاستخدام هناك.

## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | يحصل على القالب الذي أنشأ بيانات هذا المستند. |
|
|  | [getCount()](#getCount--) | يحصل على العدد الإجمالي لبيانات الحقول. |
|
|  | [get(int index)](#get-int-) | يحصل على بيانات الحقل حسب الفهرس. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | يرجع مجموعة بيانات الحقول حيث يكون الاسم مساويًا لـ  fieldName . |
|
|  | [iterator()](#iterator--) | يرجع مكرّرًا للعناصر في هذه القائمة بالترتيب الصحيح. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


يحصل على القالب الذي أنشأ بيانات هذا المستند.

عندما تم إنتاج البيانات بواسطة اختيار مجموعة القوالب التلقائي (انظر
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
هذا هو القالب المحدد.
null
عندما لم يتم إنتاج البيانات بواسطة قالب.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


يحصل على العدد الإجمالي لبيانات الحقول.


**Returns:**
int - قيمة عددية تمثل إجمالي عدد بيانات الحقول.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


يحصل على بيانات الحقل حسب الفهرس.

التكرار عبر جميع الحقول:

````
// Print all extracted data
 for (int i = 0; i < data.getCount(); i++) {
     // Print field name
     System.out.print(data.get(i).getName() + ": ");
     // As we have defined only text fields in the template,
     // we cast PageArea property value to PageTextArea
     PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
             ? (PageTextArea) data.get(i).getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field PageArea property can contain any
من ورثة فئة [PageArea](../../com.groupdocs.parser.data/pagearea). على سبيل المثال، طريقة [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) تستخرج حقول النص فقط:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleFormsPdf)) {
     // Extract data from PDF document
     DocumentData data = parser.parseForm();
     // Check if form extraction is supported
     if (data == null) {
         System.out.println("Form extraction isn't supported.");
         return;
     }
     // Iterate over extracted data
     for (int i = 0; i < data.getCount(); i++) {
         System.out.print(data.get(i).getName() + ": ");
         PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
                 ? (PageTextArea) data.get(i).getPageArea()
                 : null;
         System.out.println(area == null ? "Not a template field" : area.getText());
     }
 }
 
````



**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الفهرس | int | الفهرس الصفري للحقول. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


يرجع مجموعة بيانات الحقول حيث يكون الاسم مساويًا لـ  fieldName .

ابحث عن الحقول بواسطة اسم الحقل:

````
// Print prices
 System.out.println("Prices:");
 for (FieldData field : data.getFieldsByName("Price")) {
     PageTextArea area = field.getPageArea() instanceof PageTextArea
             ? (PageTextArea) field.getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain
أي من ورثة فئة [PageArea](../../com.groupdocs.parser.data/pagearea). على سبيل المثال، طريقة [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) تستخرج حقول النص فقط.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | fieldName | java.lang.String | اسم الحقل. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - مجموعة من كائنات [FieldData](../../com.groupdocs.parser.data/fielddata)؛ مجموعة فارغة إذا لم يتم العثور على بيانات الحقل.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


يرجع مكرّرًا للعناصر في هذه القائمة بالترتيب الصحيح.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - مكرّر على العناصر في هذه القائمة بالتسلسل الصحيح.

