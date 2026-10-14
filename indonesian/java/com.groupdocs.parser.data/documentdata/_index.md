---
title: "DocumentData"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili data dokumen."
type: docs
weight: 11
url: /id/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Mewakili data dokumen. Ini terdiri dari objek [FieldData](../../com.groupdocs.parser.data/fielddata) yang berisi data bidang dari dokumen. Sebuah instance dari kelas [DocumentData](../../com.groupdocs.parser.data/documentdata) digunakan sebagai nilai kembali dari metode [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) dan [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) . Lihat contoh penggunaan di sana.

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Mendapatkan templat yang menghasilkan data dokumen ini. |
|
|  | [getCount()](#getCount--) | Mendapatkan total jumlah data bidang. |
|
|  | [get(int index)](#get-int-) | Mendapatkan data bidang berdasarkan indeks. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Mengembalikan koleksi data bidang dimana namanya sama dengan  fieldName . |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator atas elemen dalam daftar ini dalam urutan yang tepat. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Mendapatkan templat yang menghasilkan data dokumen ini.

Ketika data dihasilkan oleh pemilihan koleksi templat otomatis (lihat
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
ini adalah templat yang dipilih.
null
ketika data tidak dihasilkan oleh templat.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Mendapatkan total jumlah data bidang.


**Returns:**
int - Nilai integer yang mewakili total jumlah data bidang.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Mendapatkan data bidang berdasarkan indeks.

Iterasi melalui semua bidang:

````
// Print all extracted data
 for (int i = 0; i < data.getCount(); i++) {
     // Print field name
     System.out.print(data.get(i).getName() + ": ");
     // As we have defined only text fields in the template,
     // we cast PageArea property value to PageTextArea
     PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
             ? (PageTextArea) data.get(i).getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field PageArea property can contain any
dari turunan kelas [PageArea](../../com.groupdocs.parser.data/pagearea). Misalnya, metode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) mengekstrak hanya bidang teks:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleFormsPdf)) {
     // Extract data from PDF document
     DocumentData data = parser.parseForm();
     // Check if form extraction is supported
     if (data == null) {
         System.out.println("Form extraction isn't supported.");
         return;
     }
     // Iterate over extracted data
     for (int i = 0; i < data.getCount(); i++) {
         System.out.print(data.get(i).getName() + ": ");
         PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
                 ? (PageTextArea) data.get(i).getPageArea()
                 : null;
         System.out.println(area == null ? "Not a template field" : area.getText());
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indeks | int | Indeks berbasis nol dari bidang. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Mengembalikan koleksi data bidang dimana namanya sama dengan  fieldName .

Temukan bidang berdasarkan nama bidang:

````
// Print prices
 System.out.println("Prices:");
 for (FieldData field : data.getFieldsByName("Price")) {
     PageTextArea area = field.getPageArea() instanceof PageTextArea
             ? (PageTextArea) field.getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain
apapun turunan kelas [PageArea](../../com.groupdocs.parser.data/pagearea). Misalnya, metode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) mengekstrak hanya bidang teks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fieldName | java.lang.String | Nama bidang. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - Sekumpulan objek [FieldData](../../com.groupdocs.parser.data/fielddata); koleksi kosong jika tidak ada data bidang yang ditemukan.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Mengembalikan iterator atas elemen dalam daftar ini dalam urutan yang tepat.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - iterator atas elemen dalam daftar ini dalam urutan yang tepat.

