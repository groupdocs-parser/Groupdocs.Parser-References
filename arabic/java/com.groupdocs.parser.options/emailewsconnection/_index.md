---
title: "EmailEwsConnection"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل معلومات اتصال البريد الإلكتروني لبروتوكول EWS."
type: docs
weight: 13
url: /ar/java/com.groupdocs.parser.options/emailewsconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailEwsConnection extends EmailConnection
```

يمثل معلومات اتصال البريد الإلكتروني لبروتوكول EWS.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [EmailEwsConnection(String mailboxUri, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
|  | [EmailEwsConnection(String mailboxUri, String domain, String userName, String password)](#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getMailboxUri()](#getMailboxUri--) | يحصل على URI لصندوق البريد. |
|
|  | [getDomain()](#getDomain--) | يحصل على اسم النطاق. |
|
### EmailEwsConnection(String mailboxUri, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String userName, String password)
```


ينشئ مثيلاً جديداً من الفئة [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | URI صندوق البريد. |
|
|  | userName | java.lang.String | اسم المستخدم. |
|
|  | كلمة المرور | java.lang.String | كلمة المرور. |
|

### EmailEwsConnection(String mailboxUri, String domain, String userName, String password) {#EmailEwsConnection-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public EmailEwsConnection(String mailboxUri, String domain, String userName, String password)
```


ينشئ مثيلاً جديداً من الفئة [EmailEwsConnection](../../com.groupdocs.parser.options/emailewsconnection).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | mailboxUri | java.lang.String | URI صندوق البريد. |
|
|  | domain | java.lang.String | اسم النطاق. |
|
|  | userName | java.lang.String | اسم المستخدم. |
|
|  | كلمة المرور | java.lang.String | كلمة المرور. |
|

### getMailboxUri() {#getMailboxUri--}
```
public String getMailboxUri()
```


يحصل على URI لصندوق البريد.


**Returns:**
java.lang.String - قيمة نصية تمثل URI لصندوق البريد.

### getDomain() {#getDomain--}
```
public String getDomain()
```


يحصل على اسم النطاق.


**Returns:**
java.lang.String - قيمة نصية تمثل اسم النطاق.

