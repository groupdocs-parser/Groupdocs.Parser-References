---
title: "DocumentInfo"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Belge bilgisini temsil eder."
type: docs
weight: 11
url: /tr/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Belge bilgisini temsil eder.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFileType()](#getFileType--) | Belge tipini alır. |
|
|  | [getPageCount()](#getPageCount--) | Belge sayfalarının toplam sayısını alır. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Belgenin ham sayfalarının toplam sayısını alır. |
|
|  | [getSize()](#getSize--) | Belgenin bayt cinsinden boyutunu alır. |
|
|  | [getPages()](#getPages--) | Sayfa indeksi ve sayfa boyutu gibi sayfalar hakkında bilgiyi alır. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Belge tipini alır.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Belge sayfalarının toplam sayısını alır.


**Returns:**
int - Toplam sayfa sayısını temsil eden bir tamsayı değeri.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Belgenin ham sayfalarının toplam sayısını alır.

Ham metin çıkarımı için [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) özelliğini, [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) özelliği yerine kullanın.
Bazı belgeler, doğru ve ham metin çıkarımı modlarında farklı sayfa numaralarına sahiptir.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - Ham sayfaların toplam sayısını temsil eden bir tamsayı değeri.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Belgenin bayt cinsinden boyutunu alır.


**Returns:**
long - Belge boyutunu bayt cinsinden temsil eden bir tam sayı değeri.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Sayfa indeksi ve sayfa boyutu gibi sayfalar hakkında bilgiyi alır.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - [PageInfo](../../com.groupdocs.parser.options/pageinfo) sınıflarının örneklerini içeren bir koleksiyon.

