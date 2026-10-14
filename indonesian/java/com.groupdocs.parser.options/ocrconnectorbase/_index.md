---
title: "OcrConnectorBase"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan fungsionalitas OCR."
type: docs
weight: 25
url: /id/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Menyediakan fungsionalitas OCR.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Menginisialisasi sebuah instance baru dari kelas [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi teks didukung. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi area teks didukung. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Kenali teks dari aliran  imageStream  stream. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Kenali area teks dari aliran  imageStream  stream. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Menginisialisasi sebuah instance baru dari kelas [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase).


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi teks didukung.


**Returns:**
boolean -  true  jika ekstraksi teks didukung; lainnya,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi area teks didukung.


**Returns:**
boolean -  true  jika ekstraksi area teks didukung; lainnya,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


Kenali teks dari aliran  imageStream  stream.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Representasi gambar dari halaman dokumen. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Opsi OCR. |
|

**Returns:**
java.lang.String - Sebuah string yang mewakili teks yang dikenali;  null  jika pengenalan teks tidak didukung.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Kenali area teks dari aliran  imageStream  stream.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Representasi gambar dari halaman dokumen. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | Ukuran halaman dokumen. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Opsi OCR. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Sekumpulan objek [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  jika pengenalan area teks tidak didukung.

