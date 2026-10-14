---
title: "OcrEventHandler"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan handler untuk peristiwa OCR."
type: docs
weight: 26
url: /id/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Menyediakan handler untuk peristiwa OCR.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Menginisialisasi instance baru dari kelas [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Mendapatkan daftar pesan peringatan. |
|
|  | [hasWarnings()](#hasWarnings--) | Mendapatkan nilai yang menunjukkan apakah daftar peringatan tidak kosong. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Mengembalikan daftar pesan peringatan untuk halaman dengan pageIndex. |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Mengatur pesan peringatan untuk halaman. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Menginisialisasi instance baru dari kelas [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Mendapatkan daftar pesan peringatan.


**Returns:**
java.util.List<java.lang.String> - Daftar pesan peringatan untuk semua halaman.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Mendapatkan nilai yang menunjukkan apakah daftar peringatan tidak kosong.


**Returns:**
boolean -  true  jika daftar peringatan tidak kosong; jika tidak,  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Mengembalikan daftar pesan peringatan untuk halaman dengan pageIndex.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

**Returns:**
java.util.List<java.lang.String> - Daftar pesan peringatan untuk halaman; daftar kosong jika tidak ada pesan peringatan untuk halaman.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Mengatur pesan peringatan untuk halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageIndex | int | Indeks halaman berbasis nol. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | Daftar pesan peringatan untuk halaman. |
|

