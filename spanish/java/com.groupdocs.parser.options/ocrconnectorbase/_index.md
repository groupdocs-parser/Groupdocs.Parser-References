---
title: "OcrConnectorBase"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona la funcionalidad OCR."
type: docs
weight: 25
url: /es/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Proporciona la funcionalidad OCR.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Inicializa una nueva instancia de la clase [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Obtiene el valor que indica si la extracción de texto es compatible. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Obtiene el valor que indica si la extracción de áreas de texto es compatible. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Reconoce un texto a partir del flujo  imageStream  stream. |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Reconoce áreas de texto del flujo  imageStream  stream. |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Inicializa una nueva instancia de la clase [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase).


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Obtiene el valor que indica si la extracción de texto es compatible.


**Returns:**
boolean -  true  si la extracción de texto es compatible; de lo contrario,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Obtiene el valor que indica si la extracción de áreas de texto es compatible.


**Returns:**
boolean -  true  si la extracción de áreas de texto es compatible; de lo contrario,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


Reconoce un texto a partir del flujo  imageStream  stream.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | La representación de imagen de la página del documento. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Las opciones de OCR. |
|

**Returns:**
java.lang.String - Una cadena que representa un texto reconocido;  null  si el reconocimiento de texto no es compatible.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Reconoce áreas de texto del flujo  imageStream  stream.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | La representación de imagen de la página del documento. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | El tamaño de la página del documento. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Las opciones de OCR. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Una colección de objetos [PageTextArea](../../com.groupdocs.parser.data/pagetextarea);  null  si el reconocimiento de áreas de texto no es compatible.

