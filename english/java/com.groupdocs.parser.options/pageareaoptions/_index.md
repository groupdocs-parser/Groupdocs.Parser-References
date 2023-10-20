---
title: PageAreaOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for page areas extraction.
type: docs
weight: 27
url: /java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Provides the options which are used for page areas extraction.

An instance of [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) class is used as parameter in [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser\#getImages-PageAreaOptions-) and [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser\#getImages-int--PageAreaOptions-) methods. See the usage examples there.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) class with the size of the ignored border. |
| [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Initializes a new instance of the [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRectangle()](#getRectangle--) | Gets the rectangular area that contains page areas. |
| [getRectangleTolerance()](#getRectangleTolerance--) | Gets the size of the border that is ignored when captured by the rectangular area. |
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Initializes a new instance of the [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) class with the size of the ignored border.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains page areas. |

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Initializes a new instance of the [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains page areas. |
| rectangleTolerance | double | The size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gets the rectangular area that contains page areas.

**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.
### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Gets the size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height.

**Returns:**
double - The double value from 0 (no border) to 1 (ignore the whole element).
