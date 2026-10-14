---
title: "TemplateTableLayout"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablon tablo düzenini sağlar; bu, tablo konumunu tanımlamak için  sınıfı tarafından kullanılır."
type: docs
weight: 21
url: /tr/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Şablon tablo düzenini sağlar; bu, tablo konumunu tanımlamak için [TemplateTable](../../com.groupdocs.parser.templates/templatetable) sınıfı tarafından kullanılır.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Yeni bir [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) sınıfının örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Tabloyu içeren dikdörtgen alanı alır. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Tablo sütun ayırıcılarını alır. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Tablo satır ayırıcılarını alır. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Aynı boyut, ayırıcılar ve noktadaki konumla yeni bir düzen oluşturur. |
|
|  | [scale(double factor)](#scale-double-) | Bu düzenin bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirilmiş şekilde oluşturur. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Yeni bir [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Tablo sütun ayırıcıları. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | Tablo satır ayırıcıları. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Tabloyu içeren dikdörtgen alanı alır.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Tablo sütun ayırıcılarını alır.


**Returns:**
java.util.List<java.lang.Double> - Tablo sütun ayırıcılarının x-koordinatlarını temsil eden double değerlerinin bir koleksiyonu.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Tablo satır ayırıcılarını alır.


**Returns:**
java.util.List<java.lang.Double> - Tablo satır ayırıcılarının y-koordinatlarını temsil eden double değerlerinin bir koleksiyonu.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Aynı boyut, ayırıcılar ve noktadaki konumla yeni bir düzen oluşturur.

Bu işlevsellik Table Layout'ı taşımaya izin verir.

Örneğin, bir belge her sayfada tablolar içerir (veya sayfada bir tablo bulunan bir dizi belge).
Bu tablolar konum ve içerik açısından farklıdır, ancak aynı sütun ve satırlara sahiptir. Bu durumda bir kullanıcı
bir [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) nesnesini (0, 0) konumunda bir kez tanımlayabilir ve ardından belirli tablonun konumuna taşıyabilir.

Tablo konumu sayfanın diğer nesnesine bağlıysa, bir kullanıcı [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) nesnesini tanımlayabilir
şablon belgeye dayanarak ve ardından bir çapa nesnesine göre taşıyabilir. Örneğin, bu bir özet tabloysa
ve detay tablosu izler (farklı sayıda satır içerebilir). Bu durumda bir kullanıcı tanımlayabilir
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
metod mevcut nesnenin bir kopyasını döndürür. Bir kullanıcı herhangi bir koordinat geçirebilir
(negatif olsa bile - o zaman düzen sola/üste taşınır).

````
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
````



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | Yeni düzenin konumu. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Bu düzenin bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirilmiş şekilde oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | faktör | double | Ölçekleme faktörü. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.

