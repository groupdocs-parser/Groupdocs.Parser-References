---
title: "FormattedTextOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة لاستخراج النص المنسق."
type: docs
weight: 21
url: /ar/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

يوفر الخيارات المستخدمة لاستخراج النص المنسق.

يتم استخدام نسخة من الفئة [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) كمعامل في [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-)
و [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) الطرق. راجع أمثلة الاستخدام هناك.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | يُنشئ نسخة جديدة من الفئة [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) دون تعيين أي وضع. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | يُنشئ مثيلًا جديدًا من الفئة [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getMode()](#getMode--) | يحصل على وضع استخراج النص المنسق. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | يضبط وضع استخراج النص المنسق. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


يُنشئ نسخة جديدة من الفئة [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) دون تعيين أي وضع.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


يُنشئ مثيلًا جديدًا من الفئة [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | وضع استخراج النص المنسق. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


يحصل على وضع استخراج النص المنسق.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


يضبط وضع استخراج النص المنسق.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | تعداد [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) الذي يحتوي على وضع استخراج النص المنسق. |
|

