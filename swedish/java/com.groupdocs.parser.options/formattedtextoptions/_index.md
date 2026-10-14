---
title: "FormattedTextOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för formaterad textutvinning."
type: docs
weight: 21
url: /sv/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Tillhandahåller de alternativ som används för formaterad textutvinning.

En instans av [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) klass används som parameter i [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-)
och [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) metoder. Se användningsexemplen där.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Initierar en ny instans av [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) klassen utan något läge inställt. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Initierar en ny instans av [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getMode()](#getMode--) | Hämtar läget för formaterad textutvinning. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Ställer in läget för formaterad textutvinning. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Initierar en ny instans av [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) klassen utan något läge inställt.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Initierar en ny instans av [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Läget för formaterad textutvinning. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Hämtar läget för formaterad textutvinning.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Ställer in läget för formaterad textutvinning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) uppräkning som innehåller ett läge för formaterad textutvinning. |
|

