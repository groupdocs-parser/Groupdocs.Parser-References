---
title: "FormattedTextOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für die Extraktion formatierten Textes verwendet werden."
type: docs
weight: 21
url: /de/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Stellt die Optionen bereit, die für die Extraktion formatierten Textes verwendet werden.

Eine Instanz der Klasse [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) wird als Parameter in [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-) verwendet.
und den Methoden [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-). Siehe dort die Anwendungsbeispiele.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Initialisiert eine neue Instanz der Klasse [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) ohne gesetzten Modus. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Initialisiert eine neue Instanz der Klasse [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getMode()](#getMode--) | Gibt den Modus der formatierter Textextraktion zurück. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Setzt den Modus der formatierter Textextraktion. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Initialisiert eine neue Instanz der Klasse [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) ohne gesetzten Modus.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Initialisiert eine neue Instanz der Klasse [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Der Modus der formatierter Textextraktion. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Gibt den Modus der formatierter Textextraktion zurück.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Setzt den Modus der formatierter Textextraktion.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) Aufzählung, die einen Modus der formatierter Textextraktion enthält. |
|

