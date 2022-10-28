---
title: FormattedTextOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for formatted text extraction.
type: docs
weight: 18
url: /java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Provides the options which are used for formatted text extraction.

An instance of [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) class is used as parameter in [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser\#getFormattedText-FormattedTextOptions-) and [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser\#getFormattedText-int--FormattedTextOptions-) methods. See the usage examples there.

**Learn more:**

 *  [Extract formatted text from document][]
 *  Extract a document text as [HTML][]
 *  Extract a document text as [Markdown][]
 *  Extract a document text as [Plain text][]


[Extract formatted text from document]: https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document
[HTML]: https://docs.groupdocs.com/display/parserjava/HTML
[Markdown]: https://docs.groupdocs.com/display/parserjava/Markdown
[Plain text]: https://docs.groupdocs.com/display/parserjava/Plain+text
## Constructors

| Constructor | Description |
| --- | --- |
| [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Initializes a new instance of the [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getMode()](#getMode--) | Gets the formatted text extraction mode. |
### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Initializes a new instance of the [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | The mode of formatted text extraction. |

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Gets the formatted text extraction mode.

**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.
