---
title: "TemplateRegexPosition"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر موضع حقل القالب الذي يستخدم التعبير النمطي."
type: docs
weight: 19
url: /ar/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

يوفر موضع حقل القالب الذي يستخدم التعبير النمطي.

المثال التالي يوضح الحالة إذا كان المستند يحتوي على "Invoice Number INV-12345"
يمكن تعريف حقل القالب بالطريقة التالية:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

في هذه الحالة يتم استخراج السلسلة بالكامل كقيمة. لاستخراج جزء فقط من السلسلة
يتم استخدام مجموعة التعبير النمطي "value":

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

في هذه الحالة يتم استخراج السلسلة "INV-3337" كقيمة.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | ينشئ مثيلاً جديداً للفئة [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | ينشئ مثيلاً جديداً للفئة [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getExpression()](#getExpression--) | يحصل على التعبير النمطي. |
|
|  | [isMatchCase()](#isMatchCase--) | يحصل على القيمة التي تشير إلى ما إذا كانت حالة النص غير متجاهلة. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


ينشئ مثيلاً جديداً للفئة [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | التعبير | java.lang.String | التعبير النمطي. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


ينشئ مثيلاً جديداً للفئة [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | التعبير | java.lang.String | التعبير النمطي. |
|
|  | مطابقة الحالة | boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


يحصل على التعبير النمطي.


**Returns:**
java.lang.String - سلسلة تمثل التعبير النمطي.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


يحصل على القيمة التي تشير إلى ما إذا كانت حالة النص غير متجاهلة.


**Returns:**
boolean -  true  إذا لم يتم تجاهل حالة النص؛ وإلا،  false .

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


ينشئ نسخة من الموضع الحالي مع تعديل جميع الإحداثيات وفق العامل المحدد.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
| العامل | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
