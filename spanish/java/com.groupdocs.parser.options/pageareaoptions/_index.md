---
title: "PageAreaOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para la extracción de áreas de página."
type: docs
weight: 28
url: /es/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Proporciona las opciones que se utilizan para la extracción de áreas de página.

Una instancia de la clase [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) se usa como parámetro en [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
y los métodos [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-). Consulte los ejemplos de uso allí.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) con el tamaño del borde ignorado. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Inicializa una nueva instancia de la clase [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtiene el área rectangular que contiene áreas de página. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Obtiene el tamaño del borde que se ignora al capturarse por el área rectangular. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) con el tamaño del borde ignorado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene áreas de página. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Inicializa una nueva instancia de la clase [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene áreas de página. |
|
|  | rectangleTolerance | double | El tamaño del borde que se ignora al capturarse por el área rectangular. Se mide por la fracción de la altura de un elemento de texto. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtiene el área rectangular que contiene áreas de página.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Obtiene el tamaño del borde que se ignora al capturarse por el área rectangular. Se mide por la fracción de la altura de un elemento de texto.


**Returns:**
double - El valor double de 0 (sin borde) a 1 (ignorar todo el elemento).

