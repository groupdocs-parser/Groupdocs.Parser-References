---
title: "Page"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili informasi halaman dokumen seperti indeks halaman dan ukuran halaman."
type: docs
weight: 16
url: /id/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Mewakili informasi halaman dokumen seperti indeks halaman dan ukuran halaman. Ini digunakan untuk mewakili halaman yang berisi turunan kelas [PageArea](../../com.groupdocs.parser.data/pagearea) dalam fungsi parsing dengan template.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Menginisialisasi instance baru dari kelas [Page](../../com.groupdocs.parser.data/page). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getIndex()](#getIndex--) | Mendapatkan indeks halaman. |
|
|  | [getSize()](#getSize--) | Mendapatkan ukuran halaman. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Menginisialisasi instance baru dari kelas [Page](../../com.groupdocs.parser.data/page).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indeks | int | Indeks halaman. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Ukuran halaman. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Mendapatkan indeks halaman.


**Returns:**
int - Indeks halaman berbasis nol.

### getSize() {#getSize--}
```
public Size getSize()
```


Mendapatkan ukuran halaman.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.

