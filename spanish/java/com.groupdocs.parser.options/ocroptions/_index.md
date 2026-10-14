---
title: "OcrOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para el Conector OCR."
type: docs
weight: 27
url: /es/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Proporciona las opciones que se utilizan para el Conector OCR.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con valores predeterminados. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con un área rectangular. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con opciones de vista previa de página. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con el objeto [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con un área rectangular y el objeto [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtiene el área rectangular que limita el área de la página que se utiliza para el reconocimiento de texto. |
|
|  | [getHandler()](#getHandler--) | Obtiene el controlador de eventos para capturar eventos de OCR. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Obtiene el valor que indica si se usa el corrector ortográfico. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | Obtiene las opciones de vista previa de página utilizadas para renderizar la página que se envía al motor OCR. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Establece las opciones de vista previa de página utilizadas para renderizar la página que se envía al motor OCR. |
|
|  | [getLanguage()](#getLanguage--) | Obtiene el idioma utilizado para el reconocimiento óptico de caracteres. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Establece el idioma utilizado para el reconocimiento óptico de caracteres. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Establece el área rectangular que delimita el área de la página utilizada para el reconocimiento de texto. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Establece el controlador de eventos para capturar eventos OCR. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Establece el valor que indica si se usa el corrector ortográfico. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con valores predeterminados.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con un área rectangular.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que delimita el área de la página utilizada para el reconocimiento de texto. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con opciones de vista previa de página.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Las opciones utilizadas para renderizar la vista previa de la página que se envía al motor OCR. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con el objeto [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Una instancia de [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) para capturar eventos OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions) con un área rectangular y el objeto [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que delimita el área de la página utilizada para el reconocimiento de texto. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Una instancia de [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) para capturar eventos OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Inicializa una nueva instancia de la clase [OcrOptions](../../com.groupdocs.parser.options/ocroptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que delimita el área de la página utilizada para el reconocimiento de texto. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Una instancia de [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) para capturar eventos OCR. |
|
|  | useSpellCheker | boolean | El valor que indica si se usa el corrector ortográfico. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtiene el área rectangular que limita el área de la página que se utiliza para el reconocimiento de texto.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Obtiene el controlador de eventos para capturar eventos de OCR.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Obtiene el valor que indica si se usa el corrector ortográfico.


**Returns:**
boolean -  true  si se usa el corrector ortográfico; de lo contrario,  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Obtiene las opciones de vista previa de página utilizadas para renderizar la página que se envía al motor OCR.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Establece las opciones de vista previa de página utilizadas para renderizar la página que se envía al motor OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Las opciones de vista previa de página. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Obtiene el idioma utilizado para el reconocimiento óptico de caracteres.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Establece el idioma utilizado para el reconocimiento óptico de caracteres.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | El valor enum de [Language](../../com.groupdocs.parser.options/language). |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Establece el área rectangular que delimita el área de la página utilizada para el reconocimiento de texto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El rectángulo, o  null  para escanear toda la página. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Establece el controlador de eventos para capturar eventos OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | El controlador de eventos. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Establece el valor que indica si se usa el corrector ortográfico.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  para habilitar la corrección ortográfica. |
|

