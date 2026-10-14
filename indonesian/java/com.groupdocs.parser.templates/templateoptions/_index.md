---
title: "TemplateOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk parsing melalui fungsionalitas templat."
type: docs
weight: 17
url: /id/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Menyediakan opsi yang digunakan untuk parsing melalui fungsionalitas templat.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Menginisialisasi sebuah instance baru dari kelas [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Mendapatkan ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Menginisialisasi sebuah instance baru dari kelas [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangleTolerance | double | Ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. Diukur dengan fraksi tinggi item teks. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Mendapatkan ukuran batas yang diabaikan ketika ditangkap oleh area persegi panjang. Diukur dengan fraksi tinggi item teks.


**Returns:**
double - Nilai double dari 0 (tanpa batas) hingga 1 (abaikan seluruh elemen).

