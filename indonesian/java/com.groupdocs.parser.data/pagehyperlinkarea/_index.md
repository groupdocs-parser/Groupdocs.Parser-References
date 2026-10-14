---
title: "PageHyperlinkArea"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili area halaman yang digunakan untuk mewakili hyperlink pada halaman."
type: docs
weight: 20
url: /id/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Mewakili area halaman yang digunakan untuk mewakili hyperlink pada halaman.

Sebuah instance dari kelas [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) digunakan sebagai nilai kembali dari metode berikut:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Lihat contoh penggunaan di sana.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi sebuah instance baru dari kelas [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getText()](#getText--) | Mendapatkan teks hyperlink. |
|
|  | [getUrl()](#getUrl--) | Mendapatkan URL hyperlink. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Menginisialisasi sebuah instance baru dari kelas [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | teks | java.lang.String | Teks hyperlink. |
|
|  | url | java.lang.String | URL hyperlink. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Halaman yang berisi hyperlink. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi hyperlink. |
|

### getText() {#getText--}
```
public String getText()
```


Mendapatkan teks hyperlink.


**Returns:**
java.lang.String - Nilai string yang mewakili teks hyperlink.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Mendapatkan URL hyperlink.


**Returns:**
java.lang.String - Nilai string yang mewakili URL hyperlink.

