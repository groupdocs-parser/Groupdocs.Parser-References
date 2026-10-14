---
title: "SearchOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para la búsqueda de texto."
type: docs
weight: 35
url: /es/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Proporciona las opciones que se utilizan para la búsqueda de texto.

Una instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) se usa como parámetro en el método [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-).
Vea los ejemplos de uso allí.

**Learn more:**

* [Search text](../https://docs.groupdocs.com/display/parserjava/Search+text)
* [Search text in Microsoft Office Word documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents)
* [Search text in Emails](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails)
* [Search text in EPUB eBooks](../https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](../https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](../https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) que se usa para buscar con las opciones de resaltado para la extracción del resaltado izquierdo y derecho. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) que se usa para buscar con las mismas opciones de resaltado para la extracción del resaltado izquierdo y derecho. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) que se usa para buscar sin extracción de resaltado. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) que se usa para buscar por páginas y sin extracción de resaltado. |
|
|  | [SearchOptions()](#SearchOptions--) | Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) con valores predeterminados. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Obtiene el valor que indica si no se ignora la distinción de mayúsculas y minúsculas del texto. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Obtiene el valor que indica si la búsqueda de texto está limitada a una palabra completa. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Obtiene el valor que indica si se utiliza una expresión regular. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Obtiene el valor que indica si la búsqueda se realiza por páginas. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Obtiene las opciones para el resaltado izquierdo. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Obtiene las opciones para el resaltado derecho. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Obtiene el valor que representa el índice máximo de la página a buscar. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matchCase | boolean | El valor que indica si una distinción de mayúsculas y minúsculas no se ignora. |
|
|  | matchWholeWord | boolean | El valor que indica si la búsqueda de texto está limitada a una palabra completa. |
|
|  | useRegularExpression | boolean | El valor que indica si se utiliza una expresión regular. |
|
|  | searchByPages | boolean | El valor que indica si la búsqueda se realiza por páginas. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Las opciones para el resaltado izquierdo. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Las opciones para el resaltado derecho. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matchCase | boolean | El valor que indica si una distinción de mayúsculas y minúsculas no se ignora. |
|
|  | matchWholeWord | boolean | El valor que indica si la búsqueda de texto está limitada a una palabra completa. |
|
|  | useRegularExpression | boolean | El valor que indica si se utiliza una expresión regular. |
|
|  | maxPageIndex | int | El valor que representa el índice máximo de la página a buscar |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Las opciones para el resaltado izquierdo. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Las opciones para el resaltado derecho. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) que se usa para buscar con las opciones de resaltado para la extracción del resaltado izquierdo y derecho.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matchCase | boolean | El valor que indica si una distinción de mayúsculas y minúsculas no se ignora. |
|
|  | matchWholeWord | boolean | El valor que indica si la búsqueda de texto está limitada a una palabra completa. |
|
|  | useRegularExpression | boolean | El valor que indica si se utiliza una expresión regular. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Las opciones para el resaltado izquierdo. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Las opciones para el resaltado derecho. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) que se usa para buscar con las mismas opciones de resaltado para la extracción del resaltado izquierdo y derecho.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matchCase | boolean | El valor que indica si una distinción de mayúsculas y minúsculas no se ignora. |
|
|  | matchWholeWord | boolean | El valor que indica si la búsqueda de texto está limitada a una palabra completa. |
|
|  | useRegularExpression | boolean | El valor que indica si se utiliza una expresión regular. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Las opciones para ambos resaltados. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) que se usa para buscar sin extracción de resaltado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matchCase | boolean | El valor que indica si una distinción de mayúsculas y minúsculas no se ignora. |
|
|  | matchWholeWord | boolean | El valor que indica si la búsqueda de texto está limitada a una palabra completa. |
|
|  | useRegularExpression | boolean | El valor que indica si se utiliza una expresión regular. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) que se usa para buscar por páginas y sin extracción de resaltado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matchCase | boolean | El valor que indica si una distinción de mayúsculas y minúsculas no se ignora. |
|
|  | matchWholeWord | boolean | El valor que indica si la búsqueda de texto está limitada a una palabra completa. |
|
|  | useRegularExpression | boolean | El valor que indica si se utiliza una expresión regular. |
|
|  | searchByPages | boolean | El valor que indica si la búsqueda se realiza por páginas. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Inicializa una nueva instancia de la clase [SearchOptions](../../com.groupdocs.parser.options/searchoptions) con valores predeterminados. Consulte las observaciones para más detalles.

Las siguientes propiedades tienen valores predeterminados:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Obtiene el valor que indica si no se ignora la distinción de mayúsculas y minúsculas del texto.


**Returns:**
boolean -  true  si una distinción de mayúsculas y minúsculas no se ignora; de lo contrario,  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Obtiene el valor que indica si la búsqueda de texto está limitada a una palabra completa.


**Returns:**
boolean -  true  si la búsqueda de texto está limitada a una palabra completa; de lo contrario,  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Obtiene el valor que indica si se utiliza una expresión regular.


**Returns:**
boolean -  true  si se utiliza una expresión regular; de lo contrario,  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Obtiene el valor que indica si la búsqueda se realiza por páginas.


**Returns:**
boolean -  true  si la búsqueda se realiza por páginas; de lo contrario,  false  y la búsqueda se realiza en todo el documento sin incluir el valor de la propiedad [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) en la clase [SearchResult](../../com.groupdocs.parser.data/searchresult).

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Obtiene las opciones para el resaltado izquierdo.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Obtiene las opciones para el resaltado derecho.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Obtiene el valor que representa el índice máximo de la página a buscar.


**Returns:**
int - Un valor entero que representa el índice máximo de la página a buscar; -1 si no está establecido;

