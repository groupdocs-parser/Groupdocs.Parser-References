---
title: TextStyle
second_title: GroupDocs.Parser for Java API Reference
description: Represents the style of the text such as a font name a font size and so on.
type: docs
weight: 30
url: /java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Represents the style of the text such as a font name, a font size and so on.
## Constructors

| Constructor | Description |
| --- | --- |
| [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Initializes a new instance of the [TextStyle](../../com.groupdocs.parser.data/textstyle) class. |
## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--) | Gets the style name. |
| [getFontName()](#getFontName--) | Gets the font name. |
| [getFontSize()](#getFontSize--) | Gets the font size. |
| [isBold()](#isBold--) | Gets the value that indicates whether the font is bold. |
| [isItalic()](#isItalic--) | Gets the value that indicates whether the font is italic. |
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Initializes a new instance of the [TextStyle](../../com.groupdocs.parser.data/textstyle) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the style. |
| fontName | java.lang.String | The name of the font. |
| fontSize | double | The size of the font. |
| bold | boolean | The value that indicates whether the font is bold. |
| italic | boolean | The value that indicates whether the font is italic. |

### getName() {#getName--}
```
public String getName()
```


Gets the style name.

**Returns:**
java.lang.String - A string value that represents the style name.
### getFontName() {#getFontName--}
```
public String getFontName()
```


Gets the font name.

**Returns:**
java.lang.String - A string value that represents the font name.
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Gets the font size.

**Returns:**
double - A double value that represents the font size.
### isBold() {#isBold--}
```
public boolean isBold()
```


Gets the value that indicates whether the font is bold.

**Returns:**
boolean -  true  if the font is bold; otherwise,  false .
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Gets the value that indicates whether the font is italic.

**Returns:**
boolean -  true  if the font is italic; otherwise,  false .
### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Parameter | Type | Description |
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
