---
title: "SearchOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk pencarian teks."
type: docs
weight: 35
url: /id/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Menyediakan opsi yang digunakan untuk pencarian teks.

Sebuah instance dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) digunakan sebagai parameter dalam metode [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-).
Lihat contoh penggunaan di sana.

**Learn more:**

* [Search text](../https://docs.groupdocs.com/display/parserjava/Search+text)
* [Search text in Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents)
* [Search text in Emails](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails)
* [Search text in EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) yang digunakan untuk pencarian dengan opsi penyorotan untuk ekstraksi penyorotan kiri dan kanan. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) yang digunakan untuk pencarian dengan opsi penyorotan yang sama untuk ekstraksi penyorotan kiri dan kanan. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) yang digunakan untuk pencarian tanpa ekstraksi penyorotan. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) yang digunakan untuk pencarian berdasarkan halaman dan tanpa ekstraksi penyorotan. |
|
|  | [SearchOptions()](#SearchOptions--) | Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) dengan nilai default. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Mendapatkan nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Mendapatkan nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Mendapatkan nilai yang menunjukkan apakah ekspresi reguler digunakan. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Mendapatkan nilai yang menunjukkan apakah pencarian dilakukan per halaman. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Mendapatkan opsi untuk penyorotan kiri. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Mendapatkan opsi untuk penyorotan kanan. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Mendapatkan nilai yang mewakili indeks maksimum halaman yang akan dicari. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | matchCase | boolean | Nilai yang menunjukkan apakah huruf teks tidak diabaikan. |
|
|  | matchWholeWord | boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
|
|  | useRegularExpression | boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
|
|  | searchByPages | boolean | Nilai yang menunjukkan apakah pencarian dilakukan per halaman. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Opsi untuk penyorotan kiri. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Opsi untuk penyorotan kanan. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | matchCase | boolean | Nilai yang menunjukkan apakah huruf teks tidak diabaikan. |
|
|  | matchWholeWord | boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
|
|  | useRegularExpression | boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
|
|  | maxPageIndex | int | Nilai yang mewakili indeks maksimum halaman yang akan dicari |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Opsi untuk penyorotan kiri. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Opsi untuk penyorotan kanan. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) yang digunakan untuk pencarian dengan opsi penyorotan untuk ekstraksi penyorotan kiri dan kanan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | matchCase | boolean | Nilai yang menunjukkan apakah huruf teks tidak diabaikan. |
|
|  | matchWholeWord | boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
|
|  | useRegularExpression | boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Opsi untuk penyorotan kiri. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Opsi untuk penyorotan kanan. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) yang digunakan untuk pencarian dengan opsi penyorotan yang sama untuk ekstraksi penyorotan kiri dan kanan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | matchCase | boolean | Nilai yang menunjukkan apakah huruf teks tidak diabaikan. |
|
|  | matchWholeWord | boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
|
|  | useRegularExpression | boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Opsi untuk kedua penyorotan. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) yang digunakan untuk pencarian tanpa ekstraksi penyorotan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | matchCase | boolean | Nilai yang menunjukkan apakah huruf teks tidak diabaikan. |
|
|  | matchWholeWord | boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
|
|  | useRegularExpression | boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) yang digunakan untuk pencarian berdasarkan halaman dan tanpa ekstraksi penyorotan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | matchCase | boolean | Nilai yang menunjukkan apakah huruf teks tidak diabaikan. |
|
|  | matchWholeWord | boolean | Nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap. |
|
|  | useRegularExpression | boolean | Nilai yang menunjukkan apakah ekspresi reguler digunakan. |
|
|  | searchByPages | boolean | Nilai yang menunjukkan apakah pencarian dilakukan per halaman. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Menginisialisasi instance baru dari kelas [SearchOptions](../../com.groupdocs.parser.options/searchoptions) dengan nilai default. Lihat catatan untuk detail.

Properti berikut memiliki nilai default:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Mendapatkan nilai yang menunjukkan apakah kapitalisasi teks tidak diabaikan.


**Returns:**
boolean -  true  jika huruf teks tidak diabaikan; jika tidak,  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Mendapatkan nilai yang menunjukkan apakah pencarian teks dibatasi oleh kata lengkap.


**Returns:**
boolean -  true  jika pencarian teks dibatasi oleh kata lengkap; jika tidak,  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Mendapatkan nilai yang menunjukkan apakah ekspresi reguler digunakan.


**Returns:**
boolean -  true  jika ekspresi reguler digunakan; jika tidak,  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Mendapatkan nilai yang menunjukkan apakah pencarian dilakukan per halaman.


**Returns:**
boolean -  true  jika pencarian dilakukan per halaman; jika tidak,  false  dan pencarian dilakukan pada seluruh dokumen tanpa menyertakan nilai properti [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) dalam kelas [SearchResult](../../com.groupdocs.parser.data/searchresult).

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Mendapatkan opsi untuk penyorotan kiri.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Mendapatkan opsi untuk penyorotan kanan.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Mendapatkan nilai yang mewakili indeks maksimum halaman yang akan dicari.


**Returns:**
int - Nilai integer yang mewakili indeks maksimum halaman yang akan dicari; -1 jika tidak diatur;

