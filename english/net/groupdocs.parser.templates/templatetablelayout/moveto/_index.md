---
title: MoveTo
second_title: GroupDocs.Parser for .NET API Reference
description: Creates a new layout with the same size separators and position in the point.
type: docs
weight: 50
url: /net/groupdocs.parser.templates/templatetablelayout/moveto/
---
## TemplateTableLayout.MoveTo method

Creates a new layout with the same size, separators and position in the *point*.

```csharp
public TemplateTableLayout MoveTo(Point point)
```

| Parameter | Type | Description |
| --- | --- | --- |
| point | Point | The position of the new layout. |

### Return Value

A new layout with the same size, separators and position in the *point*.

### Examples

This functionality allows to move Table Layout.

For example, a document has tables on each page (or a set of documents with a table on the page). These tables differ by position and content, but have the same columns and rows. In this case a user can define [`TemplateTableLayout`](../../templatetablelayout) object at `(0, 0)` once and then move it to the location of the definite table.

If the table position depends on the other object of the page, a user can define [`TemplateTableLayout`](../../templatetablelayout) object based on template document and then move it according to an anchor object. For example, if this is a summary table and it is followed by details table (which can contain a different count of rows). In this case a user can define [`TemplateTableLayout`](../../templatetablelayout) object on template document (with the known details table rectangle) and then move [`TemplateTableLayout`](../../templatetablelayout) object according to the difference of details table rectangle of template and real document.

`MoveTo` method returns a copy of the current object. A user can pass any coordinates (even negative - then layout will be moved to the left/top).

```csharp
// Create a table layout
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 0, 25, 150, 180, 230 },
    new double[] { 0, 15, 30, 45, 60, 75 });

// Print a rectangle
Rectangle rect = layout.Rectangle;

// Prints: pos: (0, 0) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", rect.Left, rect.Top, rect.Size.Width, rect.Size.Height));

// Move layout to the definite table location
TemplateTableLayout movedLayout = layout.MoveTo(new Point(315, 250));

// Ensure that the first separators are moved:
Console.WriteLine(movedLayout.VerticalSeparators[0]); // prints: 315
Console.WriteLine(movedLayout.HorizontalSeparators[0]); // prints: 250

Rectangle movedRect = movedLayout.Rectangle;

// Prints: pos: (315, 250) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", movedRect.Left, movedRect.Top, movedRect.Size.Width, movedRect.Size.Height));

// movedLayout object is a copy of layout object, thus we can tune separators without the impact on the original layout:
movedLayout.HorizontalSeparators.Add(90);

Console.WriteLine(movedLayout.HorizontalSeparators.Count); // prints: 7
Console.WriteLine(layout.HorizontalSeparators.Count); // prints: 6
```

### See Also

* class [Point](../../../groupdocs.parser.data/point)
* class [TemplateTableLayout](../../templatetablelayout)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
