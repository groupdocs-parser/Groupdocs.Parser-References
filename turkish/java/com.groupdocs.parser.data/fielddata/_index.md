---
title: "FieldData"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Bir ad, sayfa indeksi, alan değeri vb. gibi alan verilerini temsil eder."
type: docs
weight: 13
url: /tr/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Bir ad, bir sayfa indeksi, bir alan değeri vb. gibi alan verilerini temsil eder. Alana bağlı olarak değer bir metin, bir görüntü, bir tablo vb. olabilir.

[FieldData](../../com.groupdocs.parser.data/fielddata) sınıfının örnekleri, [DocumentData](../../com.groupdocs.parser.data/documentdata) koleksiyonunda kullanılır.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getName()](#getName--) | Alan adını alır. |
|
|  | [getPageIndex()](#getPageIndex--) | Sayfa indeksini alır. |
|
|  | [getPageArea()](#getPageArea--) | Alan değerini alır. |
|
|  | [getLinkedField()](#getLinkedField--) | Bağlantılı alanı alır. |
|
|  | [getText()](#getText--) | Metni alır. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | bir  Name  değerinin BÜYÜK HARFLE yazıya dönüştürülüp dönüştürülmediğini gösteren bir değer alır. |
|
### getName() {#getName--}
```
public String getName()
```


Alan adını alır.


**Returns:**
java.lang.String - Alan adını temsil eden büyük harfli bir dize değeri.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Sayfa indeksini alır.


**Returns:**
int - Alanı içeren sayfanın sıfır tabanlı indeksi.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Alan değerini alır.

Alana bağlı olarak PageArea özelliği, [PageArea](../../com.groupdocs.parser.data/pagearea) sınıfının herhangi bir türevi içerebilir.
Örneğin, [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) yöntemi yalnızca metin alanlarını çıkarır.

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


Bağlantılı alanı alır.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Metni alır.


**Returns:**
java.lang.String - Alan metninin değerini temsil eden bir dize değeri; [PageArea](../../com.groupdocs.parser.data/pagearea) özelliği [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) değilse  null.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


bir  Name  değerinin BÜYÜK HARFLE yazıya dönüştürülüp dönüştürülmediğini gösteren bir değer alır.


**Returns:**
boolean - Bir boolean değeri, bir  Name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösterir.

