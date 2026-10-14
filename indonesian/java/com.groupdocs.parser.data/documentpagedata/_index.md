---
title: "DocumentPageData"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili data halaman dokumen."
type: docs
weight: 12
url: /id/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Mewakili data halaman dokumen. Ini terdiri dari objek [FieldData](../../com.groupdocs.parser.data/fielddata) yang berisi data bidang dari halaman dokumen.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Menginisialisasi sebuah instance baru dari kelas [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Mendapatkan indeks halaman. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Menginisialisasi sebuah instance baru dari kelas [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fields | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | Koleksi data bidang. |
|
|  | pageIndex | int | Indeks halaman berbasis nol. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Mendapatkan indeks halaman.


**Returns:**
int - Indeks halaman berbasis nol.

