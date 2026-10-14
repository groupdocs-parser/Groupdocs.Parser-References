---
title: "PageGroupArea"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablonla ayrıştırma işlevinde belge sayfasının farklı blok türlerini gruplamak için kullanılan bir sayfa alanı grubunu temsil eder."
type: docs
weight: 19
url: /tr/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Şablonla ayrıştırma işlevinde belge sayfasının farklı blok türlerini gruplamak için kullanılan bir sayfa alanı grubunu temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Yeni bir [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) sınıfının bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getAreas()](#getAreas--) | Gruplanmış sayfa alanlarının koleksiyonunu alır. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Yeni bir [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) sınıfının bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | alanlar | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | Gruplanacak sayfa alanlarının koleksiyonu. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Alanı içeren sayfa. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Gruplanmış sayfa alanlarının koleksiyonunu alır.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - [PageArea](../../com.groupdocs.parser.data/pagearea) nesnelerinin bir koleksiyonu.

