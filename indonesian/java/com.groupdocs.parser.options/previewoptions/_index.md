---
title: "PreviewOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi untuk mengatur persyaratan dan delegasi aliran untuk pembuatan pratinjau."
type: docs
weight: 34
url: /id/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Menyediakan opsi untuk mengatur persyaratan dan delegasi aliran untuk pembuatan pratinjau.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Menginisialisasi instance baru dari kelas [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) yang menyebabkan aliran keluaran ditutup. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Menginisialisasi instance baru dari kelas [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) yang menyebabkan aliran keluaran dikembalikan ke klien untuk penggunaan lebih lanjut. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getWidth()](#getWidth--) | Mendapatkan lebar pratinjau halaman. |
|
|  | [setWidth(int width)](#setWidth-int-) | Mengatur lebar pratinjau halaman. |
|
|  | [getHeight()](#getHeight--) | Mendapatkan tinggi pratinjau halaman. |
|
|  | [setHeight(int height)](#setHeight-int-) | Mengatur tinggi pratinjau halaman. |
|
|  | [getDpi()](#getDpi--) | Mendapatkan dpi. |
|
|  | [setDpi(int dpi)](#setDpi-int-) | Mengatur dpi. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Mendapatkan array nomor halaman untuk menghasilkan pratinjau. |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Mengatur array nomor halaman untuk menghasilkan pratinjau. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Mendapatkan format gambar pratinjau. |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Mengatur format gambar pratinjau. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Mendapatkan instance delegasi pembuatan aliran halaman. |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Mengatur instance delegasi pembuatan aliran halaman. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Mendapatkan instance delegasi penyelesaian pratinjau halaman. |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Mengatur instance delegasi penyelesaian pratinjau halaman. |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | Mendapatkan instance delegasi informasi render pratinjau halaman. |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Mengatur instance delegasi informasi render pratinjau halaman. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Menginisialisasi instance baru dari kelas [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) yang menyebabkan aliran keluaran ditutup.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Membuat aliran untuk pratinjau halaman tertentu. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Menginisialisasi instance baru dari kelas [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) yang menyebabkan aliran keluaran dikembalikan ke klien untuk penggunaan lebih lanjut.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Membuat aliran untuk pratinjau halaman tertentu |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Memberitahu bahwa pembuatan pratinjau halaman selesai dan mendapatkan aliran keluaran. |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


Mendapatkan lebar pratinjau halaman.


**Returns:**
int - Lebar halaman.

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Mengatur lebar pratinjau halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lebar | int | Lebar halaman. |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


Mendapatkan tinggi pratinjau halaman.


**Returns:**
int - Tinggi halaman.

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Mengatur tinggi pratinjau halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | tinggi | int | Tinggi halaman. |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


Mendapatkan dpi.


**Returns:**
int - Nilai integer yang mewakili dpi.

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Mengatur dpi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dpi | int | Dpi. |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Mendapatkan array nomor halaman untuk menghasilkan pratinjau.


**Returns:**
int[] - Koleksi nomor halaman.

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Mengatur array nomor halaman untuk menghasilkan pratinjau.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pageNumbers | int[] | Koleksi nomor halaman. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Mendapatkan format gambar pratinjau.


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Mengatur format gambar pratinjau.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | Format pratinjau. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Mendapatkan instance delegasi pembuatan aliran halaman.


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Mengatur instance delegasi pembuatan aliran halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Delegate pembuatan aliran halaman. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Mendapatkan instance delegasi penyelesaian pratinjau halaman.


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Mengatur instance delegasi penyelesaian pratinjau halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Delegate penyelesaian pratinjau halaman. |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Mendapatkan instance delegasi informasi render pratinjau halaman.


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Mengatur instance delegasi informasi render pratinjau halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | Delegate informasi render pratinjau halaman. |
|

