---
title: "FormattedTextOptions"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce le opzioni utilizzate per l'estrazione di testo formattato."
type: docs
weight: 21
url: /it/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Fornisce le opzioni utilizzate per l'estrazione di testo formattato.

Un'istanza della classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) è usata come parametro in [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-)
e i metodi [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) . Vedi gli esempi d'uso lì.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Inizializza una nuova istanza della classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) senza impostare alcuna modalità. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Inizializza una nuova istanza della classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getMode()](#getMode--) | Restituisce la modalità di estrazione del testo formattato. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Imposta la modalità di estrazione del testo formattato. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Inizializza una nuova istanza della classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) senza impostare alcuna modalità.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Inizializza una nuova istanza della classe [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | La modalità di estrazione del testo formattato. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Restituisce la modalità di estrazione del testo formattato.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Imposta la modalità di estrazione del testo formattato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | L'enumerazione [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) che contiene una modalità di estrazione del testo formattato. |
|

