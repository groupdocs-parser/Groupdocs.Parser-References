---
title: "DocumentInfo"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili informasi dokumen."
type: docs
weight: 11
url: /id/java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Mewakili informasi dokumen.

**Learn more:**

* [Get document info](../https://docs.groupdocs.com/display/parserjava/Get+document+info)
* [Detect encoding](../https://docs.groupdocs.com/display/parserjava/Detect+encoding)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFileType()](#getFileType--) | Mendapatkan tipe dokumen. |
|
|  | [getPageCount()](#getPageCount--) | Mendapatkan total jumlah halaman dokumen. |
|
|  | [getRawPageCount()](#getRawPageCount--) | Mendapatkan total jumlah halaman mentah dokumen. |
|
|  | [getSize()](#getSize--) | Mendapatkan ukuran dokumen dalam byte. |
|
|  | [getPages()](#getPages--) | Mendapatkan informasi tentang halaman seperti indeks dan ukuran halaman. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Mendapatkan tipe dokumen.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.

### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Mendapatkan total jumlah halaman dokumen.


**Returns:**
int - Nilai integer yang mewakili total jumlah halaman.

### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Mendapatkan total jumlah halaman mentah dokumen.

Gunakan properti [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo#getRawPageCount--) sebagai pengganti properti [getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) untuk ekstraksi teks mentah.
Beberapa dokumen memiliki nomor halaman yang berbeda dalam mode ekstraksi teks akurat dan mentah.
[getPageCount()](../../com.groupdocs.parser.options/documentinfo#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.


**Returns:**
int - Nilai integer yang mewakili total jumlah halaman mentah.

### getSize() {#getSize--}
```
public abstract long getSize()
```


Mendapatkan ukuran dokumen dalam byte.


**Returns:**
long - Nilai integer yang mewakili ukuran dokumen dalam byte.

### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Mendapatkan informasi tentang halaman seperti indeks dan ukuran halaman.


**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - Koleksi dengan instance kelas [PageInfo](../../com.groupdocs.parser.options/pageinfo).

