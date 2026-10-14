---
title: "TocItem"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل العنصر الذي يُستخدم في وظيفة استخراج جدول المحتويات."
type: docs
weight: 31
url: /ar/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

يمثل العنصر الذي يُستخدم في وظيفة استخراج جدول المحتويات.

يتم استخدام كائن من فئة [TocItem](../../com.groupdocs.parser.data/tocitem) كقيمة إرجاع لطريقة [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) . راجع أمثلة الاستخدام هناك.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | ينشئ مثيلاً جديداً من فئة TocItem. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getDepth()](#getDepth--) | يحصل على مستوى العمق. |
|
|  | [getText()](#getText--) | يحصل على النص. |
|
|  | [getPageIndex()](#getPageIndex--) | يحصل على فهرس الصفحة. |
|
|  | [extractText()](#extractText--) | يستخرج نصاً من المستند الذي يشير إليه كائن TocItem. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


ينشئ مثيلاً جديداً من فئة TocItem.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | العمق | int | مستوى العمق للعنصر. |
|
|  | text | java.lang.String | نص العنصر. |
|
|  | pageIndex | java.lang.Integer | فهرس الصفحة التي يشير إليها العنصر |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


يحصل على مستوى العمق.


**Returns:**
int - قيمة عددية تمثل مستوى العمق للعنصر.

### getText() {#getText--}
```
public String getText()
```


يحصل على النص.


**Returns:**
java.lang.String - قيمة نصية تمثل نص العنصر.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


يحصل على فهرس الصفحة.


**Returns:**
java.lang.Integer - قيمة عددية تمثل فهرس الصفحة التي يشير إليها العنصر؛  null  إذا لم يتم تعيينه.

### extractText() {#extractText--}
```
public TextReader extractText()
```


يستخرج نصاً من المستند الذي يشير إليه كائن TocItem.

المثال التالي يوضح كيفية استخراج نص بواسطة عنصر من جدول المحتويات:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.

