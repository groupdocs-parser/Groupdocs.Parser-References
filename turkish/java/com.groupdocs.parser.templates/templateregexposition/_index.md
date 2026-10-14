---
title: "TemplateRegexPosition"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Düzenli ifadeyi kullanan bir şablon alan konumunu sağlar."
type: docs
weight: 19
url: /tr/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Düzenli ifadeyi kullanan bir şablon alan konumunu sağlar.

Aşağıdaki örnek, belgenin "Invoice Number INV-12345" içermesi durumunu gösterir.
Şablon alanı aşağıdaki şekilde tanımlanabilir:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

Bu durumda değer olarak tüm dize çıkarılır. Sadece dize'nin bir kısmını çıkarmak için
"value" düzenli ifade grubu kullanılır:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

Bu durumda değer olarak "INV-3337" dizesi çıkarılır.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Yeni bir [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) sınıfının örneğini başlatır. |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Yeni bir [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) sınıfının örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getExpression()](#getExpression--) | Düzenli ifadeyi alır. |
|
|  | [isMatchCase()](#isMatchCase--) | Metin durumunun yoksayılmadığını gösteren değeri alır. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Yeni bir [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ifade | java.lang.String | Düzenli ifade. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Yeni bir [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ifade | java.lang.String | Düzenli ifade. |
|
|  | matchCase | boolean | Metin büyük/küçük harfinin yoksayılmadığını gösteren değer. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Düzenli ifadeyi alır.


**Returns:**
java.lang.String - Düzenli ifadeyi temsil eden bir dize.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Metin durumunun yoksayılmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin büyük/küçük harfi yoksayılmıyorsa; aksi takdirde,  false .

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
