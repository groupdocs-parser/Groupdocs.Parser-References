---
title: Point
second_title: GroupDocs.Parser for Java API Reference
description: Represents a point.
type: docs
weight: 25
url: /java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Represents a point.
## Constructors

| Constructor | Description |
| --- | --- |
| [Point(double x, double y)](#Point-double-double-) | Initializes a new instance of the [Point](../../com.groupdocs.parser.data/point) class. |
## Methods

| Method | Description |
| --- | --- |
| [getX()](#getX--) | Gets the x-coordinate. |
| [getY()](#getY--) | Gets the y-coordinate. |
| [parse(String s)](#parse-java.lang.String-) | Converts the string representation of a point to its class equivalent. |
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Initializes a new instance of the [Point](../../com.groupdocs.parser.data/point) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| x | double | The x-coordinate. |
| y | double | The y-coordinate. |

### getX() {#getX--}
```
public double getX()
```


Gets the x-coordinate.

**Returns:**
double - A double value that represents the x-coordinate.
### getY() {#getY--}
```
public double getY()
```


Gets the y-coordinate.

**Returns:**
double - A double value that represents the y-coordinate.
### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Converts the string representation of a point to its class equivalent. A return value indicates whether the conversion is succeeded or failed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.lang.String | A string containing a point to convert. |

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
