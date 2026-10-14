---
title: "Size"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Bir boyutu temsil eder."
type: docs
weight: 28
url: /tr/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Bir boyutu temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | [Size](../../com.groupdocs.parser.data/size) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getWidth()](#getWidth--) | Genişliği alır. |
|
|  | [getHeight()](#getHeight--) | Yüksekliği alır. |
|
|  | [isEmpty()](#isEmpty--) | Boyutun boş olup olmadığını gösteren bir değeri alır. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Bir boyutun dize temsilini sınıf eşdeğerine dönüştürür. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


[Size](../../com.groupdocs.parser.data/size) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | genişlik | double | Piksel cinsinden genişlik. |
|
|  | yükseklik | double | Piksel cinsinden yükseklik. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Genişliği alır.


**Returns:**
double - Piksel cinsinden genişliği temsil eden bir double değeri.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Yüksekliği alır.


**Returns:**
double - Piksel cinsinden yüksekliği temsil eden bir double değeri.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Boyutun boş olup olmadığını gösteren bir değeri alır.


**Returns:**
boolean -  true  eğer genişlik ve yükseklik sıfırsa; aksi takdirde,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Bir boyutun dize temsilini sınıf eşdeğerine dönüştürür. Dönüş değeri dönüşün başarılı olup olmadığını gösterir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | s | java.lang.String | Dönüştürülecek bir boyut içeren dize. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
