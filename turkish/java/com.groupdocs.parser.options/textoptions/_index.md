---
title: "TextOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Metin çıkarımı için kullanılan seçenekleri sağlar."
type: docs
weight: 37
url: /tr/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Metin çıkarımı için kullanılan seçenekleri sağlar.

Bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği, [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-) içinde parametre olarak kullanılır.
ve [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) yöntemleri. Oradaki kullanım örneklerine bakın.

Metin çıkarımının ham modunu belirtmek için kullanılır. Bu moddaki bir metin, tam doğru olmayan bir şekilde
yöntemi, ancak standart moddan daha hızlıdır. Ham mod belge formatını desteklemiyorsa,
bu parametre yok sayılır ve standart mod kullanılır.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | OCR kullanım seçeneği ile yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | OCR seçeneklerini ayarlama yeteneği ile yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Ham modun kullanılıp kullanılmadığını gösteren değeri alır. |
|
|  | [isUseOcr()](#isUseOcr--) | Bir metin çıkarmak için OCR Bağlayıcısının kullanılıp kullanılmadığını gösteren değeri alır. |
|
|  | [getOcrOptions()](#getOcrOptions--) | OCR işlevselliği için ek seçenekleri alır. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Çıkarılan metinde açıklamaların dahil edilip edilmediğini gösteren değeri alır. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Çıkarılan metinde açıklamaların dahil edilip edilmediğini gösteren değeri ayarlar. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Ham modun kullanılıp kullanılmadığını gösteren değer. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


OCR kullanım seçeneği ile yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Ham modun kullanılıp kullanılmadığını gösteren değer. |
|
|  | useOcr | boolean | OCR işlevinin bir metin çıkarmak için kullanılıp kullanılmadığını gösteren değer. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


OCR seçeneklerini ayarlama yeteneği ile yeni bir [TextOptions](../../com.groupdocs.parser.options/textoptions) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Ham modun kullanılıp kullanılmadığını gösteren değer. |
|
|  | useOcr | boolean | OCR işlevinin bir metin çıkarmak için kullanılıp kullanılmadığını gösteren değer. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR işlevi için ek seçenekler. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Ham modun kullanılıp kullanılmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer ham mod kullanılıyorsa; aksi takdirde,  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Alır değeri, çıkarılan metinde ek açıklamaların dahil edilip edilmediğini gösterir. Varsayılan değer  false .


**Returns:**
boolean -  true  eğer ek açıklamalar dahil edildiyse; aksi takdirde,  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Çıkarılan metinde açıklamaların dahil edilip edilmediğini gösteren değeri ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  çıkarılan metinde ek açıklamaları dahil etmek için. |
|

