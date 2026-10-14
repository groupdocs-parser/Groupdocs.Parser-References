---
title: "PageTextArea"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablonla veya form ayrıştırma işleviyle metin değerini temsil etmek için kullanılan bir sayfa metin alanını temsil eder."
type: docs
weight: 24
url: /tr/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Şablonla veya form ayrıştırma işleviyle metin değerini temsil etmek için kullanılan bir sayfa metin alanını temsil eder.

Aşağıdaki yöntemlerin dönüş değeri olarak [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) sınıfının bir örneği kullanılır:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

Ayrıca [PageArea](../../com.groupdocs.parser.data/pagearea) özelliğinin değeri olarak [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) sınıfının bir örneği kullanılır.
\*

Oradaki kullanım örneklerine bakın.

Metin alanı tek veya birleşik olabilir. İlk durumda, dikdörtgen bir alanla sınırlı bir metin içerir.
İkinci durumda diğer metin alanlarını içerir; metin ve tablo özellikleri alt metin alanları tarafından hesaplanır.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) sınıfının yeni bir örneğini başlatır. |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) sınıfının yeni bir örneğini başlatır. |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getText()](#getText--) | Metni alır. |
|
|  | [getBaseLine()](#getBaseLine--) | Taban çizgisini alır. |
|
|  | [getTextStyle()](#getTextStyle--) | Yazı tipi boyutu, yazı tipi adı vb. gibi metin stilini alır. |
|
|  | [getAreas()](#getAreas--) | Alt metin sayfa alanlarının koleksiyonunu alır. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


[PageTextArea](../../com.groupdocs.parser.data/pagetextarea) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | metin | java.lang.String | Metnin değeri. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Metin alanını içeren sayfa. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Metin alanını içeren dikdörtgen alan. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


[PageTextArea](../../com.groupdocs.parser.data/pagetextarea) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | metin | java.lang.String | Metnin değeri. |
|
|  | baseLine | java.lang.Double | Metnin taban çizgisi. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | Metnin stili. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Metin alanını içeren sayfa. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Metin alanını içeren dikdörtgen alan. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


[PageTextArea](../../com.groupdocs.parser.data/pagetextarea) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | alanlar | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Alt metin sayfa alanlarının koleksiyonu. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Metin alanını içeren sayfa. |
|

### getText() {#getText--}
```
public String getText()
```


Metni alır.


**Returns:**
java.lang.String - Metin sayfa alanının değerini temsil eden bir dize değeri.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Taban çizgisini alır.


**Returns:**
double - Temel çizgiyi temsil eden bir double değeri.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Yazı tipi boyutu, yazı tipi adı vb. gibi metin stilini alır.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Alt metin sayfa alanlarının koleksiyonunu alır.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - Alt metin sayfa alanlarının bir koleksiyonu; metin sayfa alanının çocuğu yoksa boş.

