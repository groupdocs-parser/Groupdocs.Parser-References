---
title: "TextStyle"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Metnin stilini, örneğin bir yazı tipi adı, bir yazı tipi boyutu vb. temsil eder."
type: docs
weight: 30
url: /tr/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Yazı tipi adı, yazı tipi boyutu vb. gibi metnin stilini temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Yeni bir [TextStyle](../../com.groupdocs.parser.data/textstyle) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getName()](#getName--) | Stil adını alır. |
|
|  | [getFontName()](#getFontName--) | Yazı tipi adını alır. |
|
|  | [getFontSize()](#getFontSize--) | Yazı tipi boyutunu alır. |
|
|  | [isBold()](#isBold--) | Yazı tipinin kalın olup olmadığını gösteren değeri alır. |
|
|  | [isItalic()](#isItalic--) | Yazı tipinin italik olup olmadığını gösteren değeri alır. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Yeni bir [TextStyle](../../com.groupdocs.parser.data/textstyle) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ad | java.lang.String | Stil adı. |
|
|  | fontName | java.lang.String | Yazı tipi adı. |
|
|  | fontSize | double | Yazı tipi boyutu. |
|
|  | bold | boolean | Yazı tipinin kalın olup olmadığını gösteren değer. |
|
|  | italic | boolean | Yazı tipinin italik olup olmadığını gösteren değer. |
|

### getName() {#getName--}
```
public String getName()
```


Stil adını alır.


**Returns:**
java.lang.String - Stil adını temsil eden bir dize değeri.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Yazı tipi adını alır.


**Returns:**
java.lang.String - Yazı tipi adını temsil eden bir dize değeri.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Yazı tipi boyutunu alır.


**Returns:**
double - Yazı tipi boyutunu temsil eden bir double değeri.

### isBold() {#isBold--}
```
public boolean isBold()
```


Yazı tipinin kalın olup olmadığını gösteren değeri alır.


**Returns:**
boolean -  true  ise yazı tipi kalındır; aksi takdirde  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Yazı tipinin italik olup olmadığını gösteren değeri alır.


**Returns:**
boolean -  true  ise yazı tipi italiktir; aksi takdirde  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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
