---
title: "PageArea"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل فئة أساسية مجردة لمناطق الصفحة التي تُستخدم لتمثيل الكتل على صفحة المستند في وظيفة التحليل باستخدام القالب."
type: docs
weight: 17
url: /ar/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

يمثل فئة أساسية مجردة لمناطق الصفحة التي تُستخدم لتمثيل الكتل على صفحة المستند في وظيفة التحليل باستخدام القالب.

## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | يحصل على المنطقة المستطيلة. |
|
|  | [getPage()](#getPage--) | يحصل على معلومات صفحة المستند مثل فهرس الصفحة وحجم الصفحة. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


يحصل على المنطقة المستطيلة.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


يحصل على معلومات صفحة المستند مثل فهرس الصفحة وحجم الصفحة.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

