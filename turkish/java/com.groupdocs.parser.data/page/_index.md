---
title: "Page"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Sayfa indeksi ve sayfa boyutu gibi belge sayfası bilgilerini temsil eder."
type: docs
weight: 16
url: /tr/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Sayfa indeksi ve sayfa boyutu gibi belge sayfası bilgilerini temsil eder. Şablon işleviyle ayrıştırmada [PageArea](../../com.groupdocs.parser.data/pagearea) sınıfının türevlerini içeren sayfayı temsil etmek için kullanılır.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | [Page](../../com.groupdocs.parser.data/page) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getIndex()](#getIndex--) | Sayfa indeksini alır. |
|
|  | [getSize()](#getSize--) | Sayfa boyutunu alır. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


[Page](../../com.groupdocs.parser.data/page) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indeks | int | Sayfa indeksi. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Sayfa boyutu. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Sayfa indeksini alır.


**Returns:**
int - Sayfanın sıfır tabanlı indeksi.

### getSize() {#getSize--}
```
public Size getSize()
```


Sayfa boyutunu alır.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.

