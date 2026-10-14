---
title: "SearchOptions"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "텍스트 검색에 사용되는 옵션을 제공합니다."
type: docs
weight: 35
url: /ko/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

텍스트 검색에 사용되는 옵션을 제공합니다.

인스턴스인 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스가 [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-) 메서드의 매개변수로 사용됩니다.
그곳의 사용 예제를 확인하십시오.

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

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 왼쪽 및 오른쪽 강조 추출을 위한 강조 옵션으로 검색하는 데 사용됩니다. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 왼쪽 및 오른쪽 강조 추출을 위한 동일한 강조 옵션으로 검색하는 데 사용됩니다. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 강조 추출 없이 검색하는 데 사용됩니다. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 페이지별로 검색하고 강조 추출 없이 검색하는 데 사용됩니다. |
|
|  | [SearchOptions()](#SearchOptions--) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 기본값으로 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | 정규식이 사용되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isSearchByPages()](#isSearchByPages--) | 검색이 페이지별로 수행되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | 왼쪽 강조에 대한 옵션을 가져옵니다. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | 오른쪽 강조에 대한 옵션을 가져옵니다. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | 검색할 페이지의 최대 인덱스를 나타내는 값을 가져옵니다. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | matchCase | boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값입니다. |
|
|  | matchWholeWord | boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값. |
|
|  | useRegularExpression | boolean | 정규식이 사용되는지 여부를 나타내는 값. |
|
|  | searchByPages | boolean | 검색이 페이지별로 수행되는지 여부를 나타내는 값. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 왼쪽 강조에 대한 옵션. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 오른쪽 강조에 대한 옵션. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | matchCase | boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값입니다. |
|
|  | matchWholeWord | boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값. |
|
|  | useRegularExpression | boolean | 정규식이 사용되는지 여부를 나타내는 값. |
|
|  | maxPageIndex | int | 검색할 페이지의 최대 인덱스를 나타내는 값 |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 왼쪽 강조에 대한 옵션. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 오른쪽 강조에 대한 옵션. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 왼쪽 및 오른쪽 강조 추출을 위한 강조 옵션으로 검색하는 데 사용됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | matchCase | boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값입니다. |
|
|  | matchWholeWord | boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값. |
|
|  | useRegularExpression | boolean | 정규식이 사용되는지 여부를 나타내는 값. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 왼쪽 강조에 대한 옵션. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 오른쪽 강조에 대한 옵션. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 왼쪽 및 오른쪽 강조 추출을 위한 동일한 강조 옵션으로 검색하는 데 사용됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | matchCase | boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값입니다. |
|
|  | matchWholeWord | boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값. |
|
|  | useRegularExpression | boolean | 정규식이 사용되는지 여부를 나타내는 값. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 양쪽 강조에 대한 옵션. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 강조 추출 없이 검색하는 데 사용됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | matchCase | boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값입니다. |
|
|  | matchWholeWord | boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값. |
|
|  | useRegularExpression | boolean | 정규식이 사용되는지 여부를 나타내는 값. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 페이지별로 검색하고 강조 추출 없이 검색하는 데 사용됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | matchCase | boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값입니다. |
|
|  | matchWholeWord | boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값. |
|
|  | useRegularExpression | boolean | 정규식이 사용되는지 여부를 나타내는 값. |
|
|  | searchByPages | boolean | 검색이 페이지별로 수행되는지 여부를 나타내는 값. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) 클래스의 새 인스턴스를 기본값으로 초기화합니다. 자세한 내용은 주석을 참조하십시오.

다음 속성은 기본값을 가집니다:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 텍스트 대소문자를 무시하지 않으면 true, 그렇지 않으면 false.

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 전체 단어로 텍스트 검색이 제한되는 경우 true; 그렇지 않으면 false.

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


정규식이 사용되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 정규식을 사용하는 경우 true; 그렇지 않으면 false.

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


검색이 페이지별로 수행되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 페이지별로 검색이 수행되는 경우 true; 그렇지 않으면 false이며, [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) 속성 값을 [SearchResult](../../com.groupdocs.parser.data/searchresult) 클래스에 포함하지 않고 전체 문서에서 검색이 수행됩니다.

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


왼쪽 강조에 대한 옵션을 가져옵니다.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


오른쪽 강조에 대한 옵션을 가져옵니다.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


검색할 페이지의 최대 인덱스를 나타내는 값을 가져옵니다.


**Returns:**
int - 검색할 페이지의 최대 인덱스를 나타내는 정수 값; 설정되지 않은 경우 -1;

