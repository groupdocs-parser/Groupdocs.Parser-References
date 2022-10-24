---
title: TemplateItem
second_title: GroupDocs.Parser for Java API Reference
description: Provides a base abstract class for template items.
type: docs
weight: 14
url: /java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Provides a base abstract class for template items.

The inheritors of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class are used in [Template](../../com.groupdocs.parser.templates/template) collection.
## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--) | Gets the name of the template item. |
| [getPageIndex()](#getPageIndex--) | Gets the page index of the template item. |
### getName() {#getName--}
```
public String getName()
```


Gets the name of the template item.

**Returns:**
java.lang.String - An uppercase string value that represents a name of the template item.
### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Gets the page index of the template item.

**Returns:**
java.lang.Integer - An integer value that represents the index of the page where the template item is located;  null  if the template item is located on any page.
