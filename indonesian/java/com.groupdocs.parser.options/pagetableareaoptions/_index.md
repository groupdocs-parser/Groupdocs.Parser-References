---
title: "PageTableAreaOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk ekstraksi area tabel halaman."
type: docs
weight: 31
url: /id/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Menyediakan opsi yang digunakan untuk ekstraksi area tabel halaman.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Menginisialisasi sebuah instance baru dari kelas [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions). |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi sebuah instance baru dari kelas [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) dengan persegi pencarian dan tanpa tata letak tetap. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Mendapatkan tata letak tabel yang mendefinisikan tabel pada halaman. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Menginisialisasi sebuah instance baru dari kelas [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tata letak tabel yang mendefinisikan tabel pada halaman. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Menginisialisasi sebuah instance baru dari kelas [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) dengan persegi pencarian dan tanpa tata letak tetap.

Berguna untuk membatasi tabel yang terdeteksi otomatis ke wilayah halaman. Mencerminkan C#

new PageTableAreaOptions(null) { Rectangle = ... }
pola.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang pada halaman tempat tabel harus dideteksi; berikan null untuk mencari seluruh halaman. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Mendapatkan tata letak tabel yang mendefinisikan tabel pada halaman.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

