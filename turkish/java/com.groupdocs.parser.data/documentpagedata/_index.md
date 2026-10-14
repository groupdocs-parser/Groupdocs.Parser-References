---
title: "DocumentPageData"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Belge sayfasının verilerini temsil eder."
type: docs
weight: 12
url: /tr/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Belge sayfasının verilerini temsil eder. Belge sayfasından alan verilerini içeren [FieldData](../../com.groupdocs.parser.data/fielddata) nesnelerinden oluşur.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Yeni bir [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) sınıfının bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Sayfa indeksini alır. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Yeni bir [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) sınıfının bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | alanlar | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | Alan verilerinin koleksiyonu. |
|
|  | pageIndex | int | Sıfır tabanlı sayfa indeksi. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Sayfa indeksini alır.


**Returns:**
int - Sayfanın sıfır tabanlı indeksi.

