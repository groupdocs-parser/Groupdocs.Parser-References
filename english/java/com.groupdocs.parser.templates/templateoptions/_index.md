---
title: TemplateOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for parsing by template functionality.
type: docs
weight: 17
url: /java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Provides the options which are used for parsing by template functionality.
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Initializes a new instance of the [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRectangleTolerance()](#getRectangleTolerance--) | Gets the size of the border that is ignored when captured by the rectangular area. |
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Initializes a new instance of the [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangleTolerance | double | The size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Gets the size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height.

**Returns:**
double - The double value from 0 (no border) to 1 (ignore the whole element).
