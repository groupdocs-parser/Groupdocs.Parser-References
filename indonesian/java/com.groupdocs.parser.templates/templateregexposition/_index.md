---
title: "TemplateRegexPosition"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan posisi bidang templat yang menggunakan ekspresi reguler."
type: docs
weight: 19
url: /id/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Menyediakan posisi bidang templat yang menggunakan ekspresi reguler.

Contoh berikut menunjukkan situasi jika dokumen berisi \"Invoice Number INV-12345\"
maka bidang templat dapat didefinisikan dengan cara berikut:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

Dalam kasus ini, sebagai nilai seluruh string diekstrak. Untuk mengekstrak hanya sebagian dari string
grup ekspresi reguler \"value\" digunakan:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

Dalam kasus ini, sebagai nilai string \"INV-3337\" diekstrak.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Menginisialisasi instance baru dari kelas [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Menginisialisasi instance baru dari kelas [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getExpression()](#getExpression--) | Mendapatkan ekspresi reguler. |
|
|  | [isMatchCase()](#isMatchCase--) | Mendapatkan nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Menginisialisasi instance baru dari kelas [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | expression | java.lang.String | Ekspresi reguler. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Menginisialisasi instance baru dari kelas [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | expression | java.lang.String | Ekspresi reguler. |
|
|  | matchCase | boolean | Nilai yang menunjukkan apakah huruf teks tidak diabaikan. |
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
