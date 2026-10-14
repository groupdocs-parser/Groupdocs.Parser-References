---
title: "HighlightOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para extraer un resaltado de un bloque de texto alrededor del texto encontrado en escenarios de búsqueda."
type: docs
weight: 22
url: /es/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Proporciona las opciones que se utilizan para extraer un resaltado (un bloque de texto alrededor del texto encontrado en escenarios de búsqueda).

Una instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) se usa como parámetro en el método [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-).
Vea los ejemplos de uso allí.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sin límites establecidos. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) que se usa para extraer un resaltado de longitud fija. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) que se usa para extraer un resaltado limitado por línea. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) que se usa para extraer un resaltado con un recuento de palabras fijo. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Obtiene una longitud máxima de texto. |
|
|  | [getWordCount()](#getWordCount--) | Obtiene un recuento máximo de palabras. |
|
|  | [isLineLimited()](#isLineLimited--) | Obtiene el valor que indica si la extracción del resaltado está limitada por el inicio (o el final) de una línea de texto. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Establece una longitud máxima de texto. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Establece un recuento máximo de palabras. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Establece el valor que indica si la extracción del resaltado está limitada por el inicio (o el final) de una línea de texto. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sin límites establecidos. Establezca al menos uno de #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) antes de pasar al analizador.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) que se usa para extraer un resaltado de longitud fija.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | maxLength | int | La longitud máxima de texto. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) que se usa para extraer un resaltado limitado por línea.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | La longitud máxima de texto. |
|
|  | isLineLimited | boolean | El valor que indica si la extracción de resaltado está limitada por el inicio (o el final) de una línea de texto. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) que se usa para extraer un resaltado con un recuento de palabras fijo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | La longitud máxima de texto. |
|
|  | wordCount | int | El recuento máximo de palabras. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Inicializa una nueva instancia de la clase [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | La longitud máxima de texto. |
|
|  | wordCount | java.lang.Integer | El recuento máximo de palabras. |
|
|  | isLineLimited | boolean | El valor que indica si la extracción de resaltado está limitada por el inicio (o el final) de una línea de texto. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Obtiene una longitud máxima de texto.


**Returns:**
java.lang.Integer - Un valor entero positivo que representa la longitud máxima del texto;  null  si la longitud del texto no está limitada.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Obtiene un recuento máximo de palabras.


**Returns:**
java.lang.Integer - Un valor entero positivo que representa el recuento máximo de palabras;  null  si el recuento de palabras no está limitado.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Obtiene el valor que indica si la extracción del resaltado está limitada por el inicio (o el final) de una línea de texto.


**Returns:**
boolean -  true  si la extracción de resaltado está limitada por el inicio (o el final) de una línea de texto; de lo contrario,  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Establece una longitud máxima de texto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Un entero no negativo;  null  para eliminar el límite de longitud. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Establece un recuento máximo de palabras.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Un entero no negativo;  null  para eliminar el límite del recuento de palabras. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Establece el valor que indica si la extracción del resaltado está limitada por el inicio (o el final) de una línea de texto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | lineLimited | boolean | true  para limitar por los límites de línea. |
|

