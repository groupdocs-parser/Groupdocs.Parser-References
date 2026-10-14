---
title: "FieldData"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل بيانات الحقل مثل الاسم وفهرس الصفحة وقيمة الحقل وما إلى ذلك."
type: docs
weight: 13
url: /ar/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

يمثل بيانات الحقل مثل الاسم، وفهرس الصفحة، وقيمة الحقل وما إلى ذلك. اعتمادًا على الحقل قد تكون القيمة نصًا أو صورة أو جدولًا وما إلى ذلك.

تُستخدم كائنات فئة [FieldData](../../com.groupdocs.parser.data/fielddata) في مجموعة [DocumentData](../../com.groupdocs.parser.data/documentdata).

## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getName()](#getName--) | يحصل على اسم الحقل. |
|
|  | [getPageIndex()](#getPageIndex--) | يحصل على فهرس الصفحة. |
|
|  | [getPageArea()](#getPageArea--) | يحصل على قيمة الحقل. |
|
|  | [getLinkedField()](#getLinkedField--) | يحصل على الحقل المرتبط. |
|
|  | [getText()](#getText--) | يحصل على النص. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | يحصل على قيمة تشير إلى ما إذا كان  Name  قد تم تحويله إلى UPPER CASE. |
|
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الحقل.


**Returns:**
java.lang.String - قيمة سلسلة بأحرف كبيرة تمثل اسم الحقل.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


يحصل على فهرس الصفحة.


**Returns:**
int - فهرس يبدأ من الصفر للصفحة التي تحتوي على الحقل.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


يحصل على قيمة الحقل.

اعتمادًا على الحقل، قد تحتوي خاصية PageArea على أي من المشتقات لفئة [PageArea](../../com.groupdocs.parser.data/pagearea).
على سبيل المثال، طريقة [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) تستخرج حقول النص فقط.

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


يحصل على الحقل المرتبط.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


يحصل على النص.


**Returns:**
java.lang.String - قيمة سلسلة تمثل قيمة نص الحقل؛ null إذا لم تكن خاصية [PageArea](../../com.groupdocs.parser.data/pagearea) هي [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


يحصل على قيمة تشير إلى ما إذا كان  Name  قد تم تحويله إلى UPPER CASE.


**Returns:**
boolean - قيمة منطقية تشير إلى ما إذا كان  Name  قد تم تحويله إلى UPPER CASE.

