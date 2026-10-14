---
title: "FormattedTextOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour l'extraction de texte formaté."
type: docs
weight: 21
url: /fr/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Fournit les options utilisées pour l'extraction de texte formaté.

Une instance de la classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) est utilisée comme paramètre dans [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-)
et les méthodes [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-). Voir les exemples d’utilisation là‑bas.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Constructors

| Constructor | Description |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Initialise une nouvelle instance de la classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) sans mode défini. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Initialise une nouvelle instance de la classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getMode()](#getMode--) | Obtient le mode d’extraction du texte formaté. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Définit le mode d’extraction du texte formaté. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Initialise une nouvelle instance de la classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) sans mode défini.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Initialise une nouvelle instance de la classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Le mode d’extraction du texte formaté. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Obtient le mode d’extraction du texte formaté.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Définit le mode d’extraction du texte formaté.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Énumération [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) qui contient un mode d’extraction du texte formaté. |
|

