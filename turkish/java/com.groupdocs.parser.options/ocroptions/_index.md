---
title: "OcrOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "OCR Bağlayıcısı için kullanılan seçenekleri sağlar."
type: docs
weight: 27
url: /tr/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

OCR Bağlayıcısı için kullanılan seçenekleri sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Varsayılan değerlerle [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Dikdörtgen alanla [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Sayfa önizleme seçenekleriyle [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) nesnesiyle [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Dikdörtgen alan ve [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) nesnesiyle [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Metin tanıma için kullanılan sayfa alanını sınırlayan dikdörtgen alanı alır. |
|
|  | [getHandler()](#getHandler--) | OCR olaylarını yakalamak için olay işleyicisini alır. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Yazım denetiminin kullanılıp kullanılmadığını gösteren değeri alır. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | OCR motoruna beslenen sayfayı oluşturmak için kullanılan sayfa önizleme seçeneklerini alır. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | OCR motoruna beslenen sayfayı oluşturmak için kullanılan sayfa önizleme seçeneklerini ayarlar. |
|
|  | [getLanguage()](#getLanguage--) | Optik karakter tanıması için kullanılan dili alır. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Optik karakter tanıması için kullanılan dili ayarlar. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Metin tanıma için kullanılan sayfa alanını sınırlayan dikdörtgen alanı ayarlar. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | OCR olaylarını yakalamak için olay işleyicisini ayarlar. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Yazım denetiminin kullanılıp kullanılmadığını gösteren değeri ayarlar. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Varsayılan değerlerle [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Dikdörtgen alanla [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Metin tanıma için kullanılan sayfa alanını sınırlayan dikdörtgen alan. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Sayfa önizleme seçenekleriyle [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | OCR motoruna beslenen sayfa önizlemesini oluşturmak için kullanılan seçenekler. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) nesnesiyle [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR olaylarını yakalamak için bir [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) örneği. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Dikdörtgen alan ve [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) nesnesiyle [OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Metin tanıma için kullanılan sayfa alanını sınırlayan dikdörtgen alan. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR olaylarını yakalamak için bir [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) örneği. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


[OcrOptions](../../com.groupdocs.parser.options/ocroptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Metin tanıma için kullanılan sayfa alanını sınırlayan dikdörtgen alan. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | OCR olaylarını yakalamak için bir [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) örneği. |
|
|  | useSpellCheker | boolean | Yazım denetiminin kullanılıp kullanılmadığını gösteren değer. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Metin tanıma için kullanılan sayfa alanını sınırlayan dikdörtgen alanı alır.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


OCR olaylarını yakalamak için olay işleyicisini alır.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Yazım denetiminin kullanılıp kullanılmadığını gösteren değeri alır.


**Returns:**
boolean -  true  ise yazım denetimi kullanılır; aksi takdirde false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


OCR motoruna beslenen sayfayı oluşturmak için kullanılan sayfa önizleme seçeneklerini alır.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


OCR motoruna beslenen sayfayı oluşturmak için kullanılan sayfa önizleme seçeneklerini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Sayfa önizleme seçenekleri. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Optik karakter tanıması için kullanılan dili alır.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Optik karakter tanıması için kullanılan dili ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | [Language](../../com.groupdocs.parser.options/language) enum değeri. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Metin tanıma için kullanılan sayfa alanını sınırlayan dikdörtgen alanı ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Dikdörtgen, ya da tüm sayfayı taramak için  null  . |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


OCR olaylarını yakalamak için olay işleyicisini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Olay işleyicisi. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Yazım denetiminin kullanılıp kullanılmadığını gösteren değeri ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  ile imla denetimini etkinleştir. |
|

