---
title: Rectangle
second_title: GroupDocs.Parser for Java API Reference
description: Represents a rectangular area.
type: docs
weight: 25
url: /java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Represents a rectangular area.
## Constructors

| Constructor | Description |
| --- | --- |
| [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Initializes a new instance of the [Rectangle](../../com.groupdocs.parser.data/rectangle) class. |
| [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Initializes a new instance of the [Rectangle](../../com.groupdocs.parser.data/rectangle) class. |
## Methods

| Method | Description |
| --- | --- |
| [getLeft()](#getLeft--) | Gets the x-coordinate of the left edge of the rectangular area. |
| [getTop()](#getTop--) | Gets the y-coordinate of the top edge of the rectangular area. |
| [getRight()](#getRight--) | Gets the x-coordinate of the right egde of the rectangular area. |
| [getBottom()](#getBottom--) | Gets the y-coordinate of the bottom edge of the rectangular area. |
| [getPosition()](#getPosition--) | Gets the coordinates of the upper-left corner of the rectangular area. |
| [getSize()](#getSize--) | Gets the size. |
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Initializes a new instance of the [Rectangle](../../com.groupdocs.parser.data/rectangle) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| left | double | The x-coordinate of the left edge of the rectangular area. |
| top | double | The y-coordinate of the top edge of the rectangular area. |
| right | double | The x-coordinate of the right edge of the rectangular area. |
| bottom | double | The y-coordinate of the bottom edge of the rectangular area. |

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Initializes a new instance of the [Rectangle](../../com.groupdocs.parser.data/rectangle) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| position | [Point](../../com.groupdocs.parser.data/point) | The coordinates of the upper-left corner of the rectangular area. |
| size | [Size](../../com.groupdocs.parser.data/size) | The size of the rectangular area. |

### getLeft() {#getLeft--}
```
public double getLeft()
```


Gets the x-coordinate of the left edge of the rectangular area.

**Returns:**
double - A double value that represents the x-coordinate of the left edge of the rectangular area.
### getTop() {#getTop--}
```
public double getTop()
```


Gets the y-coordinate of the top edge of the rectangular area.

**Returns:**
double - A double value that represents the y-coordinate of the top edge of the rectangular area.
### getRight() {#getRight--}
```
public double getRight()
```


Gets the x-coordinate of the right egde of the rectangular area.

**Returns:**
double - A double value that represents the x-coordinate of the right edge of the rectangular area.
### getBottom() {#getBottom--}
```
public double getBottom()
```


Gets the y-coordinate of the bottom edge of the rectangular area.

**Returns:**
double - A double value that represents the y-coordinate of the bottom edge of the rectangular area.
### getPosition() {#getPosition--}
```
public Point getPosition()
```


Gets the coordinates of the upper-left corner of the rectangular area.

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.
### getSize() {#getSize--}
```
public Size getSize()
```


Gets the size.

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
