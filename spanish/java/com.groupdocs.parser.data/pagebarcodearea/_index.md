---
title: "PageBarcodeArea"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un área de código de barras de página que se utiliza para representar un valor de código de barras en la funcionalidad de análisis mediante plantillas."
type: docs
weight: 18
url: /es/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Representa un área de código de barras de página que se utiliza para representar un valor de código de barras en la funcionalidad de análisis mediante plantillas.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getValue()](#getValue--) | Obtiene el valor del código de barras. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Obtiene el nombre del tipo de código de barras. |
|
|  | [getConfidence()](#getConfidence--) | Obtiene el nivel de confianza del código de barras analizado. |
|
|  | [getAngle()](#getAngle--) | Obtiene el ángulo del código de barras. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | El valor del código de barras. |
|
|  | codeTypeName | java.lang.String | El nombre del tipo de código de barras. |
|
|  | confidence | int | El nivel de confianza del código de barras analizado. |
|
|  | angle | double | El ángulo del código de barras. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La página que contiene el área del código de barras. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el área del código de barras. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Obtiene el valor del código de barras.


**Returns:**
java.lang.String - Un valor de cadena que representa un valor del área de página del código de barras.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Obtiene el nombre del tipo de código de barras.


**Returns:**
java.lang.String - Un valor de cadena que representa el nombre de tipo del código de barras.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Obtiene el nivel de confianza del código de barras analizado.


**Returns:**
int - Un valor entero que representa la confianza del código de barras analizado (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


Obtiene el ángulo del código de barras.


**Returns:**
double - Un valor entero que representa el ángulo del código de barras (0-360).

