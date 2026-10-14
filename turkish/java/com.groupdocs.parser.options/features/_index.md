---
title: "Özellikler"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Desteklenen özellikler listesini temsil eder."
type: docs
weight: 18
url: /tr/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Desteklenen özellikler listesini temsil eder. Belge için hangi özelliklerin desteklendiği veya desteklenmediği hakkında bilgi edinmeyi sağlar.

Bu sınıfın bir örneği, [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--) özelliği olarak kullanılır. Oradaki kullanım örneklerine bakın.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Features()](#Features--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Özelliğin desteklenip desteklenmediğini gösteren değeri döndürür. |
|
|  | [isText()](#isText--) | Metin çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isTextPage()](#isTextPage--) | Metin sayfa çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isFormattedText()](#isFormattedText--) | Biçimlendirilmiş metin çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Biçimlendirilmiş metin sayfa çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isSearch()](#isSearch--) | Metin aramasının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isHighlight()](#isHighlight--) | Vurgulama çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isBarcodes()](#isBarcodes--) | Barkod çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isToc()](#isToc--) | İçindekiler tablosu çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isMetadata()](#isMetadata--) | Meta veri çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isContainer()](#isContainer--) | Kapsayıcı çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isTextAreas()](#isTextAreas--) | Metin alanları çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isStructure()](#isStructure--) | Metin yapısı çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isImages()](#isImages--) | Görüntü çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Köprü çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isTables()](#isTables--) | Tablo çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isAnnotations()](#isAnnotations--) | Açıklama çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Şablona göre ayrıştırmanın desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isParseForm()](#isParseForm--) | Form ayrıştırmasının desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isPreview()](#isPreview--) | Önizleme oluşturmanın desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isPagePreview()](#isPagePreview--) | Sayfa önizleme oluşturmanın desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isOcr()](#isOcr--) | OCR işlevselliğinin desteklenip desteklenmediğini gösteren değeri alır. |
|
|  | [isWorksheet()](#isWorksheet--) | Çalışma sayfası çıkarımının desteklenip desteklenmediğini gösteren değeri alır. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Özelliğin desteklenip desteklenmediğini gösteren değeri döndürür.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | featureName | java.lang.String | Özellik adı. |
|

**Returns:**
boolean -  true  eğer özellik destekleniyorsa; aksi takdirde,  false .

### isText() {#isText--}
```
public boolean isText()
```


Metin çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin çıkarımı destekleniyorsa; aksi takdirde,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Metin sayfa çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin sayfa çıkarımı destekleniyorsa; aksi takdirde,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Biçimlendirilmiş metin çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer biçimlendirilmiş metin çıkarımı destekleniyorsa; aksi takdirde,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Biçimlendirilmiş metin sayfa çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer biçimlendirilmiş metin sayfası destekleniyorsa; aksi takdirde,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Metin aramasının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin araması destekleniyorsa; aksi takdirde,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Vurgulama çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer vurgulama çıkarımı destekleniyorsa; aksi takdirde,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Barkod çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer barkod çıkarımı destekleniyorsa; aksi takdirde,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


İçindekiler tablosu çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer içindekiler tablosu çıkarımı destekleniyorsa; aksi takdirde,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Meta veri çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer üst veri çıkarımı destekleniyorsa; aksi takdirde,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Kapsayıcı çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer konteyner çıkarımı destekleniyorsa; aksi takdirde,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Metin alanları çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin alanları çıkarımı destekleniyorsa; aksi takdirde,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Metin yapısı çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin yapısı çıkarımı destekleniyorsa; aksi takdirde,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Görüntü çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer görüntü çıkarımı destekleniyorsa; aksi takdirde,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Köprü çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer hiperlink çıkarımı destekleniyorsa; aksi takdirde,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Tablo çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer tablo çıkarımı destekleniyorsa; aksi takdirde,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Açıklama çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer açıklama çıkarımı destekleniyorsa; aksi takdırde,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Şablona göre ayrıştırmanın desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer şablona göre ayrıştırma destekleniyorsa; aksi takdirde,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Form ayrıştırmasının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer form ayrıştırması destekleniyorsa; aksi takdirde,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Önizleme oluşturmanın desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer önizleme oluşturma destekleniyorsa; aksi takdirde,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Sayfa önizleme oluşturmanın desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer sayfa önizleme oluşturma destekleniyorsa; aksi takdirde,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


OCR işlevselliğinin desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer OCR işlevselliği destekleniyorsa; aksi takdirde,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Çalışma sayfası çıkarımının desteklenip desteklenmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer çalışma sayfası çıkarımı destekleniyorsa; aksi takdirde,  false .

