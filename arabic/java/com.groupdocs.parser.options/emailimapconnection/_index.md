---
title: "EmailImapConnection"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل معلومات اتصال البريد الإلكتروني لبروتوكول IMAP."
type: docs
weight: 14
url: /ar/java/com.groupdocs.parser.options/emailimapconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailImapConnection extends EmailConnection
```

يمثل معلومات اتصال البريد الإلكتروني لبروتوكول IMAP.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [EmailImapConnection(String host, int port, String userName, String password)](#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-) | يقوم بإنشاء نسخة جديدة من الفئة [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getHost()](#getHost--) | يحصل على اسم المضيف. |
|
|  | [getPort()](#getPort--) | يحصل على رقم المنفذ. |
|
### EmailImapConnection(String host, int port, String userName, String password) {#EmailImapConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailImapConnection(String host, int port, String userName, String password)
```


يقوم بإنشاء نسخة جديدة من الفئة [EmailImapConnection](../../com.groupdocs.parser.options/emailimapconnection).


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

