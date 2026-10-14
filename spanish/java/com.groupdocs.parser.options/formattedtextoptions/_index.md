---
title: "FormattedTextOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para la extracción de texto con formato."
type: docs
weight: 21
url: /es/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Proporciona las opciones que se utilizan para la extracción de texto con formato.

Una instancia de la clase [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) se usa como parámetro en [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-)
y los métodos [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) . Consulte los ejemplos de uso allí.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Inicializa una nueva instancia de la clase [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) sin modo establecido. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Inicializa una nueva instancia de la clase [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getMode()](#getMode--) | Obtiene el modo de extracción de texto formateado. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Establece el modo de extracción de texto formateado. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Inicializa una nueva instancia de la clase [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) sin modo establecido.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Inicializa una nueva instancia de la clase [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | El modo de extracción de texto formateado. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Obtiene el modo de extracción de texto formateado.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Establece el modo de extracción de texto formateado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Enumeración [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) que contiene un modo de extracción de texto formateado. |
|

