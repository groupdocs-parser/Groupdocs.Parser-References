---
title: "PageTableAreaCell"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili sel tabel yang digunakan dalam kelas."
type: docs
weight: 23
url: /id/java/com.groupdocs.parser.data/pagetableareacell/
---
**Inheritance:**
java.lang.Object
```
public class PageTableAreaCell
```

Mewakili sel tabel yang digunakan dalam kelas [PageTableArea](../../com.groupdocs.parser.data/pagetablearea).

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-) | Menginisialisasi instance baru dari kelas [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
|  | [PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)](#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-) | Menginisialisasi instance baru dari kelas [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRowIndex()](#getRowIndex--) | Mendapatkan indeks baris. |
|
|  | [getColumnIndex()](#getColumnIndex--) | Mendapatkan indeks kolom. |
|
|  | [getRowSpan()](#getRowSpan--) | Mendapatkan total jumlah baris yang berisi sel tabel. |
|
|  | [getColumnSpan()](#getColumnSpan--) | Mendapatkan total jumlah kolom yang berisi sel tabel. |
|
|  | [getPageArea()](#getPageArea--) | Mendapatkan nilai sel tabel. |
|
|  | [getText()](#getText--) | Mendapatkan nilai teks sel tabel. |
|
### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea)
```


Menginisialisasi instance baru dari kelas [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rowIndex | int | Indeks berbasis nol dari baris. |
|
|  | columnIndex | int | Indeks berbasis nol dari kolom. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Nilai sel tabel. |
|

### PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan) {#PageTableAreaCell-int-int-com.groupdocs.parser.data.PageArea-int-int-}
```
public PageTableAreaCell(int rowIndex, int columnIndex, PageArea pageArea, int rowSpan, int columnSpan)
```


Menginisialisasi instance baru dari kelas [PageTableAreaCell](../../com.groupdocs.parser.data/pagetableareacell).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rowIndex | int | Indeks berbasis nol dari baris. |
|
|  | columnIndex | int | Indeks berbasis nol dari kolom. |
|
|  | pageArea | [PageArea](../../com.groupdocs.parser.data/pagearea) | Nilai sel tabel. |
|
|  | rowSpan | int | Total jumlah baris yang berisi sel tabel. |
|
|  | columnSpan | int | Total jumlah kolom yang berisi sel tabel. |
|

### getRowIndex() {#getRowIndex--}
```
public int getRowIndex()
```


Mendapatkan indeks baris.


**Returns:**
int - Indeks berbasis nol dari baris pertama yang berisi sel tabel.

### getColumnIndex() {#getColumnIndex--}
```
public int getColumnIndex()
```


Mendapatkan indeks kolom.


**Returns:**
int - Indeks berbasis nol dari kolom pertama yang berisi sel tabel.

### getRowSpan() {#getRowSpan--}
```
public int getRowSpan()
```


Mendapatkan total jumlah baris yang berisi sel tabel.


**Returns:**
int - Nilai integer positif yang mewakili total jumlah baris yang berisi sel tabel.

### getColumnSpan() {#getColumnSpan--}
```
public int getColumnSpan()
```


Mendapatkan total jumlah kolom yang berisi sel tabel.


**Returns:**
int - Nilai integer positif yang mewakili total jumlah kolom yang berisi sel tabel.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Mendapatkan nilai sel tabel.


**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - Depending on cell [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain any of the inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class.

### getText() {#getText--}
```
public String getText()
```


Mendapatkan nilai teks sel tabel.


**Returns:**
java.lang.String - Sebuah string yang mewakili nilai teks dari sel; null jika sel tidak berisi nilai teks.

