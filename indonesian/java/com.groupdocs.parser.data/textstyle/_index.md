---
title: "TextStyle"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili gaya teks seperti nama font, ukuran font, dan sebagainya."
type: docs
weight: 30
url: /id/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Mewakili gaya teks seperti nama font, ukuran font, dan sebagainya.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Menginisialisasi sebuah instance baru dari kelas [TextStyle](../../com.groupdocs.parser.data/textstyle). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getName()](#getName--) | Mendapatkan nama gaya. |
|
|  | [getFontName()](#getFontName--) | Mendapatkan nama font. |
|
|  | [getFontSize()](#getFontSize--) | Mendapatkan ukuran font. |
|
|  | [isBold()](#isBold--) | Mendapatkan nilai yang menunjukkan apakah font tebal. |
|
|  | [isItalic()](#isItalic--) | Mendapatkan nilai yang menunjukkan apakah font miring. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Menginisialisasi sebuah instance baru dari kelas [TextStyle](../../com.groupdocs.parser.data/textstyle).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nama | java.lang.String | Nama gaya. |
|
|  | fontName | java.lang.String | Nama font. |
|
|  | fontSize | double | Ukuran font. |
|
|  | bold | boolean | Nilai yang menunjukkan apakah font tebal. |
|
|  | italic | boolean | Nilai yang menunjukkan apakah font miring. |
|

### getName() {#getName--}
```
public String getName()
```


Mendapatkan nama gaya.


**Returns:**
java.lang.String - Nilai string yang mewakili nama gaya.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Mendapatkan nama font.


**Returns:**
java.lang.String - Nilai string yang mewakili nama font.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Mendapatkan ukuran font.


**Returns:**
double - Nilai double yang mewakili ukuran font.

### isBold() {#isBold--}
```
public boolean isBold()
```


Mendapatkan nilai yang menunjukkan apakah font tebal.


**Returns:**
boolean -  true  jika font tebal; jika tidak,  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Mendapatkan nilai yang menunjukkan apakah font miring.


**Returns:**
boolean -  true  jika font miring; jika tidak,  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
