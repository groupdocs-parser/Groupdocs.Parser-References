---
title: "PageAreaOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk ekstraksi area halaman."
type: docs
weight: 28
url: /id/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Menyediakan opsi yang digunakan untuk ekstraksi area halaman.

Suatu instance dari kelas [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) digunakan sebagai parameter dalam [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
dan metode [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-). Lihat contoh penggunaan di sana.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi instance baru dari kelas [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) dengan ukuran batas yang diabaikan. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Menginisialisasi instance baru dari kelas [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Mendapatkan area persegi panjang yang berisi area halaman. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Mendapatkan ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Menginisialisasi instance baru dari kelas [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) dengan ukuran batas yang diabaikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi area halaman. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Menginisialisasi instance baru dari kelas [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi area halaman. |
|
|  | rectangleTolerance | double | Ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. Diukur dengan fraksi tinggi item teks. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Mendapatkan area persegi panjang yang berisi area halaman.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Mendapatkan ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. Diukur dengan fraksi tinggi item teks.


**Returns:**
double - Nilai double dari 0 (tanpa batas) hingga 1 (abaikan seluruh elemen).

