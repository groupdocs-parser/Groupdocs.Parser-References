---
title: "HighlightOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk mengekstrak sorotan blok teks di sekitar teks yang ditemukan dalam skenario pencarian."
type: docs
weight: 22
url: /id/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Menyediakan opsi yang digunakan untuk mengekstrak sorotan (sebuah blok teks di sekitar teks yang ditemukan dalam skenario pencarian).

Sebuah instance dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) digunakan sebagai parameter dalam metode [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-).
Lihat contoh penggunaan di sana.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) tanpa batas yang ditetapkan. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) yang digunakan untuk mengekstrak sorotan dengan panjang tetap. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) yang digunakan untuk mengekstrak sorotan terbatas baris. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) yang digunakan untuk mengekstrak sorotan dengan jumlah kata tetap. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Mendapatkan panjang teks maksimum. |
|
|  | [getWordCount()](#getWordCount--) | Mendapatkan jumlah kata maksimum. |
|
|  | [isLineLimited()](#isLineLimited--) | Mendapatkan nilai yang menunjukkan apakah ekstraksi sorotan dibatasi oleh awal (atau akhir) baris teks. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Mengatur panjang teks maksimum. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Mengatur jumlah kata maksimum. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Mengatur nilai yang menunjukkan apakah ekstraksi sorotan dibatasi oleh awal (atau akhir) baris teks. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) tanpa batas yang ditetapkan. Atur setidaknya satu dari #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) sebelum mengirimkannya ke parser.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) yang digunakan untuk mengekstrak sorotan dengan panjang tetap.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | maxLength | int | Panjang teks maksimum. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) yang digunakan untuk mengekstrak sorotan terbatas baris.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Panjang teks maksimum. |
|
|  | isLineLimited | boolean | Nilai yang menunjukkan apakah ekstraksi sorotan dibatasi oleh awal (atau akhir) baris teks. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) yang digunakan untuk mengekstrak sorotan dengan jumlah kata tetap.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Panjang teks maksimum. |
|
|  | wordCount | int | Jumlah kata maksimum. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Menginisialisasi sebuah instance baru dari kelas [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Panjang teks maksimum. |
|
|  | wordCount | java.lang.Integer | Jumlah kata maksimum. |
|
|  | isLineLimited | boolean | Nilai yang menunjukkan apakah ekstraksi sorotan dibatasi oleh awal (atau akhir) baris teks. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Mendapatkan panjang teks maksimum.


**Returns:**
java.lang.Integer - Nilai integer positif yang mewakili panjang teks maksimum;  null  jika panjang teks tidak dibatasi.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Mendapatkan jumlah kata maksimum.


**Returns:**
java.lang.Integer - Nilai integer positif yang mewakili jumlah kata maksimum;  null  jika jumlah kata tidak dibatasi.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Mendapatkan nilai yang menunjukkan apakah ekstraksi sorotan dibatasi oleh awal (atau akhir) baris teks.


**Returns:**
boolean -  true  jika ekstraksi sorotan dibatasi oleh awal (atau akhir) baris teks; jika tidak,  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Mengatur panjang teks maksimum.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Integer non-negatif;  null  untuk menghapus batas panjang. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Mengatur jumlah kata maksimum.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Integer non-negatif;  null  untuk menghapus batas jumlah kata. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Mengatur nilai yang menunjukkan apakah ekstraksi sorotan dibatasi oleh awal (atau akhir) baris teks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lineLimited | boolean | true  untuk membatasi berdasarkan batas baris. |
|

