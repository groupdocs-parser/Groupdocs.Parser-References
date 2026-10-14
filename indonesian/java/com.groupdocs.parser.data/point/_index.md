---
title: "Point"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili titik."
type: docs
weight: 25
url: /id/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Mewakili titik.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Menginisialisasi sebuah instance baru dari kelas [Point](../../com.groupdocs.parser.data/point). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getX()](#getX--) | Mendapatkan koordinat x. |
|
|  | [getY()](#getY--) | Mendapatkan koordinat y. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Mengonversi representasi string dari sebuah titik ke kelas yang setara. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Menginisialisasi sebuah instance baru dari kelas [Point](../../com.groupdocs.parser.data/point).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | x | double | Koordinat x. |
|
|  | y | double | Koordinat y. |
|

### getX() {#getX--}
```
public double getX()
```


Mendapatkan koordinat x.


**Returns:**
double - Nilai double yang mewakili koordinat x.

### getY() {#getY--}
```
public double getY()
```


Mendapatkan koordinat y.


**Returns:**
double - Nilai double yang mewakili koordinat y.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Mengonversi representasi string dari sebuah titik ke ekivalen kelasnya. Nilai kembali menunjukkan apakah konversi berhasil atau gagal.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | s | java.lang.String | String yang berisi sebuah titik untuk dikonversi. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
