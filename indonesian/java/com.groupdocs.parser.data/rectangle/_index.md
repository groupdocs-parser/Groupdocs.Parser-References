---
title: "Rectangle"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili area persegi panjang."
type: docs
weight: 26
url: /id/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Mewakili area persegi panjang.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Menginisialisasi instance baru dari kelas [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Menginisialisasi instance baru dari kelas [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getLeft()](#getLeft--) | Mendapatkan koordinat x dari tepi kiri area persegi panjang. |
|
|  | [getTop()](#getTop--) | Mendapatkan koordinat y dari tepi atas area persegi panjang. |
|
|  | [getRight()](#getRight--) | Mendapatkan koordinat x dari tepi kanan area persegi panjang. |
|
|  | [getBottom()](#getBottom--) | Mendapatkan koordinat y dari tepi bawah area persegi panjang. |
|
|  | [getPosition()](#getPosition--) | Mendapatkan koordinat sudut kiri-atas area persegi panjang. |
|
|  | [getSize()](#getSize--) | Mendapatkan ukuran. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Menginisialisasi instance baru dari kelas [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kiri | double | Koordinat x dari tepi kiri area persegi panjang. |
|
|  | atas | double | Koordinat y dari tepi atas area persegi panjang. |
|
|  | kanan | double | Koordinat x dari tepi kanan area persegi panjang. |
|
|  | bawah | double | Koordinat y dari tepi bawah area persegi panjang. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Menginisialisasi instance baru dari kelas [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | Koordinat sudut kiri-atas area persegi panjang. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Ukuran area persegi panjang. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Mendapatkan koordinat x dari tepi kiri area persegi panjang.


**Returns:**
double - Nilai double yang mewakili koordinat x dari tepi kiri area persegi panjang.

### getTop() {#getTop--}
```
public double getTop()
```


Mendapatkan koordinat y dari tepi atas area persegi panjang.


**Returns:**
double - Nilai double yang mewakili koordinat y dari tepi atas area persegi panjang.

### getRight() {#getRight--}
```
public double getRight()
```


Mendapatkan koordinat x dari tepi kanan area persegi panjang.


**Returns:**
double - Nilai double yang mewakili koordinat x dari tepi kanan area persegi panjang.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Mendapatkan koordinat y dari tepi bawah area persegi panjang.


**Returns:**
double - Nilai double yang mewakili koordinat y dari tepi bawah area persegi panjang.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Mendapatkan koordinat sudut kiri-atas area persegi panjang.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Mendapatkan ukuran.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
