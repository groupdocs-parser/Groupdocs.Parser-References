---
title: "SearchOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour la recherche de texte."
type: docs
weight: 35
url: /fr/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Fournit les options utilisées pour la recherche de texte.

Une instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) est utilisée comme paramètre dans la méthode [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-).
Voir les exemples d'utilisation là-bas.

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

## Constructors

| Constructor | Description |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) qui est utilisée pour rechercher avec les options de surlignage pour l’extraction du surlignage gauche et droit. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) qui est utilisée pour rechercher avec les mêmes options de surlignage pour l’extraction du surlignage gauche et droit. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) qui est utilisée pour rechercher sans extraction de surlignage. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) qui est utilisée pour rechercher par pages et sans extraction de surlignage. |
|
|  | [SearchOptions()](#SearchOptions--) | Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) avec les valeurs par défaut. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Obtient la valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Obtient la valeur indiquant si la recherche de texte est limitée à un mot entier. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Obtient la valeur qui indique si une expression régulière est utilisée. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Obtient la valeur qui indique si la recherche est effectuée par pages. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Obtient les options pour la mise en surbrillance gauche. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Obtient les options pour la mise en surbrillance droite. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Obtient la valeur qui représente l'index maximal de la page à rechercher. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | matchCase | boolean | La valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | matchWholeWord | boolean | La valeur qui indique si la recherche de texte est limitée à un mot entier. |
|
|  | useRegularExpression | boolean | La valeur qui indique si une expression régulière est utilisée. |
|
|  | searchByPages | boolean | La valeur qui indique si la recherche est effectuée par pages. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Les options pour la mise en surbrillance gauche. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Les options pour la mise en surbrillance droite. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | matchCase | boolean | La valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | matchWholeWord | boolean | La valeur qui indique si la recherche de texte est limitée à un mot entier. |
|
|  | useRegularExpression | boolean | La valeur qui indique si une expression régulière est utilisée. |
|
|  | maxPageIndex | int | La valeur qui représente l'index maximal de la page à rechercher |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Les options pour la mise en surbrillance gauche. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Les options pour la mise en surbrillance droite. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) qui est utilisée pour rechercher avec les options de surlignage pour l’extraction du surlignage gauche et droit.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | matchCase | boolean | La valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | matchWholeWord | boolean | La valeur qui indique si la recherche de texte est limitée à un mot entier. |
|
|  | useRegularExpression | boolean | La valeur qui indique si une expression régulière est utilisée. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Les options pour la mise en surbrillance gauche. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Les options pour la mise en surbrillance droite. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) qui est utilisée pour rechercher avec les mêmes options de surlignage pour l’extraction du surlignage gauche et droit.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | matchCase | boolean | La valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | matchWholeWord | boolean | La valeur qui indique si la recherche de texte est limitée à un mot entier. |
|
|  | useRegularExpression | boolean | La valeur qui indique si une expression régulière est utilisée. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Les options pour les deux mises en surbrillance. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) qui est utilisée pour rechercher sans extraction de surlignage.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | matchCase | boolean | La valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | matchWholeWord | boolean | La valeur qui indique si la recherche de texte est limitée à un mot entier. |
|
|  | useRegularExpression | boolean | La valeur qui indique si une expression régulière est utilisée. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) qui est utilisée pour rechercher par pages et sans extraction de surlignage.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | matchCase | boolean | La valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | matchWholeWord | boolean | La valeur qui indique si la recherche de texte est limitée à un mot entier. |
|
|  | useRegularExpression | boolean | La valeur qui indique si une expression régulière est utilisée. |
|
|  | searchByPages | boolean | La valeur qui indique si la recherche est effectuée par pages. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initialise une nouvelle instance de la classe [SearchOptions](../../com.groupdocs.parser.options/searchoptions) avec les valeurs par défaut. Voir les remarques pour plus de détails.

Les propriétés suivantes ont des valeurs par défaut :

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Obtient la valeur qui indique si la casse du texte n'est pas ignorée.


**Returns:**
boolean -  true  si la casse du texte n'est pas ignorée ; sinon,  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Obtient la valeur indiquant si la recherche de texte est limitée à un mot entier.


**Returns:**
boolean -  true  si la recherche de texte est limitée à un mot entier ; sinon,  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Obtient la valeur qui indique si une expression régulière est utilisée.


**Returns:**
boolean -  true  si une expression régulière est utilisée ; sinon,  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Obtient la valeur qui indique si la recherche est effectuée par pages.


**Returns:**
boolean -  true  si la recherche est effectuée par pages ; sinon,  false  et la recherche est effectuée sur l'ensemble du document sans inclure la valeur de la propriété [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) dans la classe [SearchResult](../../com.groupdocs.parser.data/searchresult).

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Obtient les options pour la mise en surbrillance gauche.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Obtient les options pour la mise en surbrillance droite.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Obtient la valeur qui représente l'index maximal de la page à rechercher.


**Returns:**
int - Une valeur entière qui représente l'index maximal de la page à rechercher ; -1 si non définie ;

