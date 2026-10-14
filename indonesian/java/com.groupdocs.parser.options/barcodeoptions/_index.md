---
title: "BarcodeOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk ekstraksi kode batang."
type: docs
weight: 10
url: /id/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Menyediakan opsi yang digunakan untuk ekstraksi kode batang.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | Menginisialisasi instance baru dari kelas BarcodeOptions dengan nilai default. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi instance baru dari kelas BarcodeOptions dengan area persegi panjang. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Menginisialisasi instance baru dari kelas BarcodeOptions dengan pengaturan kualitas dan tipe kode. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Menginisialisasi instance baru dari kelas BarcodeOptions. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Mendapatkan nilai yang menunjukkan apakah barcode yang tidak tepat diizinkan. |
|
|  | [getDimension()](#getDimension--) | Mendapatkan ukuran minimal dari elemen barcode minimal. |
|
|  | [getImageQuality()](#getImageQuality--) | Mendapatkan kualitas gambar sumber. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Mendapatkan kualitas barcode sumber. |
|
|  | [getRectangle()](#getRectangle--) | Mendapatkan area persegi panjang yang berisi area halaman. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Mendapatkan tipe barcode yang akan dibaca. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Mengatur nilai yang menunjukkan apakah barcode yang tidak tepat diizinkan. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Mengatur ukuran minimal dari elemen barcode minimal. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Mengatur kualitas gambar sumber. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Mengatur kualitas barcode sumber. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Mengatur area persegi panjang yang berisi barcode. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Mengatur tipe barcode yang akan dibaca. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Menginisialisasi instance baru dari kelas BarcodeOptions dengan nilai default.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Menginisialisasi instance baru dari kelas BarcodeOptions dengan area persegi panjang.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi barcode. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Menginisialisasi instance baru dari kelas BarcodeOptions dengan pengaturan kualitas dan tipe kode.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kualitas gambar sumber. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kualitas barcode sumber. |
|
|  | codeTypes | java.lang.String[] | Jenis-jenis barcode yang akan dibaca. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Menginisialisasi instance baru dari kelas BarcodeOptions.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi barcode. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kualitas gambar sumber. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kualitas barcode sumber. |
|
|  | dimension | java.lang.Float | Ukuran minimal elemen minimal barcode. |
|
|  | allowIncorrectBarcodes | boolean | Nilai yang menunjukkan apakah barcode yang tidak benar diizinkan. |
|
|  | codeTypes | java.lang.String[] | Jenis-jenis barcode yang akan dibaca. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Mendapatkan nilai yang menunjukkan apakah barcode yang tidak tepat diizinkan.


**Returns:**
boolean -  true  jika barcode yang tidak benar diizinkan; jika tidak,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Mendapatkan ukuran minimal dari elemen barcode minimal.


**Returns:**
java.lang.Float - Nilai float yang mewakili elemen minimal barcode;  null  jika mode otomatis digunakan.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Mendapatkan kualitas gambar sumber.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Mendapatkan kualitas barcode sumber.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Mendapatkan area persegi panjang yang berisi area halaman.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Mendapatkan tipe barcode yang akan dibaca.


**Returns:**
java.util.List<java.lang.String> - Koleksi hanya-baca yang berisi jenis-jenis barcode untuk dibaca; koleksi kosong jika tidak disetel.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Mengatur nilai yang menunjukkan apakah barcode yang tidak tepat diizinkan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  jika barcode yang tidak benar diizinkan. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Mengatur ukuran minimal dari elemen barcode minimal.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dimension | java.lang.Float | Elemen minimal barcode;  null  untuk mode otomatis. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Mengatur kualitas gambar sumber.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Mode kualitas gambar. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Mengatur kualitas barcode sumber.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Mode kualitas barcode. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Mengatur area persegi panjang yang berisi barcode.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang;  null  untuk memindai seluruh halaman. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Mengatur tipe barcode yang akan dibaca.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | Jenis-jenis barcode;  null  atau kosong untuk semua jenis. |
|

