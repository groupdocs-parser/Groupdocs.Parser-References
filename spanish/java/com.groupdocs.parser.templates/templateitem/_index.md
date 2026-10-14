---
title: "TemplateItem"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona una clase abstracta base para los elementos de plantilla."
type: docs
weight: 14
url: /es/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Proporciona una clase abstracta base para los elementos de plantilla.

Los herederos de la clase [TemplateItem](../../com.groupdocs.parser.templates/templateitem) se utilizan en la colección [Template](../../com.groupdocs.parser.templates/template).

## Métodos

| Método | Descripción |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Crea una copia del elemento actual con todas las coordenadas escaladas por el factor dado. |
|
|  | [getName()](#getName--) | Obtiene el nombre del elemento de plantilla. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtiene el índice de página del elemento de plantilla. |
|
|  | [getPageWidth()](#getPageWidth--) | Obtiene el ancho de la página que se utilizó para crear el elemento de plantilla. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Obtiene un valor que indica si un  Name  fue convertido a MAYÚSCULAS. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Crea una copia del elemento actual con todas las coordenadas escaladas por el factor dado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | factor | double | El factor de escala. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del elemento de plantilla.


**Returns:**
java.lang.String - Un valor de cadena en mayúsculas que representa el nombre del elemento de plantilla.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Obtiene el índice de página del elemento de plantilla.


**Returns:**
java.lang.Integer - Un valor entero que representa el índice de la página donde se encuentra el elemento de plantilla;  null  si el elemento de plantilla está ubicado en cualquier página.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Obtiene el ancho de la página que se utilizó para crear el elemento de plantilla.


**Returns:**
java.lang.Double - El ancho de la página en píxeles;  null  si el ancho de la página es desconocido.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Obtiene un valor que indica si un  Name  fue convertido a MAYÚSCULAS.


**Returns:**
boolean - Un valor booleano que indica si un  Name  fue convertido a MAYÚSCULAS.

