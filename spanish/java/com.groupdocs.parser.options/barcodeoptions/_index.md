---
title: "BarcodeOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para la extracción de códigos de barras."
type: docs
weight: 10
url: /es/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Proporciona las opciones que se utilizan para la extracción de códigos de barras.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | Inicializa una nueva instancia de la clase BarcodeOptions con valores predeterminados. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase BarcodeOptions con el área rectangular. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Inicializa una nueva instancia de la clase BarcodeOptions con configuraciones de calidad y tipos de código. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Inicializa una nueva instancia de la clase BarcodeOptions. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Obtiene el valor que indica si se permiten los códigos de barras incorrectos. |
|
|  | [getDimension()](#getDimension--) | Obtiene el tamaño mínimo del elemento mínimo del código de barras. |
|
|  | [getImageQuality()](#getImageQuality--) | Obtiene la calidad de una imagen de origen. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Obtiene la calidad de un código de barras de origen. |
|
|  | [getRectangle()](#getRectangle--) | Obtiene el área rectangular que contiene áreas de página. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Obtiene los tipos de códigos de barras a leer. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Establece el valor que indica si se permiten los códigos de barras incorrectos. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Establece el tamaño mínimo del elemento mínimo del código de barras. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Establece la calidad de una imagen de origen. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Establece la calidad de un código de barras de origen. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Establece el área rectangular que contiene códigos de barras. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Establece los tipos de códigos de barras a leer. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Inicializa una nueva instancia de la clase BarcodeOptions con valores predeterminados.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Inicializa una nueva instancia de la clase BarcodeOptions con el área rectangular.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene códigos de barras. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Inicializa una nueva instancia de la clase BarcodeOptions con configuraciones de calidad y tipos de código.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La calidad de una imagen de origen. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La calidad de un código de barras de origen. |
|
|  | codeTypes | java.lang.String[] | Los tipos de códigos de barras a leer. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Inicializa una nueva instancia de la clase BarcodeOptions.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene códigos de barras. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La calidad de una imagen de origen. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La calidad de un código de barras de origen. |
|
|  | dimension | java.lang.Float | El tamaño mínimo del elemento mínimo del código de barras. |
|
|  | allowIncorrectBarcodes | boolean | El valor que indica si se permiten los códigos de barras incorrectos. |
|
|  | codeTypes | java.lang.String[] | Los tipos de códigos de barras a leer. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Obtiene el valor que indica si se permiten los códigos de barras incorrectos.


**Returns:**
boolean -  true  si se permiten los códigos de barras incorrectos; de lo contrario,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Obtiene el tamaño mínimo del elemento mínimo del código de barras.


**Returns:**
java.lang.Float - El valor float que representa el elemento mínimo del código de barras;  null  si se usa el modo automático.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Obtiene la calidad de una imagen de origen.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Obtiene la calidad de un código de barras de origen.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtiene el área rectangular que contiene áreas de página.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Obtiene los tipos de códigos de barras a leer.


**Returns:**
java.util.List<java.lang.String> - La colección de solo lectura que contiene tipos de códigos de barras a leer; colección vacía si no está establecida.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Establece el valor que indica si se permiten los códigos de barras incorrectos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  si se permiten los códigos de barras incorrectos. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Establece el tamaño mínimo del elemento mínimo del código de barras.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | dimension | java.lang.Float | El elemento mínimo del código de barras;  null  para modo automático. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Establece la calidad de una imagen de origen.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | El modo de calidad de imagen. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Establece la calidad de un código de barras de origen.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | El modo de calidad del código de barras. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Establece el área rectangular que contiene códigos de barras.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular;  null  para escanear toda la página. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Establece los tipos de códigos de barras a leer.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | Los tipos de códigos de barras;  null  o vacío para todos los tipos. |
|

