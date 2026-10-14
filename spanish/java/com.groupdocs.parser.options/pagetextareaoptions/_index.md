---
title: "PageTextAreaOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para la extracción de áreas de texto de página."
type: docs
weight: 32
url: /es/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Proporciona las opciones que se utilizan para la extracción de áreas de texto de página.

Una instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) se usa como parámetro en [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
y los métodos [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-). Consulte los ejemplos de uso allí.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con valores predeterminados. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions) con la opción de uso de OCR. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions) con la capacidad de establecer opciones de OCR. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con la expresión regular. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con la expresión regular y el área rectangular. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con la expresión regular, el área rectangular y el tamaño del borde ignorado. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions). |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con el tamaño del borde ignorado. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getExpression()](#getExpression--) | Obtiene la expresión regular. |
|
|  | [isMatchCase()](#isMatchCase--) | Obtiene el valor que indica si no se ignora la distinción de mayúsculas y minúsculas del texto. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Obtiene el valor que indica si los segmentos están unidos. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Obtiene el valor que indica si se ignora el formato del texto. |
|
|  | [isUseOcr()](#isUseOcr--) | Obtiene el valor que indica si se usa el Conector OCR para extraer un texto. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Obtiene las opciones adicionales para la funcionalidad OCR. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con valores predeterminados.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions) con la opción de uso de OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | useOcr | boolean | El valor que indica si se usa la funcionalidad OCR para extraer un texto. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


Inicializa una nueva instancia de la clase [TextOptions](../../com.groupdocs.parser.options/textoptions) con la capacidad de establecer opciones de OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | useOcr | boolean | El valor que indica si se usa la funcionalidad OCR para extraer un texto. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Las opciones adicionales para la funcionalidad OCR. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con la expresión regular. Otras opciones se establecen por defecto (ver observaciones para más detalles).

Las siguientes propiedades tienen valores predeterminados:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | expression | java.lang.String | La expresión regular. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con la expresión regular y el área rectangular. Otras opciones se establecen por defecto (ver observaciones para más detalles).

Las siguientes propiedades tienen valores predeterminados:

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | expression | java.lang.String | La expresión regular. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene áreas de página. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con la expresión regular, el área rectangular y el tamaño del borde ignorado. Otras opciones se establecen por defecto (ver observaciones para más detalles).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | expression | java.lang.String | La expresión regular. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene áreas de página. |
|
|  | rectangleTolerance | double | El tamaño del borde que se ignora al capturarse por el área rectangular. Se mide por la fracción de la altura de un elemento de texto. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | expression | java.lang.String | La expresión regular. |
|
|  | matchCase | boolean | El valor que indica si una distinción de mayúsculas y minúsculas no se ignora. |
|
|  | uniteSegments | boolean | El valor que indica si los segmentos están unidos. |
|
|  | ignoreFormatting | boolean | El valor que indica si el formato de texto se ignora. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene áreas de página. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Inicializa una nueva instancia de la clase [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) con el tamaño del borde ignorado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | expression | java.lang.String | La expresión regular. |
|
|  | matchCase | boolean | El valor que indica si una distinción de mayúsculas y minúsculas no se ignora. |
|
|  | uniteSegments | boolean | El valor que indica si los segmentos están unidos. |
|
|  | ignoreFormatting | boolean | El valor que indica si el formato de texto se ignora. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene áreas de página. |
|
|  | rectangleTolerance | double | El tamaño del borde que se ignora al capturarse por el área rectangular. Se mide por la fracción de la altura de un elemento de texto. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Obtiene la expresión regular.


**Returns:**
java.lang.String - Una cadena que representa la expresión regular.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Obtiene el valor que indica si no se ignora la distinción de mayúsculas y minúsculas del texto.


**Returns:**
boolean -  true  si una distinción de mayúsculas y minúsculas no se ignora; de lo contrario,  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Obtiene el valor que indica si los segmentos están unidos.


**Returns:**
boolean - {code true} si los segmentos están unidos; de lo contrario, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Obtiene el valor que indica si se ignora el formato del texto.


**Returns:**
boolean -  true  si el formato de texto se ignora; de lo contrario,  false .

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

