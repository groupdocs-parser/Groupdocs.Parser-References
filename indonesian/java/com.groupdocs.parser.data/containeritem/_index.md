---
title: "ContainerItem"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili item kontainer seperti entitas arsip Zip, lampiran email, item Portfolio PDF, dan sebagainya."
type: docs
weight: 10
url: /id/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Mewakili item kontainer seperti entitas arsip Zip, lampiran email, item PDF Portfolio, dan sebagainya.

Sebuah instance dari kelas [ContainerItem](../../com.groupdocs.parser.data/containeritem) digunakan sebagai nilai kembali dari metode [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--) . Lihat contoh penggunaan di sana.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Menginisialisasi sebuah instance baru dari [ContainerItem](../../com.groupdocs.parser.data/containeritem) dengan nama item dan direktori. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Menginisialisasi sebuah instance baru dari [ContainerItem](../../com.groupdocs.parser.data/containeritem) dengan jalur lengkap item. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getName()](#getName--) | Mendapatkan nama item. |
|
|  | [getDirectory()](#getDirectory--) | Mendapatkan direktori item. |
|
|  | [getFilePath()](#getFilePath--) | Mendapatkan jalur lengkap item. |
|
|  | [getSize()](#getSize--) | Mendapatkan ukuran item. |
|
|  | [getMetadata()](#getMetadata--) | Mendapatkan koleksi item metadata. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Mendapatkan nilai metadata. |
|
|  | [openStream()](#openStream--) | Membuka aliran konten item. |
|
|  | [openParser()](#openParser--) | Membuat objek [Parser](../../com.groupdocs.parser/parser) untuk konten item. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Membuat objek [Parser](../../com.groupdocs.parser/parser) untuk konten item dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Membuat objek [Parser](../../com.groupdocs.parser/parser) untuk konten item dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dan [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Mendeteksi tipe file dari item kontainer. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Menginisialisasi sebuah instance baru dari [ContainerItem](../../com.groupdocs.parser.data/containeritem) dengan nama item dan direktori.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nama | java.lang.String | Nama item. |
|
|  | direktori | java.lang.String | Direktori item. |
|
|  | size | long | Ukuran item. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Koleksi item metadata. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Menginisialisasi sebuah instance baru dari [ContainerItem](../../com.groupdocs.parser.data/containeritem) dengan jalur lengkap item.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur lengkap item. |
|
|  | size | long | Ukuran item. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Koleksi item metadata. |
|

### getName() {#getName--}
```
public String getName()
```


Mendapatkan nama item.


**Returns:**
java.lang.String - Nilai string yang mewakili nama file dari item (tanpa direktori).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Mendapatkan direktori item.


**Returns:**
java.lang.String - Nilai string yang mewakili direktori dari item (tanpa nama file).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Mendapatkan jalur lengkap item.


**Returns:**
java.lang.String - Nilai string yang mewakili jalur lengkap dari item.

### getSize() {#getSize--}
```
public long getSize()
```


Mendapatkan ukuran item.


**Returns:**
long - Nilai integer yang mewakili ukuran item dalam byte.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Mendapatkan koleksi item metadata.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Sekumpulan objek [MetadataItem](../../com.groupdocs.parser.data/metadataitem); kosong jika metadata tidak diatur.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Mendapatkan nilai metadata.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nama | java.lang.String | Nama metadata. |
|

**Returns:**
java.lang.String - Nilai string yang mewakili nilai item metadata; null jika metadata dengan nama ini tidak ditemukan.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Membuka aliran konten item.


**Returns:**
java.io.InputStream - Aliran dengan konten item.

### openParser() {#openParser--}
```
public Parser openParser()
```


Membuat objek [Parser](../../com.groupdocs.parser/parser) untuk konten item.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Membuat objek [Parser](../../com.groupdocs.parser/parser) untuk konten item dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Opsi untuk membuka konten item. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Membuat objek [Parser](../../com.groupdocs.parser/parser) untuk konten item dengan [LoadOptions](../../com.groupdocs.parser.options/loadoptions) dan [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Opsi untuk membuka konten item. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Mendeteksi tipe file dari item kontainer.


detectionMode
parameter memberikan kemampuan untuk mengontrol deteksi tipe file:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

Contoh berikut menunjukkan cara mendeteksi tipe file dari item kontainer:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Extract attachments from the container
     Iterable attachments = parser.getContainer();
     // Check if container extraction is supported
     if (attachments == null) {
         System.out.println("Container extraction isn't supported");
     }
     // Iterate over attachments
     for (ContainerItem item : attachments) {
         // Detect the file type
         FileType fileType = item.detectFileType(FileTypeDetectionMode.Default);
         // Print the name and file type
         System.out.println(String.format("%s: %s", item.getName(), fileType));
     }
 }
 
````



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Mendefinisikan mode deteksi tipe file. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

