---
title: "PageArea"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablonla ayrıştırma işlevinde belge sayfasındaki blokları temsil etmek için kullanılan sayfa alanları için soyut bir temel sınıfı temsil eder."
type: docs
weight: 17
url: /tr/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Şablonla ayrıştırma işlevinde belge sayfasındaki blokları temsil etmek için kullanılan sayfa alanları için soyut bir temel sınıfı temsil eder.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Dikdörtgen alanı alır. |
|
|  | [getPage()](#getPage--) | Sayfa indeksi ve sayfa boyutu gibi belge sayfası bilgilerini alır. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Dikdörtgen alanı alır.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Sayfa indeksi ve sayfa boyutu gibi belge sayfası bilgilerini alır.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

