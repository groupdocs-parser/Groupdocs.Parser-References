---
title: TemplatePosition
second_title: GroupDocs.Parser for Java API Reference
description: Provides a base abstract class for template positions.
type: docs
weight: 18
url: /java/com.groupdocs.parser.templates/templateposition/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplatePosition
```

Provides a base abstract class for template positions.
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplatePosition()](#TemplatePosition--) |  |
## Methods

| Method | Description |
| --- | --- |
| [scale(double factor)](#scale-double-) | Creates a copy of the current position with all coordinates scaled by the given factor. |
### TemplatePosition() {#TemplatePosition--}
```
public TemplatePosition()
```


### scale(double factor) {#scale-double-}
```
public abstract TemplatePosition scale(double factor)
```


Creates a copy of the current position with all coordinates scaled by the given factor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| factor | double | The scaling factor. |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - A new [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) with scaled coordinates.
