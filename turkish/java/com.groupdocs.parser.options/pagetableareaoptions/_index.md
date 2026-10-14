---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Sayfa tablo alanı çıkarımı için kullanılan seçenekleri sağlar."
type: docs
weight: 31
url: /tr/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Sayfa tablo alanı çıkarımı için kullanılan seçenekleri sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Yeni bir [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) sınıfı örneği oluşturur. |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Arama dikdörtgeni ve sabit düzen olmadan yeni bir [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) sınıfı örneği oluşturur. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Sayfadaki tabloyu tanımlayan tablo düzenini alır. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Yeni bir [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) sınıfı örneği oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Sayfadaki tabloyu tanımlayan tablo düzeni. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Arama dikdörtgeni ve sabit düzen olmadan yeni bir [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) sınıfı örneği oluşturur.

Sayfadaki bir bölgeye otomatik algılanan tabloları sınırlamak için kullanışlıdır. C#'a yansır.

new PageTableAreaOptions(null) { Rectangle = ... }
desen.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Tabloların algılanması gereken sayfadaki dikdörtgen alan; tüm sayfayı aramak için  null  geçirin. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Sayfadaki tabloyu tanımlayan tablo düzenini alır.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

