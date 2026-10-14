---
title: "SearchOptions"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет параметры, используемые для поиска текста."
type: docs
weight: 35
url: /ru/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Предоставляет параметры, используемые для поиска текста.

Экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions) используется в качестве параметра в методе [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-).
Смотрите примеры использования там.

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

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions), который используется для поиска с параметрами подсветки левой и правой подсветки. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions), который используется для поиска с одинаковыми параметрами подсветки левой и правой подсветки. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions), который используется для поиска без подсветки. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions), который используется для поиска по страницам и без подсветки. |
|
|  | [SearchOptions()](#SearchOptions--) | Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions) со значениями по умолчанию. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Возвращает значение, что регистр текста не игнорируется. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Получает значение, указывающее, ограничен ли поиск текста целым словом. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Получает значение, указывающее, используется ли регулярное выражение. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Получает значение, указывающее, выполняется ли поиск по страницам. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Получает параметры для левой подсветки. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Получает параметры для правой подсветки. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Получает значение, представляющее максимальный индекс страницы для поиска. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | matchCase | boolean | Значение, указывающее, не игнорируется ли регистр текста. |
|
|  | matchWholeWord | boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
|
|  | useRegularExpression | boolean | Значение, указывающее, используется ли регулярное выражение. |
|
|  | searchByPages | boolean | Значение, указывающее, выполняется ли поиск по страницам. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Параметры для выделения слева. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Параметры для выделения справа. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | matchCase | boolean | Значение, указывающее, не игнорируется ли регистр текста. |
|
|  | matchWholeWord | boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
|
|  | useRegularExpression | boolean | Значение, указывающее, используется ли регулярное выражение. |
|
|  | maxPageIndex | int | Значение, представляющее максимальный индекс страницы для поиска |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Параметры для выделения слева. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Параметры для выделения справа. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions), который используется для поиска с параметрами подсветки левой и правой подсветки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | matchCase | boolean | Значение, указывающее, не игнорируется ли регистр текста. |
|
|  | matchWholeWord | boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
|
|  | useRegularExpression | boolean | Значение, указывающее, используется ли регулярное выражение. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Параметры для выделения слева. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Параметры для выделения справа. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions), который используется для поиска с одинаковыми параметрами подсветки левой и правой подсветки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | matchCase | boolean | Значение, указывающее, не игнорируется ли регистр текста. |
|
|  | matchWholeWord | boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
|
|  | useRegularExpression | boolean | Значение, указывающее, используется ли регулярное выражение. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Параметры для обоих выделений. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions), который используется для поиска без подсветки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | matchCase | boolean | Значение, указывающее, не игнорируется ли регистр текста. |
|
|  | matchWholeWord | boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
|
|  | useRegularExpression | boolean | Значение, указывающее, используется ли регулярное выражение. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions), который используется для поиска по страницам и без подсветки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | matchCase | boolean | Значение, указывающее, не игнорируется ли регистр текста. |
|
|  | matchWholeWord | boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
|
|  | useRegularExpression | boolean | Значение, указывающее, используется ли регулярное выражение. |
|
|  | searchByPages | boolean | Значение, указывающее, выполняется ли поиск по страницам. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Инициализирует новый экземпляр класса [SearchOptions](../../com.groupdocs.parser.options/searchoptions) с значениями по умолчанию. См. примечания для подробностей.

Следующие свойства имеют значения по умолчанию:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Возвращает значение, что регистр текста не игнорируется.


**Returns:**
boolean — true, если регистр текста не игнорируется; иначе false.

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Получает значение, указывающее, ограничен ли поиск текста целым словом.


**Returns:**
boolean —  true  если поиск текста ограничен целым словом; иначе  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Получает значение, указывающее, используется ли регулярное выражение.


**Returns:**
boolean —  true  если используется регулярное выражение; иначе  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Получает значение, указывающее, выполняется ли поиск по страницам.


**Returns:**
boolean —  true  если поиск выполняется по страницам; иначе  false  и поиск выполняется по всему документу без включения значения свойства [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) в класс [SearchResult](../../com.groupdocs.parser.data/searchresult).

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Получает параметры для левой подсветки.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Получает параметры для правой подсветки.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Получает значение, представляющее максимальный индекс страницы для поиска.


**Returns:**
int — Целочисленное значение, представляющее максимальный индекс страницы для поиска; -1, если не установлено;

