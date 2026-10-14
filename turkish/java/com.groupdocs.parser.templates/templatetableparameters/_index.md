---
title: "TemplateTableParameters"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Tablo algılama algoritmaları için parametreler sağlar."
type: docs
weight: 22
url: /tr/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Tablo algılama algoritmaları için parametreler sağlar.

Bir tablo tespit etmek için iki algoritma vardır:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

Algoritmaların bir tabloyu tespit edemediği veya doğru olmayan bir şekilde tespit ettiği bazı durumlarda [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) sınıfı kullanılır.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Tabloyu içeren dikdörtgen alanı alır. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Tablo sütun ayırıcılarını alır. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Tablonun birleştirilmiş hücrelere sahip olup olmadığını gösteren değeri alır. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Tablonun minimum satır sayısını alır. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Tablonun minimum sütun sayısını alır. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Tablo sütunları arasındaki minimum boşluğu alır. |
|
|  | [scale(double factor)](#scale-double-) | Bu parametrelerin bir kopyasını oluşturur ve tüm koordinatları verilen faktörle ölçeklendirir. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Tabloyu içeren dikdörtgen alan. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Tablo sütun ayırıcıları. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Tabloyu içeren dikdörtgen alan. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Tablo sütun ayırıcıları. |
|
|  | mergedCells | java.lang.Boolean | Tablonun birleştirilmiş hücreleri olup olmadığını gösteren değer. |
|
|  | minRowCount | java.lang.Integer | Tablo satırlarının minimum sayısı. |
|
|  | minColumnCount | java.lang.Integer | Tablo sütunlarının minimum sayısı. |
|
|  | minVerticalSpace | java.lang.Integer | Tablo sütunları arasındaki minimum boşluk. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Tabloyu içeren dikdörtgen alanı alır.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Tablo sütun ayırıcılarını alır.


**Returns:**
java.util.List<java.lang.Double> - Tablo sütun ayırıcılarının x koordinatlarını temsil eden çift değerlerin koleksiyonu;  null  ayarlanmamışsa.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Tablonun birleştirilmiş hücrelere sahip olup olmadığını gösteren değeri alır.


**Returns:**
java.lang.Boolean -  true  tablo birleştirilmiş hücrelere sahipse; aksi takdirde,  false .  null  ayarlanmamışsa.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Tablonun minimum satır sayısını alır.


**Returns:**
java.lang.Integer - Tablo satırlarının minimum sayısını temsil eden tam sayı değeri;  null  ayarlanmamışsa.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Tablonun minimum sütun sayısını alır.


**Returns:**
java.lang.Integer - Tablo sütunlarının minimum sayısını temsil eden tam sayı değeri;  null  ayarlanmamışsa.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Tablo sütunları arasındaki minimum boşluğu alır.


**Returns:**
java.lang.Integer - Tablo sütunları arasındaki minimum boşluğu temsil eden tam sayı değeri;  null  ayarlanmamışsa.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Bu parametrelerin bir kopyasını oluşturur ve tüm koordinatları verilen faktörle ölçeklendirir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | faktör | double | Ölçekleme faktörü. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

