---
title: "TemplateItem"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan kelas abstrak dasar untuk item templat."
type: docs
weight: 14
url: /id/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Menyediakan kelas abstrak dasar untuk item templat.

Pewarisan dari kelas [TemplateItem](../../com.groupdocs.parser.templates/templateitem) digunakan dalam koleksi [Template](../../com.groupdocs.parser.templates/template).

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Membuat salinan item saat ini dengan semua koordinat diskalakan oleh faktor yang diberikan. |
|
|  | [getName()](#getName--) | Mendapatkan nama item templat. |
|
|  | [getPageIndex()](#getPageIndex--) | Mendapatkan indeks halaman dari item templat. |
|
|  | [getPageWidth()](#getPageWidth--) | Mendapatkan lebar halaman yang digunakan untuk membuat item templat. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Mendapatkan nilai yang menunjukkan apakah  Name  telah diubah menjadi UPPER CASE. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Membuat salinan item saat ini dengan semua koordinat diskalakan oleh faktor yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | faktor | double | Faktor skala. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Mendapatkan nama item templat.


**Returns:**
java.lang.String - Nilai string huruf besar yang mewakili nama item templat.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Mendapatkan indeks halaman dari item templat.


**Returns:**
java.lang.Integer - Nilai integer yang mewakili indeks halaman tempat item templat berada;  null  jika item templat berada di halaman mana pun.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Mendapatkan lebar halaman yang digunakan untuk membuat item templat.


**Returns:**
java.lang.Double - Lebar halaman dalam piksel;  null  jika lebar halaman tidak diketahui.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Mendapatkan nilai yang menunjukkan apakah  Name  telah diubah menjadi UPPER CASE.


**Returns:**
boolean - Nilai boolean yang menunjukkan apakah  Name  telah diubah menjadi UPPER CASE.

