---
title: "TextReader"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Sıralı bir karakter serisini okuyabilen bir okuyucuyu temsil eder."
type: docs
weight: 29
url: /tr/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Sıralı bir karakter serisini okuyabilen bir okuyucuyu temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Metin okuyucudan bir satır karakter okur ve veriyi bir dize olarak döndürür. |
|
|  | [readToEnd()](#readToEnd--) | Mevcut konumdan metin okuyucunun sonuna kadar tüm karakterleri okur ve tek bir dize olarak döndürür. |
|
|  | [dispose()](#dispose--) | [TextReader](../../com.groupdocs.parser.data/textreader) nesnesi tarafından kullanılan tüm kaynakları serbest bırakır. |
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


Metin okuyucudan bir satır karakter okur ve veriyi bir dize olarak döndürür.


**Returns:**
java.lang.String - Okuyucudan bir sonraki satır, veya  null  tüm karakterler okunduysa.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Mevcut konumdan metin okuyucunun sonuna kadar tüm karakterleri okur ve tek bir dize olarak döndürür.


**Returns:**
java.lang.String - Mevcut konumdan metin okuyucunun sonuna kadar tüm karakterleri içeren bir dize.

### dispose() {#dispose--}
```
public void dispose()
```


[TextReader](../../com.groupdocs.parser.data/textreader) nesnesi tarafından kullanılan tüm kaynakları serbest bırakır.


