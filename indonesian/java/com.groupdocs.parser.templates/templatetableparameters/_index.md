---
title: "TemplateTableParameters"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan parameter untuk algoritma deteksi tabel."
type: docs
weight: 22
url: /id/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Menyediakan parameter untuk algoritma deteksi tabel.

Ada dua algoritma untuk mendeteksi tabel:

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

Dalam beberapa kasus ketika algoritma tidak dapat mendeteksi tabel atau melakukannya dengan cara yang tidak akurat, kelas [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) digunakan.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Menginisialisasi instance baru dari kelas [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Menginisialisasi instance baru dari kelas [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Mendapatkan area persegi panjang yang berisi tabel. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Mendapatkan pemisah kolom tabel. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Mengambil nilai yang menunjukkan apakah tabel memiliki sel yang digabung. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Mengambil jumlah minimum baris tabel. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Mengambil jumlah minimum kolom tabel. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Mengambil ruang minimum antara kolom tabel. |
|
|  | [scale(double factor)](#scale-double-) | Membuat salinan parameter ini dengan semua koordinat diskalakan oleh faktor yang diberikan. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Menginisialisasi instance baru dari kelas [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi tabel. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Pemisah kolom tabel. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Menginisialisasi instance baru dari kelas [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi tabel. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Pemisah kolom tabel. |
|
|  | mergedCells | java.lang.Boolean | Nilai yang menunjukkan apakah tabel memiliki sel yang digabung. |
|
|  | minRowCount | java.lang.Integer | Jumlah minimum baris tabel. |
|
|  | minColumnCount | java.lang.Integer | Jumlah minimum kolom tabel. |
|
|  | minVerticalSpace | java.lang.Integer | Ruang minimum antara kolom tabel. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Mendapatkan area persegi panjang yang berisi tabel.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Mendapatkan pemisah kolom tabel.


**Returns:**
java.util.List<java.lang.Double> - Sekumpulan nilai double yang mewakili koordinat x pemisah kolom tabel;  null  jika tidak disetel.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Mengambil nilai yang menunjukkan apakah tabel memiliki sel yang digabung.


**Returns:**
java.lang.Boolean -  true  jika tabel memiliki sel yang digabung; jika tidak,  false .  null  jika tidak disetel.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Mengambil jumlah minimum baris tabel.


**Returns:**
java.lang.Integer - Nilai integer yang mewakili jumlah minimum baris tabel;  null  jika tidak disetel.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Mengambil jumlah minimum kolom tabel.


**Returns:**
java.lang.Integer - Nilai integer yang mewakili jumlah minimum kolom tabel;  null  jika tidak disetel.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Mengambil ruang minimum antara kolom tabel.


**Returns:**
java.lang.Integer - Nilai integer yang mewakili ruang minimum antara kolom tabel;  null  jika tidak disetel.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Membuat salinan parameter ini dengan semua koordinat diskalakan oleh faktor yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | faktor | double | Faktor skala. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

