---
title: "PageTextArea"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili area teks halaman yang digunakan untuk mewakili nilai teks dalam fungsi parsing dengan templat atau parsing formulir."
type: docs
weight: 24
url: /id/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Mewakili area teks halaman yang digunakan untuk mewakili nilai teks dalam fungsi parsing dengan templat atau parsing formulir.

Sebuah instance dari kelas [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) digunakan sebagai nilai kembali dari metode berikut:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

Juga sebuah instance dari kelas [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) digunakan sebagai nilai properti [PageArea](../../com.groupdocs.parser.data/pagearea).
\*

Lihat contoh penggunaan di sana.

Area teks dapat berupa tunggal atau komposit. Pada kasus pertama, ia berisi teks yang dibatasi oleh area persegi panjang.
Pada kasus kedua, ia berisi area teks lain; properti teks dan tabel dihitung oleh area teks anak.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi sebuah instance baru dari kelas [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi sebuah instance baru dari kelas [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Menginisialisasi sebuah instance baru dari kelas [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getText()](#getText--) | Mendapatkan teks. |
|
|  | [getBaseLine()](#getBaseLine--) | Mendapatkan garis dasar. |
|
|  | [getTextStyle()](#getTextStyle--) | Mendapatkan gaya teks seperti ukuran font, nama font, dan seterusnya. |
|
|  | [getAreas()](#getAreas--) | Mendapatkan koleksi area halaman teks anak. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Menginisialisasi sebuah instance baru dari kelas [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | teks | java.lang.String | Nilai teks. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Halaman yang berisi area teks. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi area teks. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Menginisialisasi sebuah instance baru dari kelas [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | teks | java.lang.String | Nilai teks. |
|
|  | baseLine | java.lang.Double | Garis dasar teks. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | Gaya teks. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Halaman yang berisi area teks. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi area teks. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Menginisialisasi sebuah instance baru dari kelas [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Koleksi area halaman teks anak. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Halaman yang berisi area teks. |
|

### getText() {#getText--}
```
public String getText()
```


Mendapatkan teks.


**Returns:**
java.lang.String - Nilai string yang mewakili nilai area halaman teks.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Mendapatkan garis dasar.


**Returns:**
double - Nilai double yang mewakili garis dasar.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Mendapatkan gaya teks seperti ukuran font, nama font, dan seterusnya.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Mendapatkan koleksi area halaman teks anak.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - Koleksi area halaman teks anak; kosong jika area halaman teks tidak memiliki anak.

