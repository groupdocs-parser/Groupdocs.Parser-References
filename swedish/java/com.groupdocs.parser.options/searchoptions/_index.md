---
title: "SearchOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för textsökning."
type: docs
weight: 35
url: /sv/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Tillhandahåller de alternativ som används för textsökning.

En instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klass används som parameter i [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-) metoden.
Se användningsexemplen där.

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

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen som används för att söka med markeringsalternativen för vänster och höger markeringsextraktion. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen som används för att söka med samma markeringsalternativ för vänster och höger markeringsextraktion. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen som används för att söka utan markeringsextraktion. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen som används för att söka per sidor och utan markeringsextraktion. |
|
|  | [SearchOptions()](#SearchOptions--) | Initierar en ny instans av klassen [SearchOptions](../../com.groupdocs.parser.options/searchoptions) med standardvärden. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Hämtar värdet som indikerar om ett textfall inte ignoreras. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Hämtar värdet som indikerar om textsökning är begränsad till ett helt ord. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Hämtar värdet som indikerar om ett reguljärt uttryck används. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Hämtar värdet som indikerar om sökningen utförs per sida. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Hämtar alternativen för den vänstra markeringen. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Hämtar alternativen för den högra markeringen. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Hämtar värdet som representerar det maximala sidindexet att söka. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | matchCase | boolean | Värdet som indikerar om skiftläge i texten inte ignoreras. |
|
|  | matchWholeWord | boolean | Värdet som indikerar om textsökning är begränsad till ett helt ord. |
|
|  | useRegularExpression | boolean | Värdet som indikerar om ett reguljärt uttryck används. |
|
|  | searchByPages | boolean | Värdet som indikerar om sökningen utförs per sida. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Alternativen för den vänstra markeringen. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Alternativen för den högra markeringen. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | matchCase | boolean | Värdet som indikerar om skiftläge i texten inte ignoreras. |
|
|  | matchWholeWord | boolean | Värdet som indikerar om textsökning är begränsad till ett helt ord. |
|
|  | useRegularExpression | boolean | Värdet som indikerar om ett reguljärt uttryck används. |
|
|  | maxPageIndex | int | Värdet som representerar det maximala sidindexet att söka |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Alternativen för den vänstra markeringen. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Alternativen för den högra markeringen. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen som används för att söka med markeringsalternativen för vänster och höger markeringsextraktion.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | matchCase | boolean | Värdet som indikerar om skiftläge i texten inte ignoreras. |
|
|  | matchWholeWord | boolean | Värdet som indikerar om textsökning är begränsad till ett helt ord. |
|
|  | useRegularExpression | boolean | Värdet som indikerar om ett reguljärt uttryck används. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Alternativen för den vänstra markeringen. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Alternativen för den högra markeringen. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen som används för att söka med samma markeringsalternativ för vänster och höger markeringsextraktion.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | matchCase | boolean | Värdet som indikerar om skiftläge i texten inte ignoreras. |
|
|  | matchWholeWord | boolean | Värdet som indikerar om textsökning är begränsad till ett helt ord. |
|
|  | useRegularExpression | boolean | Värdet som indikerar om ett reguljärt uttryck används. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Alternativen för båda markeringarna. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen som används för att söka utan markeringsextraktion.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | matchCase | boolean | Värdet som indikerar om skiftläge i texten inte ignoreras. |
|
|  | matchWholeWord | boolean | Värdet som indikerar om textsökning är begränsad till ett helt ord. |
|
|  | useRegularExpression | boolean | Värdet som indikerar om ett reguljärt uttryck används. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Initierar en ny instans av [SearchOptions](../../com.groupdocs.parser.options/searchoptions) klassen som används för att söka per sidor och utan markeringsextraktion.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | matchCase | boolean | Värdet som indikerar om skiftläge i texten inte ignoreras. |
|
|  | matchWholeWord | boolean | Värdet som indikerar om textsökning är begränsad till ett helt ord. |
|
|  | useRegularExpression | boolean | Värdet som indikerar om ett reguljärt uttryck används. |
|
|  | searchByPages | boolean | Värdet som indikerar om sökningen utförs per sida. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initierar en ny instans av klassen [SearchOptions](../../com.groupdocs.parser.options/searchoptions) med standardvärden. Se kommentarer för detaljer.

Följande egenskaper har standardvärden:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Hämtar värdet som indikerar om ett textfall inte ignoreras.


**Returns:**
boolean -  true  om skiftläge i texten inte ignoreras; annars,  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Hämtar värdet som indikerar om textsökning är begränsad till ett helt ord.


**Returns:**
boolean -  true  om textsökning är begränsad till ett helt ord; annars  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Hämtar värdet som indikerar om ett reguljärt uttryck används.


**Returns:**
boolean -  true  om ett reguljärt uttryck används; annars  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Hämtar värdet som indikerar om sökningen utförs per sida.


**Returns:**
boolean -  true  om sökningen utförs per sida; annars  false  och sökningen utförs på hela dokumentet utan att inkludera egenskapsvärdet [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) i klassen [SearchResult](../../com.groupdocs.parser.data/searchresult).

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Hämtar alternativen för den vänstra markeringen.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Hämtar alternativen för den högra markeringen.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Hämtar värdet som representerar det maximala sidindexet att söka.


**Returns:**
int - Ett heltalsvärde som representerar det maximala sidindexet att söka; -1 om det inte är satt;

