---
title: "QualityMode"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يحدد مستوى الجودة."
type: docs
weight: 48
url: /ar/java/com.groupdocs.parser.options/qualitymode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum QualityMode extends Enum<QualityMode>
```

يحدد مستوى الجودة.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [High](#High) | جودة عالية. |
|
|  | [Normal](#Normal) | جودة عادية. |
|
|  | [Low](#Low) | جودة منخفضة. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### High {#High}
```
public static final QualityMode High
```


جودة عالية. يتم استخدام خوارزميات معالجة سريعة.


### Normal {#Normal}
```
public static final QualityMode Normal
```


جودة عادية. يتم استخدام خوارزميات المعالجة الافتراضية.


### Low {#Low}
```
public static final QualityMode Low
```


جودة منخفضة. يتم استخدام خوارزميات معالجة بطيئة.


### values() {#values--}
```
public static QualityMode[] values()
```




**Returns:**
com.groupdocs.parser.options.QualityMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static QualityMode valueOf(String name)
```




**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode)
