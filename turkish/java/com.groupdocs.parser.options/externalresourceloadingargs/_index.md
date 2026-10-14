---
title: "ExternalResourceLoadingArgs"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Metod için verileri sağlar."
type: docs
weight: 17
url: /tr/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Metod için verileri sağlar [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) metoduna.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Dikdörtgen alan ile [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getUri()](#getUri--) | Harici kaynağın URI'sını alır. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Harici kaynağın URI'sını alır. |
|
|  | [isSkipped()](#isSkipped--) | Harici kaynağın yüklemesinin atlanması gerekip gerekmediğini gösteren değeri alır. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Harici kaynağın yüklemesinin atlanması gerekip gerekmediğini gösteren değeri ayarlar. |
|
|  | [getData()](#getData--) | Kullanıcı verisini alır. |
|
|  | [setData(byte[] data)](#setData-byte---) | Kullanıcı verisini ayarlar. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Dikdörtgen alan ile [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | uri | java.lang.String | Harici kaynağın URI'sı. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Harici kaynağın URI'sını alır.


**Returns:**
java.lang.String - Harici kaynağın URI'sını temsil eden bir dize değeri.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Harici kaynağın URI'sını alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | uri | java.lang.String | Harici kaynağın yeni bir URI'sını temsil eden bir dize değeri. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Harici kaynağın yüklemesinin atlanması gerekip gerekmediğini gösteren değeri alır.


**Returns:**
boolean - harici kaynağın yüklemesi atlanmalıysa true; aksi takdirde false.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Harici kaynağın yüklemesinin atlanması gerekip gerekmediğini gösteren değeri ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | atlandı | boolean | harici kaynağın yüklenmesinin atlanması gerekiyorsa true; aksi takdirde false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Kullanıcı verisini alır.


**Returns:**
byte[] - Harici kaynağın kullanıcı içeriğini içeren bayt dizisi. Ayarlanmamışsa null.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Kullanıcı verisini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | veri | byte[] | Harici kaynağın kullanıcı içeriğini içeren bayt dizisi. Ayarlanmamışsa null. |
|

