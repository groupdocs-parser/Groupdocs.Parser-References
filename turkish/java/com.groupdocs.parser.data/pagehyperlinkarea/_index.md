---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Sayfada bir köprü bağlantısını temsil etmek için kullanılan bir sayfa alanını temsil eder."
type: docs
weight: 20
url: /tr/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Sayfada bir köprü bağlantısını temsil etmek için kullanılan bir sayfa alanını temsil eder.

Aşağıdaki yöntemlerin dönüş değeri olarak [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) sınıfının bir örneği kullanılır:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Oradaki kullanım örneklerine bakın.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Yeni bir [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) sınıfı örneği oluşturur. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getText()](#getText--) | Köprü metnini alır. |
|
|  | [getUrl()](#getUrl--) | Köprü URL'sini alır. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Yeni bir [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) sınıfı örneği oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | metin | java.lang.String | Köprü metni. |
|
|  | url | java.lang.String | Köprü URL'si. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Köprüyü içeren sayfa. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Köprüyü içeren dikdörtgen alan. |
|

### getText() {#getText--}
```
public String getText()
```


Köprü metnini alır.


**Returns:**
java.lang.String - Köprü metnini temsil eden bir dize değeri.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Köprü URL'sini alır.


**Returns:**
java.lang.String - Köprü URL'sini temsil eden bir dize değeri.

