---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Sayfa metin alanı çıkarımı için kullanılan seçenekleri sağlar."
type: docs
weight: 32
url: /tr/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Sayfa metin alanı çıkarımı için kullanılan seçenekleri sağlar.

Bir [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının örneği, [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-) içinde parametre olarak kullanılır.
ve [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) metodları. Oradaki kullanım örneklerine bakın.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Varsayılan değerlerle [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | OCR kullanım seçeneği ile yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | OCR seçeneklerini ayarlama yeteneği ile yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Düzenli ifadeyle [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Düzenli ifade ve dikdörtgen alan ile [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Düzenli ifade, dikdörtgen alan ve yoksayılan kenarın boyutu ile [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Yoksayılan kenarın boyutu ile [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getExpression()](#getExpression--) | Düzenli ifadeyi alır. |
|
|  | [isMatchCase()](#isMatchCase--) | Metin durumunun yoksayılmadığını gösteren değeri alır. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Segmentlerin birleştirildiğini gösteren değeri alır. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Metin biçimlendirmesinin yoksayıldığını gösteren değeri alır. |
|
|  | [isUseOcr()](#isUseOcr--) | Bir metin çıkarmak için OCR Bağlayıcısının kullanılıp kullanılmadığını gösteren değeri alır. |
|
|  | [getOcrOptions()](#getOcrOptions--) | OCR işlevselliği için ek seçenekleri alır. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Varsayılan değerlerle [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


OCR kullanım seçeneği ile yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | useOcr | boolean | OCR işlevinin bir metin çıkarmak için kullanılıp kullanılmadığını gösteren değer. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


OCR seçeneklerini ayarlama yeteneği ile yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | useOcr | boolean | OCR işlevinin bir metin çıkarmak için kullanılıp kullanılmadığını gösteren değer. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR işlevi için ek seçenekler. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Düzenli ifadeyle [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır. Diğer seçenekler varsayılan olarak ayarlanır (detaylar için açıklamalara bakın).

Aşağıdaki özelliklerin varsayılan değerleri vardır:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ifade | java.lang.String | Düzenli ifade. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Düzenli ifade ve dikdörtgen alan ile [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır. Diğer seçenekler varsayılan olarak ayarlanır (ayrıntılar için açıklamalara bakın).

Aşağıdaki özelliklerin varsayılan değerleri vardır:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ifade | java.lang.String | Düzenli ifade. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Sayfa alanlarını içeren dikdörtgen alan. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Düzenli ifade, dikdörtgen alan ve yoksayılan kenarın boyutu ile [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır. Diğer seçenekler varsayılan olarak ayarlanır (ayrıntılar için açıklamalara bakın).


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ifade | java.lang.String | Düzenli ifade. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Sayfa alanlarını içeren dikdörtgen alan. |
|
|  | rectangleTolerance | double | Dikdörtgen alan tarafından yakalandığında göz ardı edilen kenarın boyutu. Bu, bir metin öğesi yüksekliğinin kesriyle ölçülür. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


[PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ifade | java.lang.String | Düzenli ifade. |
|
|  | matchCase | boolean | Metin büyük/küçük harfinin yoksayılmadığını gösteren değer. |
|
|  | uniteSegments | boolean | Segmentlerin birleştirilip birleştirilmediğini gösteren değer. |
|
|  | ignoreFormatting | boolean | Metin biçimlendirmesinin yoksayılıp yoksayılmadığını gösteren değer. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Sayfa alanlarını içeren dikdörtgen alan. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Yoksayılan kenarın boyutu ile [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ifade | java.lang.String | Düzenli ifade. |
|
|  | matchCase | boolean | Metin büyük/küçük harfinin yoksayılmadığını gösteren değer. |
|
|  | uniteSegments | boolean | Segmentlerin birleştirilip birleştirilmediğini gösteren değer. |
|
|  | ignoreFormatting | boolean | Metin biçimlendirmesinin yoksayılıp yoksayılmadığını gösteren değer. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Sayfa alanlarını içeren dikdörtgen alan. |
|
|  | rectangleTolerance | double | Dikdörtgen alan tarafından yakalandığında göz ardı edilen kenarın boyutu. Bu, bir metin öğesi yüksekliğinin kesriyle ölçülür. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Düzenli ifadeyi alır.


**Returns:**
java.lang.String - Düzenli ifadeyi temsil eden bir dize.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Metin durumunun yoksayılmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin büyük/küçük harfi yoksayılmıyorsa; aksi takdirde,  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Segmentlerin birleştirildiğini gösteren değeri alır.


**Returns:**
boolean - {code true} eğer segmentler birleştirilmişse; aksi takdirde, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Metin biçimlendirmesinin yoksayıldığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin biçimlendirmesi yoksayılmışsa; aksi takdirde,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Bir metin çıkarmak için OCR Bağlayıcısının kullanılıp kullanılmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer OCR işlevi kullanılıyorsa; aksi takdirde,  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


OCR işlevselliği için ek seçenekleri alır.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

