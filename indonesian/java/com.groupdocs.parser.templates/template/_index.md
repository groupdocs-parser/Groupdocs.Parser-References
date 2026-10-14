---
title: "Template"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan templat halaman dokumen."
type: docs
weight: 10
url: /id/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Menyediakan templat halaman dokumen. Templat ini terdiri dari objek [TemplateItem](../../com.groupdocs.parser.templates/templateitem) yang mewakili item templat seperti bidang teks dan definisi tabel.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Menginisialisasi instance baru dari kelas [Template](../../com.groupdocs.parser.templates/template). |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Menginisialisasi instance baru dari kelas [Template](../../com.groupdocs.parser.templates/template). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCount()](#getCount--) | Mendapatkan total jumlah item templat. |
|
|  | [get(int index)](#get-int-) | Mendapatkan item templat berdasarkan indeks. |
|
|  | [getOptions()](#getOptions--) | Mendapatkan opsi templat. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Memuat templat dari file. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Memuat templat dari aliran. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Menyimpan templat ke file. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Menyimpan templat ke aliran. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Menginisialisasi instance baru dari kelas [Template](../../com.groupdocs.parser.templates/template).

Penggunaan:

````
// Create an array of template fields
 TemplateItem[] fields = new TemplateItem[]
 {
     new TemplateField(new TemplateRegexPosition("From"), "From", 0),
     new TemplateField(
         new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromCompany",
         0),
     new TemplateField(
         new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromAddress",
         0)
 };
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(fields));
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Koleksi [TemplateItem](../../com.groupdocs.parser.templates/templateitem) objek. |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Menginisialisasi instance baru dari kelas [Template](../../com.groupdocs.parser.templates/template).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Koleksi [TemplateItem](../../com.groupdocs.parser.templates/templateitem) objek. |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | Opsi templat. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Mendapatkan total jumlah item templat.


**Returns:**
int - Sebuah bilangan bulat yang mewakili total jumlah item templat.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Mendapatkan item templat berdasarkan indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indeks | int | Indeks berbasis nol dari item templat. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Mendapatkan opsi templat.


**Returns:**
[TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) - An instance of [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) class.

### iterator() {#iterator--}
```
public Iterator<TemplateItem> iterator()
```




**Returns:**
java.util.Iterator<com.groupdocs.parser.templates.TemplateItem>
### load(String filePath) {#load-java.lang.String-}
```
public static Template load(String filePath)
```


Memuat templat dari file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Memuat templat dari aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | stream | java.io.InputStream | Aliran masukan. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Menyimpan templat ke file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur ke file. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Menyimpan templat ke aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Aliran output. |
|

