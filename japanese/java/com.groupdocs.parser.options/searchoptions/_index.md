---
title: "SearchOptions"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "テキスト検索に使用されるオプションを提供します。"
type: docs
weight: 35
url: /ja/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

テキスト検索に使用されるオプションを提供します。

インスタンス [SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスは、[Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-) メソッドのパラメータとして使用されます。
そこにある使用例をご覧ください。

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

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。このインスタンスは、左側と右側のハイライト抽出のハイライトオプションを使用して検索するために使用されます。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。このインスタンスは、左側と右側のハイライト抽出に同じハイライトオプションを使用して検索するために使用されます。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。このインスタンスは、ハイライト抽出なしで検索するために使用されます。 |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。このインスタンスは、ページ単位で検索し、ハイライト抽出なしで検索するために使用されます。 |
|
|  | [SearchOptions()](#SearchOptions--) | [SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスをデフォルト値で初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | テキストの大文字小文字が無視されないかどうかを示す値を取得します。 |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | テキスト検索が単語全体で制限されているかどうかを示す値を取得します。 |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | 正規表現が使用されているかどうかを示す値を取得します。 |
|
|  | [isSearchByPages()](#isSearchByPages--) | 検索がページ単位で実行されるかどうかを示す値を取得します。 |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | 左側ハイライトのオプションを取得します。 |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | 右側ハイライトのオプションを取得します。 |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | 検索対象ページの最大インデックスを表す値を取得します。 |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | matchCase | boolean | テキストの大文字小文字が無視されないかどうかを示す値です。 |
|
|  | matchWholeWord | boolean | テキスト検索が単語全体で制限されているかどうかを示す値です。 |
|
|  | useRegularExpression | boolean | 正規表現が使用されているかどうかを示す値です。 |
|
|  | searchByPages | boolean | 検索がページ単位で実行されるかどうかを示す値です。 |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 左側ハイライトのオプションです。 |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 右側ハイライトのオプションです。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | matchCase | boolean | テキストの大文字小文字が無視されないかどうかを示す値です。 |
|
|  | matchWholeWord | boolean | テキスト検索が単語全体で制限されているかどうかを示す値です。 |
|
|  | useRegularExpression | boolean | 正規表現が使用されているかどうかを示す値です。 |
|
|  | maxPageIndex | int | 検索対象ページの最大インデックスを表す値です |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 左側ハイライトのオプションです。 |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 右側ハイライトのオプションです。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。このインスタンスは、左側と右側のハイライト抽出のハイライトオプションを使用して検索するために使用されます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | matchCase | boolean | テキストの大文字小文字が無視されないかどうかを示す値です。 |
|
|  | matchWholeWord | boolean | テキスト検索が単語全体で制限されているかどうかを示す値です。 |
|
|  | useRegularExpression | boolean | 正規表現が使用されているかどうかを示す値です。 |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 左側ハイライトのオプションです。 |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 右側ハイライトのオプションです。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。このインスタンスは、左側と右側のハイライト抽出に同じハイライトオプションを使用して検索するために使用されます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | matchCase | boolean | テキストの大文字小文字が無視されないかどうかを示す値です。 |
|
|  | matchWholeWord | boolean | テキスト検索が単語全体で制限されているかどうかを示す値です。 |
|
|  | useRegularExpression | boolean | 正規表現が使用されているかどうかを示す値です。 |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | 両方のハイライトのオプションです。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。このインスタンスは、ハイライト抽出なしで検索するために使用されます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | matchCase | boolean | テキストの大文字小文字が無視されないかどうかを示す値です。 |
|
|  | matchWholeWord | boolean | テキスト検索が単語全体で制限されているかどうかを示す値です。 |
|
|  | useRegularExpression | boolean | 正規表現が使用されているかどうかを示す値です。 |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


[SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。このインスタンスは、ページ単位で検索し、ハイライト抽出なしで検索するために使用されます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | matchCase | boolean | テキストの大文字小文字が無視されないかどうかを示す値です。 |
|
|  | matchWholeWord | boolean | テキスト検索が単語全体で制限されているかどうかを示す値です。 |
|
|  | useRegularExpression | boolean | 正規表現が使用されているかどうかを示す値です。 |
|
|  | searchByPages | boolean | 検索がページ単位で実行されるかどうかを示す値です。 |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


デフォルト値で [SearchOptions](../../com.groupdocs.parser.options/searchoptions) クラスの新しいインスタンスを初期化します。詳細は備考をご覧ください。

以下のプロパティはデフォルト値を持ちます：

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


テキストの大文字小文字が無視されないかどうかを示す値を取得します。


**Returns:**
boolean -  true  テキストケースが無視されていない場合; それ以外は  false です。

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


テキスト検索が単語全体で制限されているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if テキスト検索が単語全体で制限される場合; それ以外の場合は false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


正規表現が使用されているかどうかを示す値を取得します。


**Returns:**
boolean -  true  if 正規表現が使用される場合; それ以外の場合は false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


検索がページ単位で実行されるかどうかを示す値を取得します。


**Returns:**
boolean -  true  if 検索がページ単位で実行される場合; それ以外の場合は false で、検索は [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) プロパティ値を含めずに、[SearchResult](../../com.groupdocs.parser.data/searchresult) クラス全体で実行されます。

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


左側ハイライトのオプションを取得します。


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


右側ハイライトのオプションを取得します。


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


検索対象ページの最大インデックスを表す値を取得します。


**Returns:**
int - ページ検索の最大インデックスを表す整数値です; 設定されていない場合は -1;

