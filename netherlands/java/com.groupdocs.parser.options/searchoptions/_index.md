---
title: "SearchOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor tekst zoeken."
type: docs
weight: 35
url: /nl/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Biedt de opties die worden gebruikt voor tekst zoeken.

Een exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse wordt gebruikt als parameter in de methode [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-).
Zie daar de gebruiksvoorbeelden.

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

| Constructor | Beschrijving |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse die wordt gebruikt om te zoeken met de markeeropties voor de linker- en rechtermarkeringsextractie. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse die wordt gebruikt om te zoeken met dezelfde markeeropties voor de linker- en rechtermarkeringsextractie. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse die wordt gebruikt om te zoeken zonder markeringsextractie. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse die wordt gebruikt om per pagina te zoeken en zonder markeringsextractie. |
|
|  | [SearchOptions()](#SearchOptions--) | Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse met standaardwaarden. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Haalt de waarde op die aangeeft of hoofdlettergebruik van tekst niet wordt genegeerd. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Haalt de waarde op die aangeeft of tekst zoeken beperkt is tot een heel woord. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Haalt de waarde op die aangeeft of een reguliere expressie wordt gebruikt. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Haalt de waarde op die aangeeft of het zoeken per pagina's wordt uitgevoerd. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Haalt de opties voor de linker markering op. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Haalt de opties voor de rechter markering op. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Haalt de waarde op die de maximale paginapositie voor zoeken weergeeft. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | matchCase | boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
|
|  | matchWholeWord | boolean | De waarde die aangeeft of tekst zoeken wordt beperkt tot een heel woord. |
|
|  | useRegularExpression | boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
|
|  | searchByPages | boolean | De waarde die aangeeft of de zoekopdracht per pagina wordt uitgevoerd. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | De opties voor de linker markering. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | De opties voor de rechter markering. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | matchCase | boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
|
|  | matchWholeWord | boolean | De waarde die aangeeft of tekst zoeken wordt beperkt tot een heel woord. |
|
|  | useRegularExpression | boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
|
|  | maxPageIndex | int | De waarde die de maximale index van de te doorzoeken pagina weergeeft. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | De opties voor de linker markering. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | De opties voor de rechter markering. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse die wordt gebruikt om te zoeken met de markeeropties voor de linker- en rechtermarkeringsextractie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | matchCase | boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
|
|  | matchWholeWord | boolean | De waarde die aangeeft of tekst zoeken wordt beperkt tot een heel woord. |
|
|  | useRegularExpression | boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | De opties voor de linker markering. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | De opties voor de rechter markering. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse die wordt gebruikt om te zoeken met dezelfde markeeropties voor de linker- en rechtermarkeringsextractie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | matchCase | boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
|
|  | matchWholeWord | boolean | De waarde die aangeeft of tekst zoeken wordt beperkt tot een heel woord. |
|
|  | useRegularExpression | boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | De opties voor beide markeringen. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse die wordt gebruikt om te zoeken zonder markeringsextractie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | matchCase | boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
|
|  | matchWholeWord | boolean | De waarde die aangeeft of tekst zoeken wordt beperkt tot een heel woord. |
|
|  | useRegularExpression | boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse die wordt gebruikt om per pagina te zoeken en zonder markeringsextractie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | matchCase | boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
|
|  | matchWholeWord | boolean | De waarde die aangeeft of tekst zoeken wordt beperkt tot een heel woord. |
|
|  | useRegularExpression | boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
|
|  | searchByPages | boolean | De waarde die aangeeft of de zoekopdracht per pagina wordt uitgevoerd. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initialiseert een nieuw exemplaar van de [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klasse met standaardwaarden. Zie opmerkingen voor details.

De volgende eigenschappen hebben standaardwaarden:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Haalt de waarde op die aangeeft of hoofdlettergebruik van tekst niet wordt genegeerd.


**Returns:**
boolean -  true  als een tekstcase niet wordt genegeerd; anders,  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Haalt de waarde op die aangeeft of tekst zoeken beperkt is tot een heel woord.


**Returns:**
boolean -  true  als tekst zoeken wordt beperkt tot een heel woord; anders,  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Haalt de waarde op die aangeeft of een reguliere expressie wordt gebruikt.


**Returns:**
boolean -  true  als een reguliere expressie wordt gebruikt; anders,  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Haalt de waarde op die aangeeft of het zoeken per pagina's wordt uitgevoerd.


**Returns:**
boolean -  true  als de zoekopdracht per pagina wordt uitgevoerd; anders,  false  en wordt de zoekopdracht uitgevoerd op het volledige document zonder de eigenschapswaarde van [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) op te nemen in de [SearchResult](../../com.groupdocs.parser.data/searchresult) klasse.

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Haalt de opties voor de linker markering op.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Haalt de opties voor de rechter markering op.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Haalt de waarde op die de maximale paginapositie voor zoeken weergeeft.


**Returns:**
int - Een gehele getalwaarde die de maximale index van de te doorzoeken pagina weergeeft; -1 indien niet ingesteld;

