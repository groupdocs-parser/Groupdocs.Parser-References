---
title: "Características"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa la lista de funciones compatibles."
type: docs
weight: 18
url: /es/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Representa la lista de características compatibles. Permite obtener información sobre qué características son compatibles o no para el documento.

Una instancia de esta clase se usa como propiedad [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--). Consulte los ejemplos de uso allí.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [Features()](#Features--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Devuelve el valor que indica si la característica está soportada. |
|
|  | [isText()](#isText--) | Obtiene el valor que indica si la extracción de texto está soportada. |
|
|  | [isTextPage()](#isTextPage--) | Obtiene el valor que indica si la extracción de página de texto está soportada. |
|
|  | [isFormattedText()](#isFormattedText--) | Obtiene el valor que indica si la extracción de texto formateado está soportada. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Obtiene el valor que indica si la extracción de página de texto formateado está soportada. |
|
|  | [isSearch()](#isSearch--) | Obtiene el valor que indica si la búsqueda de texto está soportada. |
|
|  | [isHighlight()](#isHighlight--) | Obtiene el valor que indica si la extracción de resaltado está soportada. |
|
|  | [isBarcodes()](#isBarcodes--) | Obtiene el valor que indica si la extracción de códigos de barras está soportada. |
|
|  | [isToc()](#isToc--) | Obtiene el valor que indica si la extracción de tabla de contenido está soportada. |
|
|  | [isMetadata()](#isMetadata--) | Obtiene el valor que indica si la extracción de metadatos está soportada. |
|
|  | [isContainer()](#isContainer--) | Obtiene el valor que indica si la extracción de contenedor está soportada. |
|
|  | [isTextAreas()](#isTextAreas--) | Obtiene el valor que indica si la extracción de áreas de texto está soportada. |
|
|  | [isStructure()](#isStructure--) | Obtiene el valor que indica si la extracción de estructura de texto está soportada. |
|
|  | [isImages()](#isImages--) | Obtiene el valor que indica si la extracción de imágenes está soportada. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Obtiene el valor que indica si la extracción de hipervínculos está soportada. |
|
|  | [isTables()](#isTables--) | Obtiene el valor que indica si la extracción de tablas está soportada. |
|
|  | [isAnnotations()](#isAnnotations--) | Obtiene el valor que indica si la extracción de anotaciones está soportada. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Obtiene el valor que indica si el análisis por plantilla está soportado. |
|
|  | [isParseForm()](#isParseForm--) | Obtiene el valor que indica si el análisis de formularios es compatible. |
|
|  | [isPreview()](#isPreview--) | Obtiene el valor que indica si la generación de vista previa es compatible. |
|
|  | [isPagePreview()](#isPagePreview--) | Obtiene el valor que indica si la generación de vista previa de la página es compatible. |
|
|  | [isOcr()](#isOcr--) | Obtiene el valor que indica si la funcionalidad OCR es compatible. |
|
|  | [isWorksheet()](#isWorksheet--) | Obtiene el valor que indica si la extracción de la hoja de cálculo es compatible. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Devuelve el valor que indica si la característica está soportada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | featureName | java.lang.String | El nombre de la característica. |
|

**Returns:**
boolean -  true  si la característica es compatible; de lo contrario,  false .

### isText() {#isText--}
```
public boolean isText()
```


Obtiene el valor que indica si la extracción de texto está soportada.


**Returns:**
boolean -  true  si la extracción de texto es compatible; de lo contrario,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Obtiene el valor que indica si la extracción de página de texto está soportada.


**Returns:**
boolean -  true  si la extracción de página de texto es compatible; de lo contrario,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Obtiene el valor que indica si la extracción de texto formateado está soportada.


**Returns:**
boolean -  true  si la extracción de texto formateado es compatible; de lo contrario,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Obtiene el valor que indica si la extracción de página de texto formateado está soportada.


**Returns:**
boolean -  true  si la página de texto formateado es compatible; de lo contrario,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Obtiene el valor que indica si la búsqueda de texto está soportada.


**Returns:**
boolean -  true  si la búsqueda de texto es compatible; de lo contrario,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Obtiene el valor que indica si la extracción de resaltado está soportada.


**Returns:**
boolean -  true  si la extracción de resaltado es compatible; de lo contrario,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Obtiene el valor que indica si la extracción de códigos de barras está soportada.


**Returns:**
boolean -  true  si la extracción de códigos de barras es compatible; de lo contrario,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


Obtiene el valor que indica si la extracción de tabla de contenido está soportada.


**Returns:**
boolean -  true  si la extracción de tabla de contenido es compatible; de lo contrario,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Obtiene el valor que indica si la extracción de metadatos está soportada.


**Returns:**
boolean -  true  si la extracción de metadatos es compatible; de lo contrario,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Obtiene el valor que indica si la extracción de contenedor está soportada.


**Returns:**
boolean -  true  si la extracción de contenedor es compatible; de lo contrario,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Obtiene el valor que indica si la extracción de áreas de texto está soportada.


**Returns:**
boolean -  true  si la extracción de áreas de texto es compatible; de lo contrario,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Obtiene el valor que indica si la extracción de estructura de texto está soportada.


**Returns:**
boolean -  true  si la extracción de estructura de texto es compatible; de lo contrario,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Obtiene el valor que indica si la extracción de imágenes está soportada.


**Returns:**
boolean -  true  si la extracción de imágenes es compatible; de lo contrario,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Obtiene el valor que indica si la extracción de hipervínculos está soportada.


**Returns:**
boolean -  true  si la extracción de hipervínculos es compatible; de lo contrario,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Obtiene el valor que indica si la extracción de tablas está soportada.


**Returns:**
boolean -  true  si la extracción de tablas es compatible; de lo contrario,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Obtiene el valor que indica si la extracción de anotaciones está soportada.


**Returns:**
boolean -  true  si la extracción de anotaciones es compatible; de lo contrario,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Obtiene el valor que indica si el análisis por plantilla está soportado.


**Returns:**
boolean -  true  si el análisis por plantilla es compatible; de lo contrario,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Obtiene el valor que indica si el análisis de formularios es compatible.


**Returns:**
boolean -  true  si se admite el análisis de formularios; de lo contrario,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Obtiene el valor que indica si la generación de vista previa es compatible.


**Returns:**
boolean -  true  si se admite la generación de vista previa; de lo contrario,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Obtiene el valor que indica si la generación de vista previa de la página es compatible.


**Returns:**
boolean -  true  si se admite la generación de vista previa de la página; de lo contrario,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Obtiene el valor que indica si la funcionalidad OCR es compatible.


**Returns:**
boolean -  true  si se admite la funcionalidad OCR; de lo contrario,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Obtiene el valor que indica si la extracción de la hoja de cálculo es compatible.


**Returns:**
boolean -  true  si se admite la extracción de hoja de cálculo; de lo contrario,  false .

