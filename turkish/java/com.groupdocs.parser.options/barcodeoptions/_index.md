---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Barkod çıkarımı için kullanılan seçenekleri sağlar."
type: docs
weight: 10
url: /tr/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Barkod çıkarımı için kullanılan seçenekleri sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | BarcodeOptions sınıfının yeni bir örneğini varsayılan değerlerle başlatır. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | BarcodeOptions sınıfının yeni bir örneğini dikdörtgen alan ile başlatır. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | BarcodeOptions sınıfının yeni bir örneğini kalite ayarları ve kod türleri ile başlatır. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | BarcodeOptions sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Yanlış barkodların izin verilip verilmediğini gösteren değeri alır. |
|
|  | [getDimension()](#getDimension--) | Barkodun minimal öğesinin en küçük boyutunu alır. |
|
|  | [getImageQuality()](#getImageQuality--) | Kaynak görüntünün kalitesini alır. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Kaynak barkodun kalitesini alır. |
|
|  | [getRectangle()](#getRectangle--) | Sayfa alanlarını içeren dikdörtgen alanı alır. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Okunacak barkod türlerini alır. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Yanlış barkodların izin verilip verilmediğini gösteren değeri ayarlar. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Barkod minimal öğesinin minimal boyutunu ayarlar. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Kaynak görüntünün kalitesini ayarlar. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Kaynak barkodun kalitesini ayarlar. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Barkodları içeren dikdörtgen alanı ayarlar. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Okunacak barkod türlerini ayarlar. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


BarcodeOptions sınıfının yeni bir örneğini varsayılan değerlerle başlatır.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


BarcodeOptions sınıfının yeni bir örneğini dikdörtgen alan ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Barkodları içeren dikdörtgen alan. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


BarcodeOptions sınıfının yeni bir örneğini kalite ayarları ve kod türleri ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kaynak görüntünün kalitesi. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kaynak barkodun kalitesi. |
|
|  | codeTypes | java.lang.String[] | Okunacak barkod türleri. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


BarcodeOptions sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Barkodları içeren dikdörtgen alan. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kaynak görüntünün kalitesi. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kaynak barkodun kalitesi. |
|
|  | dimension | java.lang.Float | Barkod minimal öğesinin minimal boyutu. |
|
|  | allowIncorrectBarcodes | boolean | Yanlış barkodların izin verilip verilmediğini gösteren değer. |
|
|  | codeTypes | java.lang.String[] | Okunacak barkod türleri. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Yanlış barkodların izin verilip verilmediğini gösteren değeri alır.


**Returns:**
boolean -  true  eğer yanlış barkodlara izin veriliyorsa; aksi takdirde,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Barkodun minimal öğesinin en küçük boyutunu alır.


**Returns:**
java.lang.Float - Barkod minimal öğesini temsil eden float değeri;  null  otomatik mod kullanılırsa.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Kaynak görüntünün kalitesini alır.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Kaynak barkodun kalitesini alır.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Sayfa alanlarını içeren dikdörtgen alanı alır.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Okunacak barkod türlerini alır.


**Returns:**
java.util.List<java.lang.String> - Okunacak barkod türlerini içeren salt okunur koleksiyon; ayarlanmamışsa boş koleksiyon.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Yanlış barkodların izin verilip verilmediğini gösteren değeri ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  eğer yanlış barkodlara izin veriliyorsa. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Barkod minimal öğesinin minimal boyutunu ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dimension | java.lang.Float | Barkod minimal öğesi;  null  otomatik mod için. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Kaynak görüntünün kalitesini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Görüntü kalite modu. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Kaynak barkodun kalitesini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Barkod kalite modu. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Barkodları içeren dikdörtgen alanı ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Dikdörtgen alan;  null  tüm sayfayı taramak için. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Okunacak barkod türlerini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | Barkod türleri; tüm türler için null veya boş. |
|

