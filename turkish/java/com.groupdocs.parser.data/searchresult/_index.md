---
title: "SearchResult"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Arama işlevinde arama sonucunu temsil eder."
type: docs
weight: 27
url: /tr/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Arama işlevinde arama sonucunu temsil eder.

Bir SearchResult sınıfı örneği, [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-) metodunun dönüş değeri olarak kullanılır
ve [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-) metodları. Oradaki kullanım örneklerine bakın.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Yeni bir [SearchResult](../../com.groupdocs.parser.data/searchresult) sınıfı örneği başlatır. |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Yeni bir [SearchResult](../../com.groupdocs.parser.data/searchresult) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getPosition()](#getPosition--) | Belge metnindeki konumu alır. |
|
|  | [getText()](#getText--) | Metni alır. |
|
|  | [getPageIndex()](#getPageIndex--) | Metnin bulunduğu sayfa indeksini alır. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Sol vurgulamayı alır. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Sağ vurgulamayı alır. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Yeni bir [SearchResult](../../com.groupdocs.parser.data/searchresult) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | konum | int | Belge metnindeki konum. |
|
|  | metin | java.lang.String | Bulunan metin. |
|
|  | pageIndex | java.lang.Integer | Metnin bulunduğu sayfa indeksi. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Sol vurgulama. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Sağ vurgulama. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Yeni bir [SearchResult](../../com.groupdocs.parser.data/searchresult) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | konum | int | Belge metnindeki konum. |
|
|  | metin | java.lang.String | Bulunan metin. |
|
|  | pageIndex | java.lang.Integer | Metnin bulunduğu sayfa indeksi. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Belge metnindeki konumu alır.


**Returns:**
int - Arama sonucunun başlangıç konumunun sıfır tabanlı indeksi.

### getText() {#getText--}
```
public String getText()
```


Metni alır.


**Returns:**
java.lang.String - Bulunan metni temsil eden bir dize değeri.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Metnin bulunduğu sayfa indeksini alır.


**Returns:**
java.lang.Integer - Metnin bulunduğu sayfanın sıfır tabanlı indeksi;  null  eğer arama tüm belge metni üzerinde yapılmışsa.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Sol vurgulamayı alır.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Sağ vurgulamayı alır.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

