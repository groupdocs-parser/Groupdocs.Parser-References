---
title: "OcrOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk OCR Connector."
type: docs
weight: 27
url: /id/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Menyediakan opsi yang digunakan untuk OCR Connector.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan nilai default. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan area persegi panjang. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan opsi pratinjau halaman. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan objek [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan area persegi panjang dan objek [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Mendapatkan area persegi panjang yang membatasi area halaman yang digunakan untuk pengenalan teks. |
|
|  | [getHandler()](#getHandler--) | Mendapatkan penangan peristiwa untuk menangkap peristiwa OCR. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Mendapatkan nilai yang menunjukkan apakah pemeriksa ejaan digunakan. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | Mendapatkan opsi pratinjau halaman yang digunakan untuk merender halaman yang diberikan ke mesin OCR. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Mengatur opsi pratinjau halaman yang digunakan untuk merender halaman yang diberikan ke mesin OCR. |
|
|  | [getLanguage()](#getLanguage--) | Mendapatkan bahasa yang digunakan untuk pengenalan karakter optik. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Mengatur bahasa yang digunakan untuk pengenalan karakter optik. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Mengatur area persegi panjang yang membatasi area halaman yang digunakan untuk mengenali teks. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Mengatur penangan peristiwa untuk menangkap peristiwa OCR. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Mengatur nilai yang menunjukkan apakah pemeriksa ejaan digunakan. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan nilai default.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan area persegi panjang.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang membatasi area halaman yang digunakan untuk mengenali teks. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan opsi pratinjau halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Opsi yang digunakan untuk merender pratinjau halaman yang diberikan ke mesin OCR. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan objek [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Sebuah instance dari [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) untuk menangkap peristiwa OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions) dengan area persegi panjang dan objek [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang membatasi area halaman yang digunakan untuk mengenali teks. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Sebuah instance dari [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) untuk menangkap peristiwa OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Menginisialisasi instance baru dari kelas [OcrOptions](../../com.groupdocs.parser.options/ocroptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Area persegi panjang yang membatasi area halaman yang digunakan untuk mengenali teks. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Sebuah instance dari [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) untuk menangkap peristiwa OCR. |
|
|  | useSpellCheker | boolean | Nilai yang menunjukkan apakah pemeriksa ejaan digunakan. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Mendapatkan area persegi panjang yang membatasi area halaman yang digunakan untuk pengenalan teks.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Mendapatkan penangan peristiwa untuk menangkap peristiwa OCR.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Mendapatkan nilai yang menunjukkan apakah pemeriksa ejaan digunakan.


**Returns:**
boolean -  true  jika pemeriksa ejaan digunakan; selainnya,  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Mendapatkan opsi pratinjau halaman yang digunakan untuk merender halaman yang diberikan ke mesin OCR.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Mengatur opsi pratinjau halaman yang digunakan untuk merender halaman yang diberikan ke mesin OCR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Opsi pratinjau halaman. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Mendapatkan bahasa yang digunakan untuk pengenalan karakter optik.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Mengatur bahasa yang digunakan untuk pengenalan karakter optik.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | Nilai enum [Language](../../com.groupdocs.parser.options/language). |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Mengatur area persegi panjang yang membatasi area halaman yang digunakan untuk mengenali teks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Persegi panjang, atau  null  untuk memindai seluruh halaman. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Mengatur penangan peristiwa untuk menangkap peristiwa OCR.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Penangan peristiwa. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Mengatur nilai yang menunjukkan apakah pemeriksa ejaan digunakan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  untuk mengaktifkan pemeriksaan ejaan. |
|

