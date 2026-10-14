---
title: "PageArea"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili kelas dasar abstrak untuk area halaman yang digunakan untuk mewakili blok pada halaman dokumen dalam fungsi parsing dengan templat."
type: docs
weight: 17
url: /id/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Mewakili kelas dasar abstrak untuk area halaman yang digunakan untuk mewakili blok pada halaman dokumen dalam fungsi parsing dengan templat.

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Mendapatkan area persegi panjang. |
|
|  | [getPage()](#getPage--) | Mendapatkan informasi halaman dokumen seperti indeks halaman dan ukuran halaman. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Mendapatkan area persegi panjang.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Mendapatkan informasi halaman dokumen seperti indeks halaman dan ukuran halaman.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

