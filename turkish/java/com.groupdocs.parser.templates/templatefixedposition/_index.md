---
title: "TemplateFixedPosition"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Dikdörtgen alanla tanımlanan bir şablon alan konumunu sağlar."
type: docs
weight: 13
url: /tr/java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Dikdörtgen alanla tanımlanan bir şablon alan konumunu sağlar.

Bu, alan konumunu tanımlamanın en basit yoludur. Sayfada alanı sınırlayan dikdörtgen bir bölge ayarlamayı gerektirir
alan değerini. Dikdörtgen alana (kısmen dahi) dahil olan tüm metin bir değer olarak çıkarılacaktır:

````
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Yeni bir [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Şablon alanını içeren dikdörtgen alanı alır. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Yeni bir [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Şablon alanını içeren dikdörtgen alan. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Şablon alanını içeren dikdörtgen alanı alır.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Mevcut konumun bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirilmiş şekilde oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| faktör | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
