---
title: "TemplateTableLayout"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan tata letak tabel templat yang digunakan oleh kelas untuk menentukan posisi tabel."
type: docs
weight: 21
url: /id/java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Menyediakan tata letak tabel templat yang digunakan oleh kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable) untuk menentukan posisi tabel.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Menginisialisasi instance baru dari kelas [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Mendapatkan area persegi panjang yang berisi tabel. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Mendapatkan pemisah kolom tabel. |
|
|  | [getHorizontalSeparators()](#getHorizontalSeparators--) | Mendapatkan pemisah baris tabel. |
|
|  | [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Membuat tata letak baru dengan ukuran, pemisah, dan posisi yang sama pada titik. |
|
|  | [scale(double factor)](#scale-double-) | Membuat salinan tata letak ini dengan semua koordinat diskalakan oleh faktor yang diberikan. |
|
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Menginisialisasi instance baru dari kelas [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Pemisah kolom tabel. |
|
|  | horizontalSeparators | java.lang.Iterable<java.lang.Double> | Pemisah baris tabel. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Mendapatkan area persegi panjang yang berisi tabel.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Mendapatkan pemisah kolom tabel.


**Returns:**
java.util.List<java.lang.Double> - Sekumpulan nilai double yang mewakili koordinat x dari pemisah kolom tabel.

### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Mendapatkan pemisah baris tabel.


**Returns:**
java.util.List<java.lang.Double> - Sekumpulan nilai double yang mewakili koordinat y dari pemisah baris tabel.

### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Membuat tata letak baru dengan ukuran, pemisah, dan posisi yang sama pada titik.

Fungsionalitas ini memungkinkan untuk memindahkan Tata Letak Tabel.

Misalnya, sebuah dokumen memiliki tabel di setiap halaman (atau sekumpulan dokumen dengan tabel pada halaman).
Tabel-tabel ini berbeda dalam posisi dan konten, tetapi memiliki kolom dan baris yang sama. Dalam kasus ini pengguna
dapat mendefinisikan objek [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) pada (0, 0) sekali dan kemudian memindahkannya ke lokasi tabel yang pasti.

Jika posisi tabel tergantung pada objek lain di halaman, pengguna dapat mendefinisikan objek [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout)
berdasarkan dokumen templat dan kemudian memindahkannya sesuai dengan objek jangkar. Misalnya, jika ini adalah tabel ringkasan
dan diikuti oleh tabel detail (yang dapat berisi jumlah baris yang berbeda). Dalam kasus ini pengguna dapat mendefinisikan
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.


moveTo(Point)
metode mengembalikan salinan objek saat ini. Pengguna dapat memberikan koordinat apa pun
(bahkan negatif - maka tata letak akan dipindahkan ke kiri/atas).

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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | point | [Point](../../com.groupdocs.parser.data/point) | Posisi tata letak baru. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.

### scale(double factor) {#scale-double-}
```
public TemplateTableLayout scale(double factor)
```


Membuat salinan tata letak ini dengan semua koordinat diskalakan oleh faktor yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | faktor | double | Faktor skala. |
|

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) with scaled separators.

