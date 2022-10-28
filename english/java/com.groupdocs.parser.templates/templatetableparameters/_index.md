---
title: TemplateTableParameters
second_title: GroupDocs.Parser for Java API Reference
description: Provides parameters for the table detection algorithms.
type: docs
weight: 21
url: /java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Provides parameters for the table detection algorithms.

There are two algorithms to detect a table:

 *  Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
 *  Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

In some cases when algorithms can't detect a table or do it in non-accurate way [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class is used.
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Initializes a new instance of the [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. |
| [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Initializes a new instance of the [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRectangle()](#getRectangle--) | Gets the rectangular area that contains the table. |
| [getVerticalSeparators()](#getVerticalSeparators--) | Gets the table columns separators. |
| [hasMergedCells()](#hasMergedCells--) | Gets the value that indicates whether the table has merged cells. |
| [getMinRowCount()](#getMinRowCount--) | Gets the minimum number of the table rows. |
| [getMinColumnCount()](#getMinColumnCount--) | Gets the minimum number of the table columns. |
| [getMinVerticalSpace()](#getMinVerticalSpace--) | Gets the minumum space between the table columns. |
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Initializes a new instance of the [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the table. |
| verticalSeparators | java.lang.Iterable<java.lang.Double> | The table columns separators. |

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Initializes a new instance of the [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the table. |
| verticalSeparators | java.lang.Iterable<java.lang.Double> | The table columns separators. |
| mergedCells | java.lang.Boolean | The value that indicates whether the table has merged cells. |
| minRowCount | java.lang.Integer | The minimum number of the table rows. |
| minColumnCount | java.lang.Integer | The minumum number of the table columns. |
| minVerticalSpace | java.lang.Integer | The minumum space between the table columns. |

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gets the rectangular area that contains the table.

**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.
### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Gets the table columns separators.

**Returns:**
java.util.List<java.lang.Double> - A collection of double values that represent x-coordinates of the table columns separators;  null  if it isn't set.
### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Gets the value that indicates whether the table has merged cells.

**Returns:**
java.lang.Boolean -  true  if the table has merged cells; otherwise,  false .  null  if it isn't set.
### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Gets the minimum number of the table rows.

**Returns:**
java.lang.Integer - An integer value that represents the minimum number of the table rows;  null  if it isn't set.
### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Gets the minimum number of the table columns.

**Returns:**
java.lang.Integer - An integer value that represents the minimum number of the table columns;  null  if it isn't set.
### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Gets the minumum space between the table columns.

**Returns:**
java.lang.Integer - An integer value that represents the minumum space between the table columns;  null  if it isn't set.
