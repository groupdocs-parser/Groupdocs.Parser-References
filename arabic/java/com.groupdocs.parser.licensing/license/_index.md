---
title: "الرخصة"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل ترخيص GroupDocs.Parser."
type: docs
weight: 10
url: /ar/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

يمثل ترخيص GroupDocs.Parser.

يوضح هذا المثال كيفية إعداد الرخصة.

````
 ```

// تهيئة فئة الرخصة
License license = new License();
// حدد المسار إلى ملف .lic
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [License()](#License--) | يُنشئ مثيلاً جديدًا من الفئة [License](../../com.groupdocs.parser.licensing/license). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | يرخص المكوّن. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | يرخص المكوّن. |
|
### License() {#License--}
```
public License()
```


يُنشئ مثيلاً جديدًا من الفئة [License](../../com.groupdocs.parser.licensing/license).


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


يرخص المكوّن.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار المطلق إلى ملف الترخيص. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


يرخص المكوّن.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | stream | java.io.InputStream | دفق الترخيص. |
|

