---
title: "ExternalResourceHandler"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر معالجًا لتحميل الموارد الخارجية."
type: docs
weight: 16
url: /ar/java/com.groupdocs.parser.options/externalresourcehandler/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceHandler
```

يوفر معالجًا لتحميل الموارد الخارجية.

## البناؤات

| البناء | الوصف |
| --- | --- |
| [ExternalResourceHandler()](#ExternalResourceHandler--) |  |
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [onLoading(ExternalResourceLoadingArgs args)](#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-) | يتم استدعاؤه قبل تحميل أي مورد خارجي. |
|
### ExternalResourceHandler() {#ExternalResourceHandler--}
```
public ExternalResourceHandler()
```


### onLoading(ExternalResourceLoadingArgs args) {#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-}
```
public void onLoading(ExternalResourceLoadingArgs args)
```


يتم استدعاؤه قبل تحميل أي مورد خارجي.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | args | [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) | البيانات للتحكم في تحميل الموارد الخارجية. |
|

