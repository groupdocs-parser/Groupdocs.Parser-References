---
title: "TemplateItem"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablon öğeleri için temel soyut sınıfı sağlar."
type: docs
weight: 14
url: /tr/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Şablon öğeleri için temel soyut sınıfı sağlar.

[TemplateItem](../../com.groupdocs.parser.templates/templateitem) sınıfının türevleri, [Template](../../com.groupdocs.parser.templates/template) koleksiyonunda kullanılır.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Mevcut öğenin bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirerek oluşturur. |
|
|  | [getName()](#getName--) | Şablon öğesinin adını alır. |
|
|  | [getPageIndex()](#getPageIndex--) | Şablon öğesinin sayfa indeksini alır. |
|
|  | [getPageWidth()](#getPageWidth--) | Şablon öğesini oluşturmak için kullanılan sayfanın genişliğini alır. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | bir  Name  değerinin BÜYÜK HARFLE yazıya dönüştürülüp dönüştürülmediğini gösteren bir değer alır. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Mevcut öğenin bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirerek oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | faktör | double | Ölçekleme faktörü. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Şablon öğesinin adını alır.


**Returns:**
java.lang.String - Şablon öğesinin adını temsil eden büyük harfli bir dize değeri.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Şablon öğesinin sayfa indeksini alır.


**Returns:**
java.lang.Integer - Şablon öğesinin bulunduğu sayfanın indeksini temsil eden tam sayı değeri;  null  şablon öğesi herhangi bir sayfada bulunuyorsa.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Şablon öğesini oluşturmak için kullanılan sayfanın genişliğini alır.


**Returns:**
java.lang.Double - Sayfanın piksel cinsinden genişliği;  null  sayfa genişliği bilinmiyorsa.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


bir  Name  değerinin BÜYÜK HARFLE yazıya dönüştürülüp dönüştürülmediğini gösteren bir değer alır.


**Returns:**
boolean - Bir boolean değeri, bir  Name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösterir.

