---
title: "Point"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Bir noktayı temsil eder."
type: docs
weight: 25
url: /tr/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Bir noktayı temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Yeni bir [Point](../../com.groupdocs.parser.data/point) sınıfı örneği oluşturur. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getX()](#getX--) | x koordinatını alır. |
|
|  | [getY()](#getY--) | y koordinatını alır. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Bir noktanın dize temsilini sınıf eşdeğerine dönüştürür. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Yeni bir [Point](../../com.groupdocs.parser.data/point) sınıfı örneği oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | x | double | x-koordinatı. |
|
|  | y | double | y-koordinatı. |
|

### getX() {#getX--}
```
public double getX()
```


x koordinatını alır.


**Returns:**
double - x-koordinatını temsil eden bir double değeri.

### getY() {#getY--}
```
public double getY()
```


y koordinatını alır.


**Returns:**
double - y-koordinatını temsil eden bir double değeri.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Bir noktanın dize temsilini sınıf eşdeğerine dönüştürür. Döndürülen değer, dönüşümün başarılı olup olmadığını gösterir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | s | java.lang.String | Dönüştürülecek bir nokta içeren bir dize. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
