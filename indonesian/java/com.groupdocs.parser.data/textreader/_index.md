---
title: "TextReader"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Mewakili pembaca yang dapat membaca rangkaian karakter secara berurutan."
type: docs
weight: 29
url: /id/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Mewakili pembaca yang dapat membaca rangkaian karakter secara berurutan.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Membaca satu baris karakter dari text reader dan mengembalikan data sebagai string. |
|
|  | [readToEnd()](#readToEnd--) | Membaca semua karakter dari posisi saat ini hingga akhir text reader dan mengembalikannya sebagai satu string. |
|
|  | [dispose()](#dispose--) | Melepaskan semua sumber daya yang digunakan oleh objek [TextReader](../../com.groupdocs.parser.data/textreader). |
|
### TextReader() {#TextReader--}
```
public TextReader()
```


### markSupported() {#markSupported--}
```
public boolean markSupported()
```




**Returns:**
boolean
### readLine() {#readLine--}
```
public abstract String readLine()
```


Membaca satu baris karakter dari text reader dan mengembalikan data sebagai string.


**Returns:**
java.lang.String - Baris berikutnya dari pembaca, atau  null  jika semua karakter telah dibaca.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Membaca semua karakter dari posisi saat ini hingga akhir text reader dan mengembalikannya sebagai satu string.


**Returns:**
java.lang.String - String yang berisi semua karakter dari posisi saat ini hingga akhir text reader.

### dispose() {#dispose--}
```
public void dispose()
```


Melepaskan semua sumber daya yang digunakan oleh objek [TextReader](../../com.groupdocs.parser.data/textreader).


