---
title: "FormattedTextOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor het extraheren van opgemaakte tekst."
type: docs
weight: 21
url: /nl/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Biedt de opties die worden gebruikt voor het extraheren van opgemaakte tekst.

Een instantie van de klasse [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) wordt gebruikt als parameter in [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-)
en [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) methoden. Zie daar de gebruiksvoorbeelden.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Initialiseert een nieuwe instantie van de klasse [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) zonder ingestelde modus. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Initialiseert een nieuw exemplaar van de [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getMode()](#getMode--) | Haalt de modus voor het extraheren van opgemaakte tekst op. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Stelt de modus voor het extraheren van opgemaakte tekst in. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Initialiseert een nieuwe instantie van de klasse [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) zonder ingestelde modus.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Initialiseert een nieuw exemplaar van de [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | De modus voor het extraheren van opgemaakte tekst. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Haalt de modus voor het extraheren van opgemaakte tekst op.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Stelt de modus voor het extraheren van opgemaakte tekst in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeratie die een modus voor het extraheren van opgemaakte tekst bevat. |
|

