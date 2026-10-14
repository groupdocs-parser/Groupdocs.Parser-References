---
title: "Lisensi"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili lisensi GroupDocs.Parser."
type: docs
weight: 10
url: /id/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Mewakili lisensi GroupDocs.Parser.

Contoh ini menunjukkan cara menyiapkan lisensi.

````
 ```

// Inisialisasi kelas Lisensi
License license = new License();
// Atur jalur ke file .lic
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [License()](#License--) | Menginisialisasi instance baru dari kelas [License](../../com.groupdocs.parser.licensing/license) class. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Memberi lisensi pada komponen. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Memberi lisensi pada komponen. |
|
### License() {#License--}
```
public License()
```


Menginisialisasi instance baru dari kelas [License](../../com.groupdocs.parser.licensing/license) class.


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Memberi lisensi pada komponen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur absolut ke file lisensi. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Memberi lisensi pada komponen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | stream | java.io.InputStream | Aliran lisensi. |
|

