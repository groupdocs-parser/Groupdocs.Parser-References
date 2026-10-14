---
title: "TextOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para la extracción de texto."
type: docs
weight: 37
url: /es/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Proporciona las opciones que se utilizan para la extracción de texto.

Una instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions) se usa como parámetro en [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-)
y los métodos [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-) . Consulte los ejemplos de uso allí.

Se usa para especificar el modo bruto de extracción de texto. Un texto en este modo se extrae de forma no precisa
pero más rápido que en el modo estándar. Si el modo bruto no admite el formato del documento,
entonces este parámetro se ignora y se usa el modo estándar.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions). |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions) con la opción de uso de OCR. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions) con la capacidad de establecer opciones de OCR. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Obtiene el valor que indica si se usa el modo bruto. |
|
|  | [isUseOcr()](#isUseOcr--) | Obtiene el valor que indica si se usa el Conector OCR para extraer un texto. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Obtiene las opciones adicionales para la funcionalidad OCR. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Obtiene el valor que indica si las anotaciones están incluidas en el texto extraído. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Establece el valor que indica si las anotaciones están incluidas en el texto extraído. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | El valor que indica si se usa el modo bruto. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions) con la opción de uso de OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | El valor que indica si se usa el modo bruto. |
|
|  | useOcr | boolean | El valor que indica si se usa la funcionalidad OCR para extraer un texto. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions) con la capacidad de establecer opciones de OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | El valor que indica si se usa el modo bruto. |
|
|  | useOcr | boolean | El valor que indica si se usa la funcionalidad OCR para extraer un texto. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Las opciones adicionales para la funcionalidad OCR. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Obtiene el valor que indica si se usa el modo bruto.


**Returns:**
booleano -  true  si se usa el modo bruto; de lo contrario,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Obtiene el valor que indica si se usa el Conector OCR para extraer un texto.


**Returns:**
booleano -  true  si se usa la funcionalidad OCR; de lo contrario,  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Obtiene las opciones adicionales para la funcionalidad OCR.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Obtiene el valor que indica si las anotaciones están incluidas en el texto extraído. El valor predeterminado es  false .


**Returns:**
booleano -  true  si las anotaciones están incluidas; de lo contrario,  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Establece el valor que indica si las anotaciones están incluidas en el texto extraído.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  para incluir anotaciones en el texto extraído. |
|

