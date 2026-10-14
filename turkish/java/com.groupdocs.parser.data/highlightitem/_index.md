---
title: "HighlightItem"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Metnin bir bölümünü vurgulamayı temsil eder; bu genellikle arama işlevinde bulunan metnin bağlamını açıklamak için kullanılır."
type: docs
weight: 14
url: /tr/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Vurgulamayı temsil eder; bu, arama işlevinde bulunan metnin bağlamını açıklamak için genellikle kullanılan metnin bir parçasıdır.

Bir [HighlightItem](../../com.groupdocs.parser.data/highlightitem) sınıfı örneği, [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) metodunun dönüş değeri olarak kullanılır,
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Yeni bir [HighlightItem](../../com.groupdocs.parser.data/highlightitem) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getPosition()](#getPosition--) | Belge metnindeki konumu alır. |
|
|  | [getText()](#getText--) | Vurgulamanın metnini alır. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Yeni bir [HighlightItem](../../com.groupdocs.parser.data/highlightitem) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | konum | int | Belge metnindeki konum. |
|
|  | metin | java.lang.String | Vurgulamanın metni. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Belge metnindeki konumu alır.


**Returns:**
int - Vurgulamanın başlangıç konumunun sıfır tabanlı indeksi.

### getText() {#getText--}
```
public String getText()
```


Vurgulamanın metnini alır.


**Returns:**
java.lang.String - Vurgulamanın metnini temsil eden bir dize değeri.

