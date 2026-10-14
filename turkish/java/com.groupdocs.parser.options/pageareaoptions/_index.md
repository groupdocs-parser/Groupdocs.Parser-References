---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Sayfa alanı çıkarımı için kullanılan seçenekleri sağlar."
type: docs
weight: 28
url: /tr/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Sayfa alanı çıkarımı için kullanılan seçenekleri sağlar.

Bir [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) sınıfı örneği, [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-) içinde parametre olarak kullanılır.
ve [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-) metodları. Orada kullanım örneklerine bakın.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Yoksayılan kenarın boyutu ile yeni bir [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) sınıf örneği başlatır. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Yeni bir [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) sınıfının örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Sayfa alanlarını içeren dikdörtgen alanı alır. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Dikdörtgen alan tarafından yakalandığında göz ardı edilen kenarın boyutunu alır. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Yoksayılan kenarın boyutu ile yeni bir [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) sınıf örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Sayfa alanlarını içeren dikdörtgen alan. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Yeni bir [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Sayfa alanlarını içeren dikdörtgen alan. |
|
|  | rectangleTolerance | double | Dikdörtgen alan tarafından yakalandığında göz ardı edilen kenarın boyutu. Bu, bir metin öğesi yüksekliğinin kesriyle ölçülür. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Sayfa alanlarını içeren dikdörtgen alanı alır.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Dikdörtgen alan tarafından yakalandığında göz ardı edilen kenarın boyutunu alır. Bu, bir metin öğesi yüksekliğinin kesriyle ölçülür.


**Returns:**
double - 0 (kenar yok) ile 1 (tüm öğeyi yoksay) arasında bir double değeri.

