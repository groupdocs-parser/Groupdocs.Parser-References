---
title: "HighlightItem"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili penyorotan bagian teks yang biasanya digunakan untuk menjelaskan konteks teks yang ditemukan dalam fungsi pencarian."
type: docs
weight: 14
url: /id/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Mewakili penyorotan, bagian teks yang biasanya digunakan untuk menjelaskan konteks teks yang ditemukan dalam fungsi pencarian.

Sebuah instance dari kelas [HighlightItem](../../com.groupdocs.parser.data/highlightitem) digunakan sebagai nilai kembali dari metode [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-),
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [HighlightItem](../../com.groupdocs.parser.data/highlightitem). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getPosition()](#getPosition--) | Mendapatkan posisi dalam teks dokumen. |
|
|  | [getText()](#getText--) | Mendapatkan teks sorotan. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Menginisialisasi sebuah instance baru dari kelas [HighlightItem](../../com.groupdocs.parser.data/highlightitem).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | posisi | int | Posisi dalam teks dokumen. |
|
|  | teks | java.lang.String | Teks sorotan. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Mendapatkan posisi dalam teks dokumen.


**Returns:**
int - Indeks berbasis nol dari posisi awal sorotan.

### getText() {#getText--}
```
public String getText()
```


Mendapatkan teks sorotan.


**Returns:**
java.lang.String - Nilai string yang mewakili teks sorotan.

