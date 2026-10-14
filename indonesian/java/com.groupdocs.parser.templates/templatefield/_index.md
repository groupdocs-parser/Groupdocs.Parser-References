---
title: "TemplateField"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan bidang teks templat."
type: docs
weight: 12
url: /id/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Menyediakan bidang teks templat.

Bidang teks didefinisikan oleh posisinya pada halaman. Ada tiga cara untuk mendefinisikan bidang teks:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield) dengan nama HURUF BESAR. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield) dengan nama HURUF BESAR. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getPosition()](#getPosition--) | Mendapatkan nilai yang menjelaskan cara menemukan bidang templat pada halaman dokumen. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Posisi bidang. |
|
|  | nama | java.lang.String | Nama bidang. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield) dengan nama HURUF BESAR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Posisi bidang. |
|
|  | nama | java.lang.String | Nama bidang. |
|
|  | pageIndex | java.lang.Integer | Nilai integer yang mewakili indeks halaman tempat item templat berada;  null  jika item templat berada di halaman mana saja. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield) dengan nama HURUF BESAR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Posisi bidang. |
|
|  | nama | java.lang.String | Nama bidang. |
|
|  | pageIndex | java.lang.Integer | Nilai integer yang mewakili indeks halaman tempat item templat berada;  null  jika item templat berada di halaman mana saja. |
|
|  | pageWidth | java.lang.Double | Lebar halaman yang digunakan untuk membuat item templat. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Posisi bidang. |
|
|  | nama | java.lang.String | Nama bidang. |
|
|  | pageIndex | java.lang.Integer | Nilai integer yang mewakili indeks halaman tempat item templat berada;  null  jika item templat berada di halaman mana saja. |
|
|  | useUpperCaseName | boolean | Nilai yang menunjukkan apakah sebuah nama dikonversi menjadi HURUF BESAR. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Menginisialisasi instance baru dari kelas [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Posisi bidang. |
|
|  | nama | java.lang.String | Nama bidang. |
|
|  | pageIndex | java.lang.Integer | Nilai integer yang mewakili indeks halaman tempat item templat berada;  null  jika item templat berada di halaman mana saja. |
|
|  | pageWidth | java.lang.Double | Lebar halaman yang digunakan untuk membuat item templat. |
|
|  | useUpperCaseName | boolean | Nilai yang menunjukkan apakah sebuah nama dikonversi menjadi HURUF BESAR. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Mendapatkan nilai yang menjelaskan cara menemukan bidang templat pada halaman dokumen.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

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
