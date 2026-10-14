---
title: "FieldData"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili data bidang seperti nama, indeks halaman, nilai bidang, dan sebagainya."
type: docs
weight: 13
url: /id/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Mewakili data bidang seperti nama, indeks halaman, nilai bidang, dan sebagainya. Tergantung pada bidang, nilai dapat berupa teks, gambar, tabel, dan sebagainya.

Instansi kelas [FieldData](../../com.groupdocs.parser.data/fielddata) digunakan dalam koleksi [DocumentData](../../com.groupdocs.parser.data/documentdata).

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getName()](#getName--) | Mendapatkan nama bidang. |
|
|  | [getPageIndex()](#getPageIndex--) | Mendapatkan indeks halaman. |
|
|  | [getPageArea()](#getPageArea--) | Mendapatkan nilai bidang. |
|
|  | [getLinkedField()](#getLinkedField--) | Mendapatkan bidang yang ditautkan. |
|
|  | [getText()](#getText--) | Mendapatkan teks. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Mendapatkan nilai yang menunjukkan apakah  Name  telah diubah menjadi UPPER CASE. |
|
### getName() {#getName--}
```
public String getName()
```


Mendapatkan nama bidang.


**Returns:**
java.lang.String - Nilai string huruf besar yang mewakili nama bidang.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Mendapatkan indeks halaman.


**Returns:**
int - Indeks berbasis nol dari halaman yang berisi bidang.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Mendapatkan nilai bidang.

Tergantung pada bidang, properti PageArea dapat berisi salah satu turunan dari kelas [PageArea](../../com.groupdocs.parser.data/pagearea).
Sebagai contoh, metode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) mengekstrak hanya bidang teks.

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


Mendapatkan bidang yang ditautkan.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Mendapatkan teks.


**Returns:**
java.lang.String - Nilai string yang mewakili nilai teks bidang; null jika properti [PageArea](../../com.groupdocs.parser.data/pagearea) bukan [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Mendapatkan nilai yang menunjukkan apakah  Name  telah diubah menjadi UPPER CASE.


**Returns:**
boolean - Nilai boolean yang menunjukkan apakah  Name  telah diubah menjadi UPPER CASE.

