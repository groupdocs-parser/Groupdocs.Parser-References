---
title: "TocItem"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili item yang digunakan dalam fungsionalitas ekstraksi daftar isi."
type: docs
weight: 31
url: /id/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Mewakili item yang digunakan dalam fungsionalitas ekstraksi daftar isi.

Sebuah instance dari kelas [TocItem](../../com.groupdocs.parser.data/tocitem) digunakan sebagai nilai kembali dari metode [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) . Lihat contoh penggunaan di sana.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Menginisialisasi sebuah instance baru dari kelas TocItem. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDepth()](#getDepth--) | Mendapatkan tingkat kedalaman. |
|
|  | [getText()](#getText--) | Mendapatkan teks. |
|
|  | [getPageIndex()](#getPageIndex--) | Mendapatkan indeks halaman. |
|
|  | [extractText()](#extractText--) | Mengekstrak teks dari dokumen yang dirujuk oleh objek TocItem. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Menginisialisasi sebuah instance baru dari kelas TocItem.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | depth | int | Tingkat kedalaman item. |
|
|  | teks | java.lang.String | Teks item. |
|
|  | pageIndex | java.lang.Integer | Indeks halaman yang dirujuk oleh item |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Mendapatkan tingkat kedalaman.


**Returns:**
int - Nilai integer yang mewakili tingkat kedalaman item.

### getText() {#getText--}
```
public String getText()
```


Mendapatkan teks.


**Returns:**
java.lang.String - Nilai string yang mewakili teks item.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Mendapatkan indeks halaman.


**Returns:**
java.lang.Integer - Nilai integer yang mewakili indeks halaman yang dirujuk oleh item;  null  jika tidak diatur.

### extractText() {#extractText--}
```
public TextReader extractText()
```


Mengekstrak teks dari dokumen yang dirujuk oleh objek TocItem.

Contoh berikut cara mengekstrak teks menggunakan sebuah item dari daftar isi:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.

