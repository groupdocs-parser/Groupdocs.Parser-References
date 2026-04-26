---
title: PageTableAreaOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for page table areas extraction.
type: docs
weight: 31
url: /java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Provides the options which are used for page table areas extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Initializes a new instance of the [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) class. |
| [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) class with a search rectangle and no fixed layout. |
## Methods

| Method | Description |
| --- | --- |
| [getTableLayout()](#getTableLayout--) | Gets the table layout which defines the table on a page. |
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Initializes a new instance of the [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | The table layout which defines the table on a page. |

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Initializes a new instance of the [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) class with a search rectangle and no fixed layout.

Useful for restricting auto-detected tables to a region of the page. Mirrors the C\#  new PageTableAreaOptions(null) \{ Rectangle = ... \}  pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area on the page where tables should be detected; pass  null  to search the entire page. |

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Gets the table layout which defines the table on a page.

**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.
