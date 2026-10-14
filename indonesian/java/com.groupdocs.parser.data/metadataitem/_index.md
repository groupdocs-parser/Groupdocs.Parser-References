---
title: "MetadataItem"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili item metadata yang digunakan dalam item kontainer dan fungsi ekstraksi metadata."
type: docs
weight: 15
url: /id/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Mewakili item metadata yang digunakan dalam item kontainer dan fungsi ekstraksi metadata.

Sebuah instansi kelas [MetadataItem](../../com.groupdocs.parser.data/metadataitem) digunakan sebagai nilai kembali dari metode [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--).
dan sebagai item dalam koleksi [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--). Lihat contoh penggunaan di sana.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | Menginisialisasi sebuah instansi baru dari kelas [MetadataItem](../../com.groupdocs.parser.data/metadataitem). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getName()](#getName--) | Mendapatkan nama item metadata. |
|
|  | [getValue()](#getValue--) | Mendapatkan nilai item metadata. |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


Menginisialisasi sebuah instansi baru dari kelas [MetadataItem](../../com.groupdocs.parser.data/metadataitem).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nama | java.lang.String | Nama item metadata. |
|
|  | nilai | java.lang.String | Nilai item metadata. |
|

### getName() {#getName--}
```
public String getName()
```


Mendapatkan nama item metadata.


**Returns:**
java.lang.String - Nilai string yang mewakili nama item metadata.

### getValue() {#getValue--}
```
public String getValue()
```


Mendapatkan nilai item metadata.


**Returns:**
java.lang.String - Nilai string yang mewakili nilai item metadata.

