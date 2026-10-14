---
title: "TemplateField"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablon metin alanını sağlar."
type: docs
weight: 12
url: /tr/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Şablon metin alanını sağlar.

Metin alanları sayfadaki konumuna göre tanımlanır. Bir metin alanını tanımlamanın üç yolu vardır:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneği başlatır. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneğini BÜYÜK HARF adıyla başlatır. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneğini BÜYÜK HARF adıyla başlatır. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneği başlatır. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getPosition()](#getPosition--) | Şablon alanını belge sayfasında nasıl bulacağını açıklayan değeri alır. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Alan konumu. |
|
|  | ad | java.lang.String | Alan adı. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneğini BÜYÜK HARF adıyla başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Alan konumu. |
|
|  | ad | java.lang.String | Alan adı. |
|
|  | pageIndex | java.lang.Integer | Şablon öğesinin bulunduğu sayfanın dizinini temsil eden bir tamsayı değeri;  null  şablon öğesi herhangi bir sayfada bulunuyorsa. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneğini BÜYÜK HARF adıyla başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Alan konumu. |
|
|  | ad | java.lang.String | Alan adı. |
|
|  | pageIndex | java.lang.Integer | Şablon öğesinin bulunduğu sayfanın dizinini temsil eden bir tamsayı değeri;  null  şablon öğesi herhangi bir sayfada bulunuyorsa. |
|
|  | pageWidth | java.lang.Double | Şablon öğesini oluşturmak için kullanılan sayfanın genişliği. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Alan konumu. |
|
|  | ad | java.lang.String | Alan adı. |
|
|  | pageIndex | java.lang.Integer | Şablon öğesinin bulunduğu sayfanın dizinini temsil eden bir tamsayı değeri;  null  şablon öğesi herhangi bir sayfada bulunuyorsa. |
|
|  | useUpperCaseName | boolean | Bir  name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösteren değer. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Yeni bir [TemplateField](../../com.groupdocs.parser.templates/templatefield) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Alan konumu. |
|
|  | ad | java.lang.String | Alan adı. |
|
|  | pageIndex | java.lang.Integer | Şablon öğesinin bulunduğu sayfanın dizinini temsil eden bir tamsayı değeri;  null  şablon öğesi herhangi bir sayfada bulunuyorsa. |
|
|  | pageWidth | java.lang.Double | Şablon öğesini oluşturmak için kullanılan sayfanın genişliği. |
|
|  | useUpperCaseName | boolean | Bir  name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösteren değer. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Şablon alanını belge sayfasında nasıl bulacağını açıklayan değeri alır.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

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
