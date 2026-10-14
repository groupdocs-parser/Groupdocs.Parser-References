---
title: "PageBarcodeArea"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablonla ayrıştırma işlevinde bir barkod değerini temsil etmek için kullanılan sayfa barkod alanını temsil eder."
type: docs
weight: 18
url: /tr/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Şablonla ayrıştırma işlevinde bir barkod değerini temsil etmek için kullanılan sayfa barkod alanını temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Yeni bir [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) sınıfının bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getValue()](#getValue--) | Barkod değerini alır. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Barkod tipinin adını alır. |
|
|  | [getConfidence()](#getConfidence--) | Ayrıştırılan barkodun güven seviyesini alır. |
|
|  | [getAngle()](#getAngle--) | Barkodun açısını alır. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Yeni bir [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) sınıfının bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Barkodun değeri. |
|
|  | codeTypeName | java.lang.String | Barkodun tip adı. |
|
|  | confidence | int | Ayrıştırılmış barkodun güven seviyesi. |
|
|  | angle | double | Barkodun açısı. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Barkod alanını içeren sayfa. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Barkod alanını içeren dikdörtgen alan. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Barkod değerini alır.


**Returns:**
java.lang.String - Barkod sayfa alanının değerini temsil eden bir dize değeri.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Barkod tipinin adını alır.


**Returns:**
java.lang.String - Barkodun tip adını temsil eden bir dize değeri.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Ayrıştırılan barkodun güven seviyesini alır.


**Returns:**
int - Ayrıştırılan barkodun güvenini temsil eden bir tamsayı değeri (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


Barkodun açısını alır.


**Returns:**
double - Barkodun açısını temsil eden bir tamsayı değeri (0-360).

