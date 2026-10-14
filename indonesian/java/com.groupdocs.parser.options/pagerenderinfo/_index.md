---
title: "PageRenderInfo"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili informasi tentang bagaimana halaman dirender."
type: docs
weight: 30
url: /id/java/com.groupdocs.parser.options/pagerenderinfo/
---
**Inheritance:**
java.lang.Object
```
public class PageRenderInfo
```

Mewakili informasi tentang bagaimana halaman dirender.

Beberapa dokumen (misalnya spreadsheet) tidak dapat merender halaman
sebagai satu gambar. Untuk dokumen tersebut, halaman dirender sebagai sekumpulan ubin.
Ubin-ubin ini ditempatkan dalam tabel persegi panjang.


RowCount
dan
ColumnCount
mewakili total jumlah baris dan kolom
dari tabel ini. Jika halaman dokumen dirender menjadi satu gambar, properti ini bernilai 1.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageRenderInfo(int pageNumber, int rowCount, int columnCount)](#PageRenderInfo-int-int-int-) | Menginisialisasi instance baru dari kelas [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) class. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Mendapatkan nomor halaman. |
|
|  | [getRowCount()](#getRowCount--) | Dapatkan total jumlah baris ubin. |
|
|  | [getColumnCount()](#getColumnCount--) | Dapatkan total jumlah kolom ubin. |
|
|  | [getColumn(int tileIndex)](#getColumn-int-) | Mengembalikan indeks kolom tempat ubin dengan  tileIndex  ditempatkan. |
|
|  | [getRow(int tileIndex)](#getRow-int-) | Mengembalikan indeks baris tempat ubin dengan  tileIndex  ditempatkan. |
|
### PageRenderInfo(int pageNumber, int rowCount, int columnCount) {#PageRenderInfo-int-int-int-}
```
public PageRenderInfo(int pageNumber, int rowCount, int columnCount)
```


Menginisialisasi instance baru dari kelas [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) class.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageNumber | int | Nomor halaman (dimulai dari 1). |
|
|  | rowCount | int | Jumlah total baris ubin. |
|
|  | columnCount | int | Jumlah total kolom ubin. |
|

### getPageNumber() {#getPageNumber--}
```
public int getPageNumber()
```


Mendapatkan nomor halaman.


**Returns:**
int - Nilai integer yang mewakili nomor halaman (dimulai dari 1).

### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Dapatkan total jumlah baris ubin.


**Returns:**
int - Nilai integer yang mewakili jumlah total baris ubin.

### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Dapatkan total jumlah kolom ubin.


**Returns:**
int - Nilai integer yang mewakili jumlah total kolom ubin.

### getColumn(int tileIndex) {#getColumn-int-}
```
public int getColumn(int tileIndex)
```


Mengembalikan indeks kolom tempat ubin dengan  tileIndex  ditempatkan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | tileIndex | int | Indeks ubin berbasis nol. |
|

**Returns:**
int - Nilai integer berbasis nol yang mewakili indeks kolom.

### getRow(int tileIndex) {#getRow-int-}
```
public int getRow(int tileIndex)
```


Mengembalikan indeks baris tempat ubin dengan  tileIndex  ditempatkan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | tileIndex | int | Indeks ubin berbasis nol. |
|

**Returns:**
int - Nilai integer berbasis nol yang mewakili indeks baris.

