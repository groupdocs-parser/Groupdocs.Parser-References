---
title: "TemplateBarcode"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan bidang kode batang templat."
type: docs
weight: 11
url: /id/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Menyediakan bidang kode batang templat.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) dengan nama HURUF BESAR. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) dengan nama HURUF BESAR. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Mendapatkan area persegi panjang yang berisi bidang barcode templat. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi bidang barcode templat. |
|
|  | nama | java.lang.String | Nama bidang barcode. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) dengan nama HURUF BESAR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi bidang barcode templat. |
|
|  | nama | java.lang.String | Nama bidang barcode. |
|
|  | pageIndex | java.lang.Integer | Nilai integer yang mewakili indeks halaman tempat item templat berada;  null  jika item templat berada di halaman mana saja. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) dengan nama HURUF BESAR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi bidang barcode templat. |
|
|  | nama | java.lang.String | Nama bidang barcode. |
|
|  | pageIndex | java.lang.Integer | Nilai integer yang mewakili indeks halaman tempat item templat berada;  null  jika item templat berada di halaman mana saja. |
|
|  | pageWidth | java.lang.Double | Lebar halaman yang digunakan untuk membuat item templat. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi bidang barcode templat. |
|
|  | nama | java.lang.String | Nama bidang barcode. |
|
|  | pageIndex | java.lang.Integer | Nilai integer yang mewakili indeks halaman tempat item templat berada;  null  jika item templat berada di halaman mana saja. |
|
|  | useUpperCaseName | boolean | Nilai yang menunjukkan apakah sebuah nama dikonversi menjadi HURUF BESAR. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Menginisialisasi instance baru dari kelas [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi bidang barcode templat. |
|
|  | nama | java.lang.String | Nama bidang barcode. |
|
|  | pageIndex | java.lang.Integer | Nilai integer yang mewakili indeks halaman tempat item templat berada;  null  jika item templat berada di halaman mana saja. |
|
|  | pageWidth | java.lang.Double | Lebar halaman yang digunakan untuk membuat item templat. |
|
|  | useUpperCaseName | boolean | Nilai yang menunjukkan apakah sebuah nama dikonversi menjadi HURUF BESAR. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Mendapatkan area persegi panjang yang berisi bidang barcode templat.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Membuat salinan item saat ini dengan semua koordinat diskalakan oleh faktor yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| faktor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
