---
title: "OcrConnectorBase"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "OCR işlevselliğini sağlar."
type: docs
weight: 25
url: /tr/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

OCR işlevselliğini sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Yeni bir [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) sınıfının bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Metin çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Metin alanı çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | imageStream akışından bir metni tanır. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | imageStream akışından metin alanlarını tanır. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Yeni bir [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) sınıfının bir örneğini başlatır.


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Metin çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin çıkarımı destekleniyorsa; aksi takdirde,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Metin alanı çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin çıkarım alanları destekleniyorsa; aksi takdirde,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


imageStream akışından bir metni tanır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Belge sayfasının görüntü temsili. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR seçenekleri. |
|

**Returns:**
java.lang.String - Tanınan bir metni temsil eden bir dize;  null  eğer metin tanıma desteklenmiyorsa.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


imageStream akışından metin alanlarını tanır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Belge sayfasının görüntü temsili. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | Belge sayfasının boyutu. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | OCR seçenekleri. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) nesnelerinin bir koleksiyonu;  null  eğer metin alanı tanıma desteklenmiyorsa.

