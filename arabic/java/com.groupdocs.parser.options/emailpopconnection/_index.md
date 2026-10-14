---
title: "EmailPopConnection"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل معلومات اتصال البريد الإلكتروني لبروتوكول POP."
type: docs
weight: 15
url: /ar/java/com.groupdocs.parser.options/emailpopconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailPopConnection extends EmailConnection
```

يمثل معلومات اتصال البريد الإلكتروني لبروتوكول POP.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [EmailPopConnection(String host, int port, String userName, String password)](#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-) | ينشئ مثلاً جديداً من الفئة [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getHost()](#getHost--) | يحصل على اسم المضيف. |
|
|  | [getPort()](#getPort--) | يحصل على رقم المنفذ. |
|
### EmailPopConnection(String host, int port, String userName, String password) {#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailPopConnection(String host, int port, String userName, String password)
```


ينشئ مثلاً جديداً من الفئة [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | host | java.lang.String | اسم المضيف. |
|
|  | port | int | رقم المنفذ. |
|
|  | userName | java.lang.String | اسم المستخدم. |
|
|  | كلمة المرور | java.lang.String | كلمة المرور. |
|

### getHost() {#getHost--}
```
public String getHost()
```


يحصل على اسم المضيف.


**Returns:**
java.lang.String - قيمة سلسلة تمثل اسم المضيف.

### getPort() {#getPort--}
```
public int getPort()
```


يحصل على رقم المنفذ.


**Returns:**
int - قيمة عددية صحيحة تمثل رقم المنفذ.

