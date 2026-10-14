---
title: "TextOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk ekstraksi teks."
type: docs
weight: 37
url: /id/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Menyediakan opsi yang digunakan untuk ekstraksi teks.

Sebuah instance dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) digunakan sebagai parameter dalam [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-)
dan metode [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) . Lihat contoh penggunaan di sana.

Ini digunakan untuk menentukan mode mentah ekstraksi teks. Sebuah teks dalam mode ini diekstrak secara tidak akurat
tetapi lebih cepat dibandingkan mode standar. Jika mode mentah tidak mendukung format dokumen,
maka parameter ini diabaikan dan mode standar digunakan.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) . |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) dengan opsi penggunaan OCR. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) dengan kemampuan untuk mengatur opsi OCR. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Mendapatkan nilai yang menunjukkan apakah mode mentah digunakan. |
|
|  | [isUseOcr()](#isUseOcr--) | Mendapatkan nilai yang menunjukkan apakah OCR Connector digunakan untuk mengekstrak teks. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Mendapatkan opsi tambahan untuk fungsionalitas OCR. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Mendapatkan nilai yang menunjukkan apakah anotasi termasuk dalam teks yang diekstrak. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Mengatur nilai yang menunjukkan apakah anotasi termasuk dalam teks yang diekstrak. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Nilai yang menunjukkan apakah mode mentah digunakan. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) dengan opsi penggunaan OCR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Nilai yang menunjukkan apakah mode mentah digunakan. |
|
|  | useOcr | boolean | Nilai yang menunjukkan apakah fungsionalitas OCR digunakan untuk mengekstrak teks. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Menginisialisasi sebuah instance baru dari kelas [TextOptions](../../com.groupdocs.parser.options/textoptions) dengan kemampuan untuk mengatur opsi OCR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | Nilai yang menunjukkan apakah mode mentah digunakan. |
|
|  | useOcr | boolean | Nilai yang menunjukkan apakah fungsionalitas OCR digunakan untuk mengekstrak teks. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Opsi tambahan untuk fungsionalitas OCR. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Mendapatkan nilai yang menunjukkan apakah mode mentah digunakan.


**Returns:**
boolean -  true  jika mode mentah digunakan; jika tidak,  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Mendapatkan nilai yang menunjukkan apakah anotasi termasuk dalam teks yang diekstrak. Nilai default adalah  false .


**Returns:**
boolean -  true  jika anotasi termasuk; jika tidak,  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Mengatur nilai yang menunjukkan apakah anotasi termasuk dalam teks yang diekstrak.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  untuk menyertakan anotasi dalam teks yang diekstrak. |
|

