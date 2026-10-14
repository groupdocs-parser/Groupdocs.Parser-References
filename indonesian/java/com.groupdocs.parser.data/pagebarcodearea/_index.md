---
title: "PageBarcodeArea"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili area barcode halaman yang digunakan untuk mewakili nilai barcode dalam fungsi parsing dengan templat."
type: docs
weight: 18
url: /id/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Mewakili area barcode halaman yang digunakan untuk mewakili nilai barcode dalam fungsi parsing dengan templat.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi sebuah instance baru dari kelas [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getValue()](#getValue--) | Mendapatkan nilai barcode. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Mendapatkan nama tipe barcode. |
|
|  | [getConfidence()](#getConfidence--) | Mendapatkan tingkat kepercayaan barcode yang diparsing. |
|
|  | [getAngle()](#getAngle--) | Mendapatkan sudut barcode. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Menginisialisasi sebuah instance baru dari kelas [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Nilai barcode. |
|
|  | codeTypeName | java.lang.String | Nama tipe barcode. |
|
|  | confidence | int | Tingkat kepercayaan barcode yang diparsing. |
|
|  | angle | double | Sudut barcode. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Halaman yang berisi area barcode. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang berisi area barcode. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Mendapatkan nilai barcode.


**Returns:**
java.lang.String - Nilai string yang mewakili nilai area halaman barcode.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Mendapatkan nama tipe barcode.


**Returns:**
java.lang.String - Nilai string yang mewakili nama tipe barcode.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Mendapatkan tingkat kepercayaan barcode yang diparsing.


**Returns:**
int - Nilai integer yang mewakili tingkat kepercayaan barcode yang diparsing (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


Mendapatkan sudut barcode.


**Returns:**
double - Nilai integer yang mewakili sudut barcode (0-360).

