---
title: TemplateFixedPosition
second_title: GroupDocs.Parser for Java API Reference
description: Provides a template field position which is defined by the rectangular area.
type: docs
weight: 13
url: /java/com.groupdocs.parser.templates/templatefixedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateFixedPosition extends TemplatePosition
```

Provides a template field position which is defined by the rectangular area.

This is simplest way to define the field position. It requires to set a rectangular area on the page that bounds the field value. All the text that is contained (even partially) into the rectangular area will be extracted as a value:

```
// Create a fixed template field with "Address" name which is bounded by a rectangle at the position (35, 160) and with the size (110, 20)
 TemplateField templateField = new TemplateField(
     new TemplateFixedPosition(new Rectangle(new Point(35, 160), new Size(110, 20))),
     "Address");
 
```
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateFixedPosition(Rectangle rectangle)](#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRectangle()](#getRectangle--) | Gets the rectangular area that contains the template field. |
### TemplateFixedPosition(Rectangle rectangle) {#TemplateFixedPosition-com.groupdocs.parser.data.Rectangle-}
```
public TemplateFixedPosition(Rectangle rectangle)
```


Initializes a new instance of the [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that contains the template field. |

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gets the rectangular area that contains the template field.

**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template field.
