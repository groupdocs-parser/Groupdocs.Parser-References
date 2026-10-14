---
title: "PageArea"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa una clase base abstracta para áreas de página que se utilizan para representar bloques en la página del documento en la funcionalidad de análisis mediante plantillas."
type: docs
weight: 17
url: /es/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Representa una clase base abstracta para áreas de página que se utilizan para representar bloques en la página del documento en la funcionalidad de análisis mediante plantillas.

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtiene el área rectangular. |
|
|  | [getPage()](#getPage--) | Obtiene la información de la página del documento, como el índice de página y el tamaño de página. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtiene el área rectangular.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Obtiene la información de la página del documento, como el índice de página y el tamaño de página.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

