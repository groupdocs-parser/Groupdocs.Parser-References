---
title: "SearchOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于文本搜索的选项。"
type: docs
weight: 35
url: /zh/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

提供用于文本搜索的选项。

一个 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类的实例用作 [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-) 方法的参数。
请参阅那里的使用示例。

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

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | 初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | 初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | 初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例，该实例用于使用左侧和右侧高亮提取的高亮选项进行搜索。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | 初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例，该实例用于使用左侧和右侧相同的高亮选项进行搜索。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | 初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例，该实例用于在不进行高亮提取的情况下搜索。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | 初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例，该实例用于按页搜索且不进行高亮提取。 |
|
|  | [SearchOptions()](#SearchOptions--) | 使用默认值初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | 获取指示文本大小写是否未被忽略的值。 |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | 获取指示文本搜索是否受完整单词限制的值。 |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | 获取指示是否使用正则表达式的值。 |
|
|  | [isSearchByPages()](#isSearchByPages--) | 获取指示搜索是否按页执行的值。 |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | 获取左侧高亮的选项。 |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | 获取右侧高亮的选项。 |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | 获取表示要搜索的页面最大索引的值。 |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | matchCase | boolean | 指示文本大小写是否未被忽略的值。 |
|
|  | matchWholeWord | boolean | 指示文本搜索是否受完整单词限制的值。 |
|
|  | useRegularExpression | boolean | 指示是否使用正则表达式的值。 |
|
|  | searchByPages | boolean | 指示搜索是否按页执行的值。 |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 左侧高亮的选项。 |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 右侧高亮的选项。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | matchCase | boolean | 指示文本大小写是否未被忽略的值。 |
|
|  | matchWholeWord | boolean | 指示文本搜索是否受完整单词限制的值。 |
|
|  | useRegularExpression | boolean | 指示是否使用正则表达式的值。 |
|
|  | maxPageIndex | int | 表示要搜索的页面最大索引的值 |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 左侧高亮的选项。 |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 右侧高亮的选项。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例，该实例用于使用左侧和右侧高亮提取的高亮选项进行搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | matchCase | boolean | 指示文本大小写是否未被忽略的值。 |
|
|  | matchWholeWord | boolean | 指示文本搜索是否受完整单词限制的值。 |
|
|  | useRegularExpression | boolean | 指示是否使用正则表达式的值。 |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 左侧高亮的选项。 |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 右侧高亮的选项。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例，该实例用于使用左侧和右侧相同的高亮选项进行搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | matchCase | boolean | 指示文本大小写是否未被忽略的值。 |
|
|  | matchWholeWord | boolean | 指示文本搜索是否受完整单词限制的值。 |
|
|  | useRegularExpression | boolean | 指示是否使用正则表达式的值。 |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 两个高亮的选项。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例，该实例用于在不进行高亮提取的情况下搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | matchCase | boolean | 指示文本大小写是否未被忽略的值。 |
|
|  | matchWholeWord | boolean | 指示文本搜索是否受完整单词限制的值。 |
|
|  | useRegularExpression | boolean | 指示是否使用正则表达式的值。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例，该实例用于按页搜索且不进行高亮提取。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | matchCase | boolean | 指示文本大小写是否未被忽略的值。 |
|
|  | matchWholeWord | boolean | 指示文本搜索是否受完整单词限制的值。 |
|
|  | useRegularExpression | boolean | 指示是否使用正则表达式的值。 |
|
|  | searchByPages | boolean | 指示搜索是否按页执行的值。 |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


使用默认值初始化一个新的 [SearchOptions](../../com.groupdocs.parser.options/searchoptions) 类实例。有关详细信息，请参阅备注。

以下属性具有默认值：

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


获取指示文本大小写是否未被忽略的值。


**Returns:**
boolean -  true  如果文本大小写未被忽略；否则，  false 。

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


获取指示文本搜索是否受完整单词限制的值。


**Returns:**
boolean -  true  如果文本搜索受完整单词限制；否则，  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


获取指示是否使用正则表达式的值。


**Returns:**
boolean -  true  如果使用正则表达式；否则，  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


获取指示搜索是否按页执行的值。


**Returns:**
boolean -  true  如果按页执行搜索；否则，  false  并且搜索在整个文档上执行，且不包括 [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) 属性值在 [SearchResult](../../com.groupdocs.parser.data/searchresult) 类中。

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


获取左侧高亮的选项。


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


获取右侧高亮的选项。


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


获取表示要搜索的页面最大索引的值。


**Returns:**
int - 表示要搜索的页面的最大索引的整数值；如果未设置，则为 -1；

