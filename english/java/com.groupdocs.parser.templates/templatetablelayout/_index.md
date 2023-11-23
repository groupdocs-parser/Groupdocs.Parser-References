---
title: TemplateTableLayout
second_title: GroupDocs.Parser for Java API Reference
description: Provides the template table layout which is used by  class to define table position.
type: docs
weight: 21
url: /java/com.groupdocs.parser.templates/templatetablelayout/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableLayout
```

Provides the template table layout which is used by [TemplateTable](../../com.groupdocs.parser.templates/templatetable) class to define table position.
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)](#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--) | Initializes a new instance of the [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRectangle()](#getRectangle--) | Gets the rectangular area that contains the table. |
| [getVerticalSeparators()](#getVerticalSeparators--) | Gets the table columns separators. |
| [getHorizontalSeparators()](#getHorizontalSeparators--) | Gets the table rows separators. |
| [moveTo(Point point)](#moveTo-com.groupdocs.parser.data.Point-) | Creates a new layout with the same size, separators and position in the point. |
### TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators) {#TemplateTableLayout-java.lang.Iterable-java.lang.Double--java.lang.Iterable-java.lang.Double--}
```
public TemplateTableLayout(Iterable<Double> verticalSeparators, Iterable<Double> horizontalSeparators)
```


Initializes a new instance of the [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| verticalSeparators | java.lang.Iterable<java.lang.Double> | The table columns separators. |
| horizontalSeparators | java.lang.Iterable<java.lang.Double> | The table rows separators. |

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gets the rectangular area that contains the table.

**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table.
### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Gets the table columns separators.

**Returns:**
java.util.List<java.lang.Double> - A collection of double values that represent x-coordinates of the table columns separators.
### getHorizontalSeparators() {#getHorizontalSeparators--}
```
public List<Double> getHorizontalSeparators()
```


Gets the table rows separators.

**Returns:**
java.util.List<java.lang.Double> - A collection of double values that represent y-coordinates of the table rows separators.
### moveTo(Point point) {#moveTo-com.groupdocs.parser.data.Point-}
```
public TemplateTableLayout moveTo(Point point)
```


Creates a new layout with the same size, separators and position in the point.

This functionality allows to move Table Layout.

For example, a document has tables on each page (or a set of documents with a table on the page). These tables differ by position and content, but have the same columns and rows. In this case a user can define [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object at (0, 0) once and then move it to the location of the definite table.

If the table position depends on the other object of the page, a user can define [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object based on template document and then move it according to an anchor object. For example, if this is a summary table and it is followed by details table (which can contain a different count of rows). In this case a user can define [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.

 moveTo(Point)  method returns a copy of the current object. A user can pass any coordinates (even negative - then layout will be moved to the left/top).

```
// Create a table layout
 TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 0.0, 25.0, 150.0, 180.0, 230.0 }),
     java.util.Arrays.asList(new Double[] { 0.0, 15.0, 30.0, 45.0, 60.0, 75.0 }));
 // Print a rectangle
 Rectangle rect = layout.getRectangle();
 // Prints: pos: (0, 0) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         rect.getLeft(), rect.getTop(),
         rect.getSize().getWidth(), rect.getSize().getHeight()));
 // Move layout to the definite table location
 TemplateTableLayout movedLayout = layout.moveTo(new Point(315, 250));
 // Ensure that the first separators are moved:
 System.out.println(movedLayout.getVerticalSeparators().get(0)); // prints: 315
 System.out.println(movedLayout.getHorizontalSeparators().get(0)); // prints: 250
 Rectangle movedRect = movedLayout.getRectangle();
 // Prints: pos: (315, 250) size: (230, 75)
 System.out.println(String.format("pos: (%d, %d) size: (%d, %d)",
         movedRect.getLeft(), movedRect.getTop(),
         movedRect.getSize().getWidth(), movedRect.getSize().getHeight()));
 // movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
 movedLayout.getHorizontalSeparators().add(90.0);
 System.out.println(movedLayout.getHorizontalSeparators().size()); // prints: 7
 System.out.println(layout.getHorizontalSeparators().size()); // prints: 6
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| point | [Point](../../com.groupdocs.parser.data/point) | The position of the new layout. |

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - A new layout with the same size, separators and position in the point.
