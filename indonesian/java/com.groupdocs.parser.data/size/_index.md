---
title: "Size"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili ukuran."
type: docs
weight: 28
url: /id/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Mewakili ukuran.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | Menginisialisasi instance baru dari kelas [Size](../../com.groupdocs.parser.data/size). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getWidth()](#getWidth--) | Mendapatkan lebar. |
|
|  | [getHeight()](#getHeight--) | Mendapatkan tinggi. |
|
|  | [isEmpty()](#isEmpty--) | Mendapatkan nilai yang menunjukkan apakah ukuran kosong. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Mengonversi representasi string dari ukuran ke ekivalen kelasnya. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Menginisialisasi instance baru dari kelas [Size](../../com.groupdocs.parser.data/size).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lebar | double | Lebar dalam piksel. |
|
|  | tinggi | double | Tinggi dalam piksel. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Mendapatkan lebar.


**Returns:**
double - Nilai double yang mewakili lebar dalam piksel.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Mendapatkan tinggi.


**Returns:**
double - Nilai double yang mewakili tinggi dalam piksel.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Mendapatkan nilai yang menunjukkan apakah ukuran kosong.


**Returns:**
boolean -  true  jika lebar dan tinggi nol; selainnya,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Mengonversi representasi string dari ukuran ke ekivalen kelasnya. Nilai kembali menunjukkan apakah konversi berhasil atau gagal.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | s | java.lang.String | String yang berisi ukuran untuk dikonversi. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
