---
title: "PageGroupArea"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili grup area halaman yang digunakan untuk mengelompokkan berbagai jenis blok pada halaman dokumen dalam fungsi parsing dengan templat."
type: docs
weight: 19
url: /id/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Mewakili grup area halaman yang digunakan untuk mengelompokkan berbagai jenis blok pada halaman dokumen dalam fungsi parsing dengan templat.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Menginisialisasi instance baru dari kelas [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getAreas()](#getAreas--) | Mendapatkan koleksi area halaman yang dikelompokkan. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Menginisialisasi instance baru dari kelas [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | Koleksi area halaman yang akan dikelompokkan. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Halaman yang berisi area tersebut. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Mendapatkan koleksi area halaman yang dikelompokkan.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - Sebuah koleksi objek [PageArea](../../com.groupdocs.parser.data/pagearea).

