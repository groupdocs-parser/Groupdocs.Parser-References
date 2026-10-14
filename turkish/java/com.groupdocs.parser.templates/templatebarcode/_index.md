---
title: "TemplateBarcode"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablon barkod alanını sağlar."
type: docs
weight: 11
url: /tr/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Şablon barkod alanını sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Yeni bir [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) sınıfı örneği başlatır. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Yeni bir [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) clas'ı BÜYÜK HARF adıyla başlatır. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | UPPER CASE adını kullanarak [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Yeni bir [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) sınıfı örneği başlatır. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Yeni bir [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Şablon barkod alanını içeren dikdörtgen alanı alır. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Yeni bir [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Şablon barkod alanını içeren dikdörtgen alan. |
|
|  | ad | java.lang.String | Barkod alanının adı. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Yeni bir [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) clas'ı BÜYÜK HARF adıyla başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Şablon barkod alanını içeren dikdörtgen alan. |
|
|  | ad | java.lang.String | Barkod alanının adı. |
|
|  | pageIndex | java.lang.Integer | Şablon öğesinin bulunduğu sayfanın dizinini temsil eden bir tamsayı değeri;  null  şablon öğesi herhangi bir sayfada bulunuyorsa. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


UPPER CASE adını kullanarak [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Şablon barkod alanını içeren dikdörtgen alan. |
|
|  | ad | java.lang.String | Barkod alanının adı. |
|
|  | pageIndex | java.lang.Integer | Şablon öğesinin bulunduğu sayfanın dizinini temsil eden bir tamsayı değeri;  null  şablon öğesi herhangi bir sayfada bulunuyorsa. |
|
|  | pageWidth | java.lang.Double | Şablon öğesini oluşturmak için kullanılan sayfanın genişliği. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Yeni bir [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Şablon barkod alanını içeren dikdörtgen alan. |
|
|  | ad | java.lang.String | Barkod alanının adı. |
|
|  | pageIndex | java.lang.Integer | Şablon öğesinin bulunduğu sayfanın dizinini temsil eden bir tamsayı değeri;  null  şablon öğesi herhangi bir sayfada bulunuyorsa. |
|
|  | useUpperCaseName | boolean | Bir  name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösteren değer. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Yeni bir [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Şablon barkod alanını içeren dikdörtgen alan. |
|
|  | ad | java.lang.String | Barkod alanının adı. |
|
|  | pageIndex | java.lang.Integer | Şablon öğesinin bulunduğu sayfanın dizinini temsil eden bir tamsayı değeri;  null  şablon öğesi herhangi bir sayfada bulunuyorsa. |
|
|  | pageWidth | java.lang.Double | Şablon öğesini oluşturmak için kullanılan sayfanın genişliği. |
|
|  | useUpperCaseName | boolean | Bir  name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösteren değer. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Şablon barkod alanını içeren dikdörtgen alanı alır.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Mevcut öğenin bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirerek oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| faktör | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
