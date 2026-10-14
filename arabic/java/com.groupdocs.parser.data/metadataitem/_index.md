---
title: "MetadataItem"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل عنصر بيانات تعريف يُستخدم في عناصر الحاوية ووظيفة استخراج البيانات التعريفية."
type: docs
weight: 15
url: /ar/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

يمثل عنصر بيانات تعريف يُستخدم في عناصر الحاوية ووظيفة استخراج البيانات التعريفية.

يُستخدم كائن من فئة [MetadataItem](../../com.groupdocs.parser.data/metadataitem) كقيمة إرجاع لطريقة [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--).
وكعنصر في مجموعة [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--) . راجع أمثلة الاستخدام هناك.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | ينشئ كائنًا جديدًا من فئة [MetadataItem](../../com.groupdocs.parser.data/metadataitem). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getName()](#getName--) | يحصل على اسم عنصر البيانات الوصفية. |
|
|  | [getValue()](#getValue--) | يحصل على قيمة عنصر البيانات الوصفية. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


ينشئ كائنًا جديدًا من فئة [MetadataItem](../../com.groupdocs.parser.data/metadataitem).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الاسم | java.lang.String | اسم عنصر البيانات الوصفية. |
|
|  | القيمة | java.lang.String | قيمة عنصر البيانات الوصفية. |
|

### getName() {#getName--}
```
public String getName()
```


يحصل على اسم عنصر البيانات الوصفية.


**Returns:**
java.lang.String - قيمة سلسلة تمثل اسم عنصر البيانات الوصفية.

### getValue() {#getValue--}
```
public String getValue()
```


يحصل على قيمة عنصر البيانات الوصفية.


**Returns:**
java.lang.String - قيمة سلسلة تمثل قيمة عنصر البيانات الوصفية.

