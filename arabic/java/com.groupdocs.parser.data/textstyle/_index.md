---
title: "TextStyle"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل نمط النص مثل اسم الخط وحجم الخط وما إلى ذلك."
type: docs
weight: 30
url: /ar/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

يمثل نمط النص مثل اسم الخط، حجم الخط وما إلى ذلك.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | ينشئ مثيلاً جديداً من فئة [TextStyle](../../com.groupdocs.parser.data/textstyle). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getName()](#getName--) | يحصل على اسم النمط. |
|
|  | [getFontName()](#getFontName--) | يحصل على اسم الخط. |
|
|  | [getFontSize()](#getFontSize--) | يحصل على حجم الخط. |
|
|  | [isBold()](#isBold--) | يحصل على القيمة التي تشير إلى ما إذا كان الخط عريضًا. |
|
|  | [isItalic()](#isItalic--) | يحصل على القيمة التي تشير إلى ما إذا كان الخط مائلًا. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


ينشئ مثيلاً جديداً من فئة [TextStyle](../../com.groupdocs.parser.data/textstyle).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الاسم | java.lang.String | اسم النمط. |
|
|  | fontName | java.lang.String | اسم الخط. |
|
|  | fontSize | double | حجم الخط. |
|
|  | bold | boolean | القيمة التي تشير إلى ما إذا كان الخط عريضًا. |
|
|  | italic | boolean | القيمة التي تشير إلى ما إذا كان الخط مائلًا. |
|

### getName() {#getName--}
```
public String getName()
```


يحصل على اسم النمط.


**Returns:**
java.lang.String - قيمة سلسلة تمثل اسم النمط.

### getFontName() {#getFontName--}
```
public String getFontName()
```


يحصل على اسم الخط.


**Returns:**
java.lang.String - قيمة سلسلة تمثل اسم الخط.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


يحصل على حجم الخط.


**Returns:**
double - قيمة مزدوجة تمثل حجم الخط.

### isBold() {#isBold--}
```
public boolean isBold()
```


يحصل على القيمة التي تشير إلى ما إذا كان الخط عريضًا.


**Returns:**
boolean -  true  إذا كان الخط عريضًا؛ وإلا،  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


يحصل على القيمة التي تشير إلى ما إذا كان الخط مائلًا.


**Returns:**
boolean -  true  إذا كان الخط مائلًا؛ وإلا،  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
