---
title: "SearchOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für die Textsuche verwendet werden."
type: docs
weight: 35
url: /de/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Stellt die Optionen bereit, die für die Textsuche verwendet werden.

Eine Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions) wird als Parameter in der Methode [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-) verwendet.
Siehe dort die Anwendungsbeispiele.

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

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions), die zum Suchen mit den Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion verwendet wird. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions), die zum Suchen mit denselben Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion verwendet wird. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions), die zum Suchen ohne Hervorhebungsextraktion verwendet wird. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions), die zum Suchen nach Seiten und ohne Hervorhebungsextraktion verwendet wird. |
|
|  | [SearchOptions()](#SearchOptions--) | Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions) mit Standardwerten. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Liefert den Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Gibt den Wert zurück, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Gibt den Wert zurück, der angibt, ob ein regulärer Ausdruck verwendet wird. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Gibt den Wert zurück, der angibt, ob die Suche nach Seiten durchgeführt wird. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Gibt die Optionen für die linke Hervorhebung zurück. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Gibt die Optionen für die rechte Hervorhebung zurück. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Gibt den Wert zurück, der den maximalen Index der zu durchsuchenden Seite darstellt. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | matchCase | boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | matchWholeWord | boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
|
|  | useRegularExpression | boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
|
|  | searchByPages | boolean | Der Wert, der angibt, ob die Suche nach Seiten durchgeführt wird. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Die Optionen für die linke Hervorhebung. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Die Optionen für die rechte Hervorhebung. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | matchCase | boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | matchWholeWord | boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
|
|  | useRegularExpression | boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
|
|  | maxPageIndex | int | Der Wert, der den maximalen Index der zu durchsuchenden Seite darstellt |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Die Optionen für die linke Hervorhebung. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Die Optionen für die rechte Hervorhebung. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions), die zum Suchen mit den Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | matchCase | boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | matchWholeWord | boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
|
|  | useRegularExpression | boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Die Optionen für die linke Hervorhebung. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Die Optionen für die rechte Hervorhebung. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions), die zum Suchen mit denselben Hervorhebungsoptionen für die linke und rechte Hervorhebungsextraktion verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | matchCase | boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | matchWholeWord | boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
|
|  | useRegularExpression | boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Die Optionen für beide Hervorhebungen. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions), die zum Suchen ohne Hervorhebungsextraktion verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | matchCase | boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | matchWholeWord | boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
|
|  | useRegularExpression | boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Initialisiert eine neue Instanz der Klasse [SearchOptions](../../com.groupdocs.parser.options/searchoptions), die zum Suchen nach Seiten und ohne Hervorhebungsextraktion verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | matchCase | boolean | Der Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird. |
|
|  | matchWholeWord | boolean | Der Wert, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist. |
|
|  | useRegularExpression | boolean | Der Wert, der angibt, ob ein regulärer Ausdruck verwendet wird. |
|
|  | searchByPages | boolean | Der Wert, der angibt, ob die Suche nach Seiten durchgeführt wird. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initialisiert eine neue Instanz der [SearchOptions](../../com.groupdocs.parser.options/searchoptions) Klasse mit Standardwerten. Siehe Anmerkungen für Details.

Die folgenden Eigenschaften haben Standardwerte:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Liefert den Wert, der angibt, ob die Groß-/Kleinschreibung nicht ignoriert wird.


**Returns:**
boolean -  true  wenn die Groß-/Kleinschreibung nicht ignoriert wird; andernfalls  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Gibt den Wert zurück, der angibt, ob die Textsuche auf ein ganzes Wort beschränkt ist.


**Returns:**
boolean -  true  wenn die Textsuche auf ein ganzes Wort beschränkt ist; andernfalls  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Gibt den Wert zurück, der angibt, ob ein regulärer Ausdruck verwendet wird.


**Returns:**
boolean -  true  wenn ein regulärer Ausdruck verwendet wird; andernfalls  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Gibt den Wert zurück, der angibt, ob die Suche nach Seiten durchgeführt wird.


**Returns:**
boolean -  true  wenn die Suche nach Seiten durchgeführt wird; andernfalls  false  und die Suche wird im gesamten Dokument durchgeführt, ohne den Wert der Eigenschaft [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) in der Klasse [SearchResult](../../com.groupdocs.parser.data/searchresult) einzuschließen.

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Gibt die Optionen für die linke Hervorhebung zurück.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Gibt die Optionen für die rechte Hervorhebung zurück.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Gibt den Wert zurück, der den maximalen Index der zu durchsuchenden Seite darstellt.


**Returns:**
int - Ein ganzzahliger Wert, der den maximalen Index der zu durchsuchenden Seite darstellt; -1, wenn nicht gesetzt;

