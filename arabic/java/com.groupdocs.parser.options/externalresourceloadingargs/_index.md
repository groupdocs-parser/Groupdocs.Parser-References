---
title: "ExternalResourceLoadingArgs"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر البيانات للطريقة."
type: docs
weight: 17
url: /ar/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

يوفر البيانات للطريقة [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-).

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | ينشئ مثيلاً جديداً للفئة [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) مع مساحة مستطيلة. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getUri()](#getUri--) | يحصل على URI للمورد الخارجي. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | يحصل على URI للمورد الخارجي. |
|
|  | [isSkipped()](#isSkipped--) | يحصل على القيمة التي تشير إلى ما إذا كان يجب تخطي تحميل المورد الخارجي. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | يضبط القيمة التي تشير إلى ما إذا كان يجب تخطي تحميل المورد الخارجي. |
|
|  | [getData()](#getData--) | يحصل على بيانات المستخدم. |
|
|  | [setData(byte[] data)](#setData-byte---) | يضبط بيانات المستخدم. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


ينشئ مثيلاً جديداً للفئة [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) مع مساحة مستطيلة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | uri | java.lang.String | URI للمورد الخارجي. |
|

### getUri() {#getUri--}
```
public String getUri()
```


يحصل على URI للمورد الخارجي.


**Returns:**
java.lang.String - قيمة سلسلة تمثل URI للمورد الخارجي.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


يحصل على URI للمورد الخارجي.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | uri | java.lang.String | قيمة سلسلة تمثل URI جديد للمورد الخارجي. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


يحصل على القيمة التي تشير إلى ما إذا كان يجب تخطي تحميل المورد الخارجي.


**Returns:**
boolean - صحيح إذا كان يجب تخطي تحميل المورد الخارجي؛ وإلا، خطأ.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


يضبط القيمة التي تشير إلى ما إذا كان يجب تخطي تحميل المورد الخارجي.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | متخطى | boolean | صحيح إذا كان يجب تخطي تحميل المورد الخارجي؛ وإلا، خطأ. |
|

### getData() {#getData--}
```
public byte[] getData()
```


يحصل على بيانات المستخدم.


**Returns:**
byte[] - مصفوفة البايتات التي تحتوي على محتوى المستخدم للمورد الخارجي. null إذا لم يتم تعيينها.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


يضبط بيانات المستخدم.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | بيانات | byte[] | مصفوفة البايت التي تحتوي على محتوى المستخدم للمورد الخارجي. null إذا لم يتم تعيينه. |
|

