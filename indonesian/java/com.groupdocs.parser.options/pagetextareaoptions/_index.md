---
title: "PageTextAreaOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk ekstraksi area teks halaman."
type: docs
weight: 32
url: /id/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Menyediakan opsi yang digunakan untuk ekstraksi area teks halaman.

Sebuah instance dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) digunakan sebagai parameter dalam [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
dan metode [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-). Lihat contoh penggunaan di sana.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan nilai default. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) dengan opsi penggunaan OCR. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) dengan kemampuan untuk mengatur opsi OCR. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan ekspresi reguler. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan ekspresi reguler dan area persegi panjang. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan ekspresi reguler, area persegi panjang, dan ukuran batas yang diabaikan. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions). |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan ukuran batas yang diabaikan. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getExpression()](#getExpression--) | Mendapatkan ekspresi reguler. |
|
|  | [isMatchCase()](#isMatchCase--) | Mendapatkan nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Mendapatkan nilai yang menunjukkan apakah segmen digabungkan. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Mendapatkan nilai yang menunjukkan apakah pemformatan teks diabaikan. |
|
|  | [isUseOcr()](#isUseOcr--) | Mendapatkan nilai yang menunjukkan apakah OCR Connector digunakan untuk mengekstrak teks. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Mendapatkan opsi tambahan untuk fungsionalitas OCR. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan nilai default.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) dengan opsi penggunaan OCR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | useOcr | boolean | Nilai yang menunjukkan apakah fungsionalitas OCR digunakan untuk mengekstrak teks. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) dengan kemampuan untuk mengatur opsi OCR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | useOcr | boolean | Nilai yang menunjukkan apakah fungsionalitas OCR digunakan untuk mengekstrak teks. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Opsi tambahan untuk fungsionalitas OCR. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan ekspresi reguler. Opsi lain diatur ke nilai default (lihat catatan untuk detail).

Properti berikut memiliki nilai default:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | expression | java.lang.String | Ekspresi reguler. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan ekspresi reguler dan area persegi panjang. Opsi lain diatur ke nilai default (lihat catatan untuk detail).

Properti berikut memiliki nilai default:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | expression | java.lang.String | Ekspresi reguler. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi area halaman. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan ekspresi reguler, area persegi panjang, dan ukuran batas yang diabaikan. Opsi lain diatur ke nilai default (lihat catatan untuk detail).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | expression | java.lang.String | Ekspresi reguler. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi area halaman. |
|
|  | rectangleTolerance | double | Ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. Diukur dengan fraksi tinggi item teks. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | expression | java.lang.String | Ekspresi reguler. |
|
|  | matchCase | boolean | Nilai yang menunjukkan apakah huruf teks tidak diabaikan. |
|
|  | uniteSegments | boolean | Nilai yang menunjukkan apakah segmen digabungkan. |
|
|  | ignoreFormatting | boolean | Nilai yang menunjukkan apakah format teks diabaikan. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi area halaman. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Menginisialisasi sebuah instance baru dari kelas [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) dengan ukuran batas yang diabaikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | expression | java.lang.String | Ekspresi reguler. |
|
|  | matchCase | boolean | Nilai yang menunjukkan apakah huruf teks tidak diabaikan. |
|
|  | uniteSegments | boolean | Nilai yang menunjukkan apakah segmen digabungkan. |
|
|  | ignoreFormatting | boolean | Nilai yang menunjukkan apakah format teks diabaikan. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi area halaman. |
|
|  | rectangleTolerance | double | Ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. Diukur dengan fraksi tinggi item teks. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Mendapatkan ekspresi reguler.


**Returns:**
java.lang.String - Sebuah string yang merepresentasikan ekspresi reguler.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Mendapatkan nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan.


**Returns:**
boolean -  true  jika huruf teks tidak diabaikan; jika tidak,  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Mendapatkan nilai yang menunjukkan apakah segmen digabungkan.


**Returns:**
boolean - {code true} jika segmen digabungkan; jika tidak, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Mendapatkan nilai yang menunjukkan apakah pemformatan teks diabaikan.


**Returns:**
boolean -  true  jika format teks diabaikan; jika tidak,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Mendapatkan nilai yang menunjukkan apakah OCR Connector digunakan untuk mengekstrak teks.


**Returns:**
boolean -  true  jika fungsionalitas OCR digunakan; jika tidak,  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Mendapatkan opsi tambahan untuk fungsionalitas OCR.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

