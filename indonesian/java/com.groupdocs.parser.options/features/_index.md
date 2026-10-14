---
title: "Fitur"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili daftar fitur yang didukung."
type: docs
weight: 18
url: /id/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Mewakili daftar fitur yang didukung. Memungkinkan memperoleh informasi fitur mana yang didukung atau tidak untuk dokumen.

Sebuah instance dari kelas ini digunakan sebagai properti [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--). Lihat contoh penggunaan di sana.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Features()](#Features--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Mengembalikan nilai yang menunjukkan apakah fitur didukung. |
|
|  | [isText()](#isText--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi teks didukung. |
|
|  | [isTextPage()](#isTextPage--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi halaman teks didukung. |
|
|  | [isFormattedText()](#isFormattedText--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi teks terformat didukung. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi halaman teks terformat didukung. |
|
|  | [isSearch()](#isSearch--) | Mendapatkan nilai yang menunjukkan apakah pencarian teks didukung. |
|
|  | [isHighlight()](#isHighlight--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi sorotan didukung. |
|
|  | [isBarcodes()](#isBarcodes--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi kode batang didukung. |
|
|  | [isToc()](#isToc--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi daftar isi didukung. |
|
|  | [isMetadata()](#isMetadata--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi metadata didukung. |
|
|  | [isContainer()](#isContainer--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi kontainer didukung. |
|
|  | [isTextAreas()](#isTextAreas--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi area teks didukung. |
|
|  | [isStructure()](#isStructure--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi struktur teks didukung. |
|
|  | [isImages()](#isImages--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi gambar didukung. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi tautan hiperlink didukung. |
|
|  | [isTables()](#isTables--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi tabel didukung. |
|
|  | [isAnnotations()](#isAnnotations--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi anotasi didukung. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Mendapatkan nilai yang menunjukkan apakah parsing dengan templat didukung. |
|
|  | [isParseForm()](#isParseForm--) | Mendapatkan nilai yang menunjukkan apakah parsing formulir didukung. |
|
|  | [isPreview()](#isPreview--) | Mendapatkan nilai yang menunjukkan apakah pembuatan pratinjau didukung. |
|
|  | [isPagePreview()](#isPagePreview--) | Mendapatkan nilai yang menunjukkan apakah pembuatan pratinjau halaman didukung. |
|
|  | [isOcr()](#isOcr--) | Mendapatkan nilai yang menunjukkan apakah fungsionalitas OCR didukung. |
|
|  | [isWorksheet()](#isWorksheet--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi lembar kerja didukung. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Mengembalikan nilai yang menunjukkan apakah fitur didukung.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | featureName | java.lang.String | Nama fitur. |
|

**Returns:**
boolean -  true  jika fitur didukung; jika tidak,  false .

### isText() {#isText--}
```
public boolean isText()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi teks didukung.


**Returns:**
boolean -  true  jika ekstraksi teks didukung; jika tidak,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi halaman teks didukung.


**Returns:**
boolean -  true  jika ekstraksi halaman teks didukung; jika tidak,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi teks terformat didukung.


**Returns:**
boolean -  true  jika ekstraksi teks terformat didukung; jika tidak,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi halaman teks terformat didukung.


**Returns:**
boolean -  true  jika halaman teks terformat didukung; jika tidak,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Mendapatkan nilai yang menunjukkan apakah pencarian teks didukung.


**Returns:**
boolean -  true  jika pencarian teks didukung; jika tidak,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi sorotan didukung.


**Returns:**
boolean -  true  jika ekstraksi sorotan didukung; jika tidak,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi kode batang didukung.


**Returns:**
boolean -  true  jika ekstraksi kode batang didukung; jika tidak,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi daftar isi didukung.


**Returns:**
boolean -  true  jika ekstraksi daftar isi didukung; jika tidak,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi metadata didukung.


**Returns:**
boolean -  true  jika ekstraksi metadata didukung; jika tidak,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi kontainer didukung.


**Returns:**
boolean -  true  jika ekstraksi kontainer didukung; jika tidak,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi area teks didukung.


**Returns:**
boolean -  true  jika ekstraksi area teks didukung; jika tidak,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi struktur teks didukung.


**Returns:**
boolean -  true  jika ekstraksi struktur teks didukung; jika tidak,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi gambar didukung.


**Returns:**
boolean -  true  jika ekstraksi gambar didukung; jika tidak,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi tautan hiperlink didukung.


**Returns:**
boolean -  true  jika ekstraksi hyperlink didukung; jika tidak,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi tabel didukung.


**Returns:**
boolean -  true  jika ekstraksi tabel didukung; jika tidak,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi anotasi didukung.


**Returns:**
boolean -  true  jika ekstraksi anotasi didukung; jika tidak,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Mendapatkan nilai yang menunjukkan apakah parsing dengan templat didukung.


**Returns:**
boolean -  true  jika parsing berdasarkan templat didukung; jika tidak,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Mendapatkan nilai yang menunjukkan apakah parsing formulir didukung.


**Returns:**
boolean -  true  jika parsing formulir didukung; jika tidak,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Mendapatkan nilai yang menunjukkan apakah pembuatan pratinjau didukung.


**Returns:**
boolean -  true  jika pembuatan pratinjau didukung; jika tidak,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Mendapatkan nilai yang menunjukkan apakah pembuatan pratinjau halaman didukung.


**Returns:**
boolean -  true  jika pembuatan pratinjau halaman didukung; jika tidak,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Mendapatkan nilai yang menunjukkan apakah fungsionalitas OCR didukung.


**Returns:**
boolean -  true  jika fungsi OCR didukung; jika tidak,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi lembar kerja didukung.


**Returns:**
boolean -  true  jika ekstraksi lembar kerja didukung; jika tidak,  false .

