---
title: "TemplateLinkedPosition"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan posisi bidang templat yang menggunakan bidang yang ditautkan."
type: docs
weight: 15
url: /id/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Menyediakan posisi bidang templat yang menggunakan bidang yang ditautkan.

Contoh berikut menunjukkan kode untuk situasi jika diketahui bahwa bidang dengan nomor faktur
ditempatkan di sebelah kanan string "Invoice number", kode berikut digunakan:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | Menginisialisasi instance baru dari kelas [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | Menginisialisasi instance baru dari kelas [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) dengan nama HURUF BESAR. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | Menginisialisasi instance baru dari kelas [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Mendapatkan nama bidang yang terhubung. |
|
|  | [getSearchArea()](#getSearchArea--) | Mendapatkan ukuran area tempat bidang dicari. |
|
|  | [isAutoScale()](#isAutoScale--) | Mendapatkan nilai yang menunjukkan apakah SearchArea diskalakan oleh ukuran bidang yang terhubung. |
|
|  | [getEdges()](#getEdges--) | Mendapatkan tepi bidang yang terhubung tempat bidang dicari. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


Menginisialisasi instance baru dari kelas [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Nama bidang yang ditautkan. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Ukuran area tempat bidang dicari. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Tepi bidang yang ditautkan tempat bidang dicari. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


Menginisialisasi instance baru dari kelas [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) dengan nama HURUF BESAR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Nama bidang yang ditautkan. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Ukuran area tempat bidang dicari. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Tepi bidang yang ditautkan tempat bidang dicari. |
|
|  | autoScale | boolean | Nilai yang menunjukkan apakah searchArea diskalakan oleh ukuran bidang yang ditautkan. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


Menginisialisasi instance baru dari kelas [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Nama bidang yang ditautkan. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Ukuran area tempat bidang dicari. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Tepi bidang yang ditautkan tempat bidang dicari. |
|
|  | autoScale | boolean | Nilai yang menunjukkan apakah searchArea diskalakan oleh ukuran bidang yang ditautkan.\\ |
|
|  | useUpperCaseName | boolean | Nilai yang menunjukkan apakah sebuah nama dikonversi menjadi HURUF BESAR. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Mendapatkan nama bidang yang terhubung.


**Returns:**
java.lang.String - Nilai string huruf besar yang mewakili nama bidang yang ditautkan.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Mendapatkan ukuran area tempat bidang dicari.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Mendapatkan nilai yang menunjukkan apakah SearchArea diskalakan oleh ukuran bidang yang terhubung.


**Returns:**
java.lang.Boolean - {code true} jika  SearchArea  diskalakan oleh ukuran bidang yang ditautkan; jika tidak,  false .

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Mendapatkan tepi bidang yang terhubung tempat bidang dicari.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Membuat salinan posisi saat ini dengan semua koordinat diskalakan oleh faktor yang diberikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| faktor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
