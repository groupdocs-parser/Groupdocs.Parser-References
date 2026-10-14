---
title: "PageTextArea"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un área de texto de página que se utiliza para representar un valor de texto en la funcionalidad de análisis mediante plantillas o análisis de formularios."
type: docs
weight: 24
url: /es/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Representa un área de texto de página que se utiliza para representar un valor de texto en la funcionalidad de análisis mediante plantillas o análisis de formularios.

Una instancia de la clase [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) se utiliza como valor de retorno de los siguientes métodos:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

También una instancia de la clase [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) se utiliza como valor de la propiedad [PageArea](../../com.groupdocs.parser.data/pagearea).
\*

Vea los ejemplos de uso allí.

El área de texto puede ser simple o compuesta. En el primer caso contiene un texto que está delimitado por un área rectangular.
En el segundo caso contiene otras áreas de texto; las propiedades de texto y tabla se calculan mediante áreas de texto hijas.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Inicializa una nueva instancia de la clase [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getText()](#getText--) | Obtiene el texto. |
|
|  | [getBaseLine()](#getBaseLine--) | Obtiene la línea base. |
|
|  | [getTextStyle()](#getTextStyle--) | Obtiene el estilo de texto, como el tamaño de fuente, el nombre de fuente, etc. |
|
|  | [getAreas()](#getAreas--) | Obtiene la colección de áreas de página de texto hijas. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | texto | java.lang.String | El valor del texto. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La página que contiene el área de texto. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el área de texto. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | texto | java.lang.String | El valor del texto. |
|
|  | baseLine | java.lang.Double | La línea base del texto. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | El estilo del texto. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La página que contiene el área de texto. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el área de texto. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Inicializa una nueva instancia de la clase [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La colección de áreas de página de texto hijas. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La página que contiene el área de texto. |
|

### getText() {#getText--}
```
public String getText()
```


Obtiene el texto.


**Returns:**
java.lang.String - Un valor string que representa un valor del área de página de texto.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Obtiene la línea base.


**Returns:**
double - Un valor double que representa la línea base.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Obtiene el estilo de texto, como el tamaño de fuente, el nombre de fuente, etc.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Obtiene la colección de áreas de página de texto hijas.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - Una colección de áreas de página de texto hijas; vacía si el área de página de texto no tiene hijos.

