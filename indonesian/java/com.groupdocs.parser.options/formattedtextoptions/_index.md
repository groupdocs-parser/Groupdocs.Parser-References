---
title: "FormattedTextOptions"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan opsi yang digunakan untuk ekstraksi teks terformat."
type: docs
weight: 21
url: /id/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Menyediakan opsi yang digunakan untuk ekstraksi teks terformat.

Sebuah instance dari kelas [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) digunakan sebagai parameter dalam [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-)
dan metode [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-). Lihat contoh penggunaan di sana.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Menginisialisasi sebuah instance baru dari kelas [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) tanpa mode yang ditetapkan. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Menginisialisasi instance baru dari kelas [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getMode()](#getMode--) | Mendapatkan mode ekstraksi teks terformat. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Mengatur mode ekstraksi teks terformat. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Menginisialisasi sebuah instance baru dari kelas [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) tanpa mode yang ditetapkan.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Menginisialisasi instance baru dari kelas [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Mode ekstraksi teks terformat. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Mendapatkan mode ekstraksi teks terformat.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Mengatur mode ekstraksi teks terformat.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Enumerasi [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) yang berisi mode ekstraksi teks terformat. |
|

