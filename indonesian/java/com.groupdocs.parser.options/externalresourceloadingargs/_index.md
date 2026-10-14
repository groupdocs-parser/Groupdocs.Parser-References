---
title: "ExternalResourceLoadingArgs"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan data untuk metode."
type: docs
weight: 17
url: /id/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Menyediakan data untuk metode [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-).

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Menginisialisasi instance baru dari kelas [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) dengan area persegi panjang. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getUri()](#getUri--) | Mendapatkan URI dari sumber daya eksternal. |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | Mendapatkan URI dari sumber daya eksternal. |
|
|  | [isSkipped()](#isSkipped--) | Mendapatkan nilai yang menunjukkan apakah pemuatan sumber daya eksternal harus dilewati. |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | Mengatur nilai yang menunjukkan apakah pemuatan sumber daya eksternal harus dilewati. |
|
|  | [getData()](#getData--) | Mendapatkan data pengguna. |
|
|  | [setData(byte[] data)](#setData-byte---) | Mengatur data pengguna. |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Menginisialisasi instance baru dari kelas [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) dengan area persegi panjang.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | uri | java.lang.String | URI dari sumber daya eksternal. |
|

### getUri() {#getUri--}
```
public String getUri()
```


Mendapatkan URI dari sumber daya eksternal.


**Returns:**
java.lang.String - Nilai string yang mewakili URI dari sumber daya eksternal.

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Mendapatkan URI dari sumber daya eksternal.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | uri | java.lang.String | Nilai string yang mewakili URI baru dari sumber daya eksternal. |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Mendapatkan nilai yang menunjukkan apakah pemuatan sumber daya eksternal harus dilewati.


**Returns:**
boolean - true jika pemuatan sumber daya eksternal harus dilewati; jika tidak, false.

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Mengatur nilai yang menunjukkan apakah pemuatan sumber daya eksternal harus dilewati.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dilewati | boolean | true jika pemuatan sumber daya eksternal harus dilewati; jika tidak, false. |
|

### getData() {#getData--}
```
public byte[] getData()
```


Mendapatkan data pengguna.


**Returns:**
byte[] - Array byte dengan konten pengguna dari sumber daya eksternal. null jika tidak disetel.

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Mengatur data pengguna.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | byte[] | Array byte dengan konten pengguna dari sumber eksternal. null jika tidak diatur. |
|

