---
title: "EmailPopConnection"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "POP protokolü için e-posta bağlantı bilgisini temsil eder."
type: docs
weight: 15
url: /tr/java/com.groupdocs.parser.options/emailpopconnection/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.EmailConnection](../../com.groupdocs.parser.options/emailconnection)
```
public final class EmailPopConnection extends EmailConnection
```

POP protokolü için e-posta bağlantı bilgisini temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [EmailPopConnection(String host, int port, String userName, String password)](#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-) | Yeni bir [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection) sınıfının örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getHost()](#getHost--) | Ana bilgisayar adını alır. |
|
|  | [getPort()](#getPort--) | Bağlantı noktasının numarasını alır. |
|
### EmailPopConnection(String host, int port, String userName, String password) {#EmailPopConnection-java.lang.String-int-java.lang.String-java.lang.String-}
```
public EmailPopConnection(String host, int port, String userName, String password)
```


Yeni bir [EmailPopConnection](../../com.groupdocs.parser.options/emailpopconnection) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ana bilgisayar | java.lang.String | Ana bilgisayar adı. |
|
|  | bağlantı noktası | int | Bağlantı noktası numarası. |
|
|  | kullanıcıAdı | java.lang.String | Kullanıcı adı. |
|
|  | parola | java.lang.String | Parola. |
|

### getHost() {#getHost--}
```
public String getHost()
```


Ana bilgisayar adını alır.


**Returns:**
java.lang.String - Ana bilgisayar adını temsil eden bir dize değeri.

### getPort() {#getPort--}
```
public int getPort()
```


Bağlantı noktasının numarasını alır.


**Returns:**
int - Bağlantı noktasını temsil eden bir tam sayı değeri.

