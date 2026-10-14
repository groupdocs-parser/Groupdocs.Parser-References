---
title: "SearchResult"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili hasil pencarian dalam fungsi pencarian."
type: docs
weight: 27
url: /id/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Mewakili hasil pencarian dalam fungsi pencarian.

Sebuah instance dari kelas SearchResult digunakan sebagai nilai kembali dari [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-)
dan metode [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-). Lihat contoh penggunaan di sana.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Menginisialisasi sebuah instance baru dari kelas [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Menginisialisasi sebuah instance baru dari kelas [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getPosition()](#getPosition--) | Mendapatkan posisi dalam teks dokumen. |
|
|  | [getText()](#getText--) | Mendapatkan teks. |
|
|  | [getPageIndex()](#getPageIndex--) | Mendapatkan indeks halaman tempat teks ditemukan. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Mendapatkan sorotan kiri. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Mendapatkan sorotan kanan. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Menginisialisasi sebuah instance baru dari kelas [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | posisi | int | Posisi dalam teks dokumen. |
|
|  | teks | java.lang.String | Teks yang ditemukan. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat teks ditemukan. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Sorotan kiri. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Sorotan kanan. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Menginisialisasi sebuah instance baru dari kelas [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | posisi | int | Posisi dalam teks dokumen. |
|
|  | teks | java.lang.String | Teks yang ditemukan. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman tempat teks ditemukan. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Mendapatkan posisi dalam teks dokumen.


**Returns:**
int - Indeks berbasis nol dari posisi awal hasil pencarian.

### getText() {#getText--}
```
public String getText()
```


Mendapatkan teks.


**Returns:**
java.lang.String - Nilai string yang mewakili teks yang ditemukan.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Mendapatkan indeks halaman tempat teks ditemukan.


**Returns:**
java.lang.Integer - Indeks berbasis nol dari halaman tempat teks ditemukan; null jika pencarian dilakukan pada seluruh teks dokumen.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Mendapatkan sorotan kiri.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Mendapatkan sorotan kanan.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

