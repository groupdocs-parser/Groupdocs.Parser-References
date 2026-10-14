---
title: "TemplateLinkedPositionEdges"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر حواف الحقل المرتبط حيث يتم البحث عن حقل النص."
type: docs
weight: 16
url: /ar/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

يوفر حواف الحقل المرتبط حيث يتم البحث عن حقل النص. يُستخدم [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) في فئة [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | يُنشئ مثيلًا جديدًا من فئة [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | يحصل على القيمة التي تشير إلى ما إذا كان المثيل فارغًا. |
|
|  | [isLeft()](#isLeft--) | يحصل على القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من اليسار بالنسبة إلى الحقل المرتبط. |
|
|  | [isTop()](#isTop--) | يحصل على القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من الأعلى بالنسبة إلى الحقل المرتبط. |
|
|  | [isRight()](#isRight--) | يحصل على القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من اليمين بالنسبة إلى الحقل المرتبط. |
|
|  | [isBottom()](#isBottom--) | يحصل على القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من الأسفل بالنسبة إلى الحقل المرتبط. |
|
|  | [parse(String s)](#parse-java.lang.String-) | يحوّل تمثيل السلسلة للنص الحواف إلى ما يعادلها من الفئة. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


يُنشئ مثيلًا جديدًا من فئة [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | اليسار | boolean | القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من اليسار بالنسبة إلى الحقل المرتبط. |
|
|  | الأعلى | boolean | القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من الأعلى بالنسبة إلى الحقل المرتبط. |
|
|  | يمين | boolean | القيمة التي تشير إلى ما إذا كان يتم البحث عن الحقل من اليمين بالنسبة للحقل المرتبط. |
|
|  | أسفل | boolean | القيمة التي تشير إلى ما إذا كان يتم البحث عن الحقل من الأسفل بالنسبة للحقل المرتبط. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


يحصل على القيمة التي تشير إلى ما إذا كان المثيل فارغًا.


**Returns:**
boolean -  true  إذا كانت الحالة فارغة (جميع الحقول هي false)؛ وإلا، false.

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


يحصل على القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من اليسار بالنسبة إلى الحقل المرتبط.


**Returns:**
boolean -  true  إذا تم البحث عن الحقل من اليسار بالنسبة للحقل المرتبط؛ وإلا، false.

### isTop() {#isTop--}
```
public boolean isTop()
```


يحصل على القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من الأعلى بالنسبة إلى الحقل المرتبط.


**Returns:**
boolean -  true  إذا تم البحث عن الحقل من الأعلى بالنسبة للحقل المرتبط؛ وإلا، false.

### isRight() {#isRight--}
```
public boolean isRight()
```


يحصل على القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من اليمين بالنسبة إلى الحقل المرتبط.


**Returns:**
boolean -  true  إذا تم البحث عن الحقل من اليمين بالنسبة للحقل المرتبط؛ وإلا، false.

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


يحصل على القيمة التي تشير إلى ما إذا كان الحقل يُبحث عنه من الأسفل بالنسبة إلى الحقل المرتبط.


**Returns:**
boolean -  true  إذا تم البحث عن الحقل من الأسفل بالنسبة للحقل المرتبط؛ وإلا، false.

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


يحوّل تمثيل السلسلة للنص الحواف إلى ما يعادلها من الفئة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | s | java.lang.String | سلسلة نصية تحتوي على الحواف للتحويل. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
