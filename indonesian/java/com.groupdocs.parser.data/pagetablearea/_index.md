---
title: "PageTableArea"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili area tabel halaman yang digunakan untuk mewakili tabel dalam fungsi parsing dengan templat."
type: docs
weight: 22
url: /id/java/com.groupdocs.parser.data/pagetablearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTableArea extends PageArea
```

Mewakili area tabel halaman yang digunakan untuk mewakili tabel dalam fungsi parsing dengan templat.

[PageTableArea](../../com.groupdocs.parser.data/pagetablearea) class is used to organize inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in table structure.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)](#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi instance baru dari kelas [PageTableArea](../../com.groupdocs.parser.data/pagetablearea). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCells()](#getCells--) | Mendapatkan koleksi sel. |
|
|  | [getRowCount()](#getRowCount--) | Mendapatkan total jumlah baris tabel. |
|
|  | [getColumnCount()](#getColumnCount--) | Mendapatkan total jumlah kolom tabel. |
|
|  | [getRowHeight(int rowIndex)](#getRowHeight-int-) | Mengembalikan tinggi baris. |
|
|  | [getColumnWidth(int columnIndex)](#getColumnWidth-int-) | Mengembalikan lebar kolom. |
|
|  | [getCell(int rowIndex, int columnIndex)](#getCell-int-int-) | Mendapatkan sel tabel berdasarkan indeks baris dan kolom. |
|
### PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle) {#PageTableArea-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--java.lang.Iterable-com.groupdocs.parser.data.PageTableAreaCell--com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTableArea(Iterable<Double> rows, Iterable<Double> columns, Iterable<PageTableAreaCell> cells, Page page, Rectangle rectangle)
```


Menginisialisasi instance baru dari kelas [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

Catatan: proyek C# menandai konstruktor ini sebagai
internal
(commit 954951f). Dalam Java, "internal-to-the-assembly"
tidak diterjemahkan dengan bersih ke package-private karena produsen (
WordProcessingParser
,
TableAreaParser
,
dll.) berada di
com.groupdocs.parser
, bukan
com.groupdocs.parser.data
. Oleh karena itu konstruktor ini dibiarkan

public
sehingga konstruksi lintas paket masih berfungsi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | baris | java.lang.Iterable<java.lang.Double> | Koleksi tinggi baris. |
|
|  | kolom | java.lang.Iterable<java.lang.Double> | Koleksi lebar kolom. |
|
|  | sel | java.lang.Iterable<com.groupdocs.parser.data.PageTableAreaCell> | Koleksi sel. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Halaman yang berisi tabel. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi tabel. |
|

### getCells() {#getCells--}
```
public Collection<PageTableAreaCell> getCells()
```


Mendapatkan koleksi sel. Koleksi tabel sel yang hanya-baca sederhana.


**Returns:**
java.util.Collection<com.groupdocs.parser.data.PageTableAreaCell> - Sebuah koleksi sel tabel

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Mendapatkan total jumlah baris tabel.


**Returns:**
int - Nilai integer yang berisi total jumlah baris tabel.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Mendapatkan total jumlah kolom tabel.


**Returns:**
int - Nilai integer yang berisi total jumlah kolom tabel.

### getRowHeight(int rowIndex) {#getRowHeight-int-}
```
public double getRowHeight(int rowIndex)
```


Mengembalikan tinggi baris.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rowIndex | int | Indeks berbasis nol dari baris. |
|

**Returns:**
double - Nilai double yang merepresentasikan tinggi baris.

### getColumnWidth(int columnIndex) {#getColumnWidth-int-}
```
public double getColumnWidth(int columnIndex)
```


Mengembalikan lebar kolom.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | columnIndex | int | Indeks berbasis nol dari kolom. |
|

**Returns:**
double - Nilai double yang mewakili lebar kolom.

### getCell(int rowIndex, int columnIndex) {#getCell-int-int-}
```
public PageTableAreaCell getCell(int rowIndex, int columnIndex)
```


Mendapatkan sel tabel berdasarkan indeks baris dan kolom.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rowIndex | int | Indeks berbasis nol dari baris sel. |
|
|  | columnIndex | int | Indeks berbasis nol dari kolom sel. |
|

**Returns:**
[PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) - An instance of [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell) class;  null  if no cell is found.

