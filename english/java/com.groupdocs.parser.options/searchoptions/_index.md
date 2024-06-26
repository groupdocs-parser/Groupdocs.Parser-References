---
title: SearchOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for text search.
type: docs
weight: 35
url: /java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Provides the options which are used for text search.

An instance of [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class is used as parameter in [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser\#search-String--SearchOptions-) method. See the usage examples there.

**Learn more:**

 *  [Search text][]
 *  [Search text in Microsoft Office Word documents][]
 *  [Search text in Microsoft Office Excel spreadsheets][]
 *  [Search text in Microsoft Office PowerPoint presentations][]
 *  [Search text in PDF documents][]
 *  [Search text in Emails][]
 *  [Search text in EPUB eBooks][]
 *  [Search text in HTML documents][]
 *  [Search text in Microsoft OneNote sections][]


[Search text]: https://docs.groupdocs.com/display/parserjava/Search+text
[Search text in Microsoft Office Word documents]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Word+documents
[Search text in Microsoft Office Excel spreadsheets]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+Excel+spreadsheets
[Search text in Microsoft Office PowerPoint presentations]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+Office+PowerPoint+presentations
[Search text in PDF documents]: https://docs.groupdocs.com/display/parserjava/Search+text+in+PDF+documents
[Search text in Emails]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Emails
[Search text in EPUB eBooks]: https://docs.groupdocs.com/display/parserjava/Search+text+in+EPUB+eBooks
[Search text in HTML documents]: https://docs.groupdocs.com/display/parserjava/Search+text+in+HTML+documents
[Search text in Microsoft OneNote sections]: https://docs.groupdocs.com/display/parserjava/Search+text+in+Microsoft+OneNote+sections
## Constructors

| Constructor | Description |
| --- | --- |
| [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class. |
| [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class which is used to search with the highlight options for the left and the right highlight extraction. |
| [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class which is used to search with the same highlight options for the left and the right highlight extraction. |
| [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class which is used to search without highlight extraction. |
| [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class which is used to search by pages and without highlight extraction. |
| [SearchOptions()](#SearchOptions--) | Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class with default values. |
## Methods

| Method | Description |
| --- | --- |
| [isMatchCase()](#isMatchCase--) | Gets the value that indicates whether a text case isn't ignored. |
| [isMatchWholeWord()](#isMatchWholeWord--) | Gets the value that indicates whether text search is limited by a whole word. |
| [isUseRegularExpression()](#isUseRegularExpression--) | Gets the value that indicates whether a regular expression is used. |
| [isSearchByPages()](#isSearchByPages--) | Gets the value that indicates whether the search is performed by pages. |
| [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Gets the options for the left highlight. |
| [getRightHighlightOptions()](#getRightHighlightOptions--) | Gets the options for the right highlight. |
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | boolean | The value that indicates whether a regular expression is used. |
| searchByPages | boolean | The value that indicates whether the search is performed by pages. |
| leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | The options for the left highlight. |
| rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | The options for the right highlight. |

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class which is used to search with the highlight options for the left and the right highlight extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | boolean | The value that indicates whether a regular expression is used. |
| leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | The options for the left highlight. |
| rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | The options for the right highlight. |

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class which is used to search with the same highlight options for the left and the right highlight extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | boolean | The value that indicates whether a regular expression is used. |
| highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | The options for both highlights. |

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class which is used to search without highlight extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | boolean | The value that indicates whether a regular expression is used. |

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class which is used to search by pages and without highlight extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | boolean | The value that indicates whether a regular expression is used. |
| searchByPages | boolean | The value that indicates whether the search is performed by pages. |

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initializes a new instance of the [SearchOptions](../../com.groupdocs.parser.options/searchoptions) class with default values. See remarks for details.

The following properties have default values:

 *  MatchCase:  false 
 *  MatchWholeWord:  false 
 *  UseRegularExpression:  false 
 *  LeftHighlightOptions:  null 
 *  RightHighlightOptions:  null 

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Gets the value that indicates whether a text case isn't ignored.

**Returns:**
boolean -  true  if a text case isn't ignored; otherwise,  false .
### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Gets the value that indicates whether text search is limited by a whole word.

**Returns:**
boolean -  true  if text search is limited by a whole word; otherwise,  false .
### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Gets the value that indicates whether a regular expression is used.

**Returns:**
boolean -  true  if a regular expression is used; otherwise,  false .
### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Gets the value that indicates whether the search is performed by pages.

**Returns:**
boolean -  true  if the search is performed by pages; otherwise,  false  and the search is performed on the whole document without including [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult\#getPageIndex--) property value in [SearchResult](../../com.groupdocs.parser.data/searchresult) class.
### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Gets the options for the left highlight.

**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.
### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Gets the options for the right highlight.

**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.
