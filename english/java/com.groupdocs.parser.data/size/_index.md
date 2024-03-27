---
title: Size
second_title: GroupDocs.Parser for Java API Reference
description: Represents a size.
type: docs
weight: 28
url: /java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Represents a size.
## Constructors

| Constructor | Description |
| --- | --- |
| [Size(double width, double height)](#Size-double-double-) | Initializes a new instance of the [Size](../../com.groupdocs.parser.data/size) class. |
## Methods

| Method | Description |
| --- | --- |
| [getWidth()](#getWidth--) | Gets the width. |
| [getHeight()](#getHeight--) | Gets the height. |
| [isEmpty()](#isEmpty--) | Gets a value that indicates whether the size is empty. |
| [parse(String s)](#parse-java.lang.String-) | Converts the string representation of a size to its class equivalent. |
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Initializes a new instance of the [Size](../../com.groupdocs.parser.data/size) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| width | double | The width in pixels. |
| height | double | The height in pixels. |

### getWidth() {#getWidth--}
```
public double getWidth()
```


Gets the width.

**Returns:**
double - A double value that represents the width in pixels.
### getHeight() {#getHeight--}
```
public double getHeight()
```


Gets the height.

**Returns:**
double - A double value that represents the height in pixels.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Gets a value that indicates whether the size is empty.

**Returns:**
boolean -  true  if the  width  and  height  are zero; otherwise,  false .
### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Converts the string representation of a size to its class equivalent. A return value indicates whether the conversion is succeeded or failed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.lang.String | A string containing a size to convert. |

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
