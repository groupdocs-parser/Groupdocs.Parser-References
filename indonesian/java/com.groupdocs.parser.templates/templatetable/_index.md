---
title: "TemplateTable"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan tabel templat."
type: docs
weight: 20
url: /id/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Menyediakan tabel templat.

Ada dua cara untuk mendefinisikan tabel:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable) dengan nama UPPER CASE. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable) dengan nama UPPER CASE. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable) dengan nama UPPER CASE. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getLayout()](#getLayout--) | Mendapatkan tata letak tabel. |
|
|  | [getParameters()](#getParameters--) | Mendapatkan parameter untuk mendeteksi tabel dalam mode otomatis. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable) dengan nama UPPER CASE.

Tabel templat diatur oleh tata letak tabel jika tabel tidak dapat terdeteksi secara otomatis:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tata letak tabel. |
|
|  | nama | java.lang.String | Nama tabel. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat tabel templat berada; null jika tabel templat berada di halaman mana saja. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable) dengan nama UPPER CASE.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tata letak tabel. |
|
|  | nama | java.lang.String | Nama tabel. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat tabel templat berada; null jika tabel templat berada di halaman mana saja. |
|
|  | pageWidth | java.lang.Double | Lebar halaman yang digunakan untuk membuat item templat. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tata letak tabel. |
|
|  | nama | java.lang.String | Nama tabel. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat tabel templat berada; null jika tabel templat berada di halaman mana saja. |
|
|  | useUpperCaseName | boolean | Nilai yang menunjukkan apakah sebuah nama dikonversi menjadi HURUF BESAR. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tata letak tabel. |
|
|  | nama | java.lang.String | Nama tabel. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat tabel templat berada; null jika tabel templat berada di halaman mana saja. |
|
|  | pageWidth | java.lang.Double | Lebar halaman yang digunakan untuk membuat item templat. |
|
|  | useUpperCaseName | boolean | Nilai yang menunjukkan apakah sebuah nama dikonversi menjadi HURUF BESAR. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable) dengan nama UPPER CASE.

Jika tabel templat diatur oleh parameter detektor, tabel akan terdeteksi secara otomatis:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Parameter untuk mendeteksi tabel dalam mode otomatis. |
|
|  | nama | java.lang.String | Nama tabel. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat tabel templat berada; null jika tabel templat berada di halaman mana saja. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Parameter untuk mendeteksi tabel dalam mode otomatis. |
|
|  | nama | java.lang.String | Nama tabel. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat tabel templat berada; null jika tabel templat berada di halaman mana saja. |
|
|  | pageWidth | java.lang.Double | Lebar halaman yang digunakan untuk membuat item templat. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Parameter untuk mendeteksi tabel dalam mode otomatis. |
|
|  | nama | java.lang.String | Nama tabel. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat tabel templat berada; null jika tabel templat berada di halaman mana saja. |
|
|  | useUpperCaseName | boolean | Nilai yang menunjukkan apakah sebuah nama dikonversi menjadi HURUF BESAR. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Menginisialisasi instance baru dari kelas [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Parameter untuk mendeteksi tabel dalam mode otomatis. |
|
|  | nama | java.lang.String | Nama tabel. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat tabel templat berada; null jika tabel templat berada di halaman mana saja. |
|
|  | pageWidth | java.lang.Double | Lebar halaman yang digunakan untuk membuat item templat. |
|
|  | useUpperCaseName | boolean | Nilai yang menunjukkan apakah sebuah nama dikonversi menjadi HURUF BESAR. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Mendapatkan tata letak tabel.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Mendapatkan parameter untuk mendeteksi tabel dalam mode otomatis.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

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
