---
title: "TemplateOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para el análisis mediante la funcionalidad de plantilla."
type: docs
weight: 17
url: /es/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Proporciona las opciones que se utilizan para el análisis mediante la funcionalidad de plantilla.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Inicializa una nueva instancia de la clase [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Obtiene el tamaño del borde que se ignora al capturarse por el área rectangular. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Inicializa una nueva instancia de la clase [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rectangleTolerance | double | El tamaño del borde que se ignora al capturarse por el área rectangular. Se mide por la fracción de la altura de un elemento de texto. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Obtiene el tamaño del borde que se ignora al capturarse por el área rectangular. Se mide por la fracción de la altura de un elemento de texto.


**Returns:**
double - El valor double de 0 (sin borde) a 1 (ignorar todo el elemento).

