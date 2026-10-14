---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "OCR olayları için bir işleyici sağlar."
type: docs
weight: 26
url: /tr/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

OCR olayları için bir işleyici sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Yeni bir [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) sınıfının bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Uyarı mesajlarının bir listesini alır. |
|
|  | [hasWarnings()](#hasWarnings--) | Uyarı listesinin boş olup olmadığını gösteren değeri alır. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Sayfa indeksi  pageIndex  olan sayfa için uyarı mesajlarının bir listesini döndürür. |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Sayfa için uyarı mesajlarını ayarlar. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Yeni bir [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) sınıfının bir örneğini başlatır.


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Uyarı mesajlarının bir listesini alır.


**Returns:**
java.util.List<java.lang.String> - Tüm sayfalar için uyarı mesajlarının bir listesi.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Uyarı listesinin boş olup olmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer uyarı listesi boş değilse; aksi takdirde,  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Sayfa indeksi  pageIndex  olan sayfa için uyarı mesajlarının bir listesini döndürür.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

**Returns:**
java.util.List<java.lang.String> - Sayfa için uyarı mesajlarının bir listesi; sayfada uyarı mesajı yoksa boş liste.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Sayfa için uyarı mesajlarını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | Sayfa için uyarı mesajlarının listesi. |
|

