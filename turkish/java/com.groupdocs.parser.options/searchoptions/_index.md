---
title: "SearchOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Metin araması için kullanılan seçenekleri sağlar."
type: docs
weight: 35
url: /tr/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Metin araması için kullanılan seçenekleri sağlar.

Bir [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının örneği, [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-) metodunda parametre olarak kullanılır.
Oradaki kullanım örneklerine bakın.

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

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Yeni bir [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfı örneği başlatır. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Yeni bir [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfı örneği başlatır. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | Sol ve sağ vurgulama çıkarımı için vurgulama seçenekleriyle arama yapmak üzere kullanılan [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | Sol ve sağ vurgulama çıkarımı için aynı vurgulama seçenekleriyle arama yapmak üzere kullanılan [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | Vurgulama çıkarımı olmadan arama yapmak üzere kullanılan [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | Sayfalara göre ve vurgulama çıkarımı olmadan arama yapmak üzere kullanılan [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [SearchOptions()](#SearchOptions--) | Varsayılan değerlerle [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | Metin durumunun yoksayılmadığını gösteren değeri alır. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | Metin aramasının tam kelimeyle sınırlı olup olmadığını gösteren değeri alır. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | Düzenli ifadelerin kullanılıp kullanılmadığını gösteren değeri alır. |
|
|  | [isSearchByPages()](#isSearchByPages--) | Aramanın sayfalara göre yapılıp yapılmadığını gösteren değeri alır. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | Sol vurgulama için seçenekleri alır. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | Sağ vurgulama için seçenekleri alır. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | Aranacak sayfanın maksimum indeksini temsil eden değeri alır. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Yeni bir [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | matchCase | boolean | Metin büyük/küçük harfinin yoksayılmadığını gösteren değer. |
|
|  | matchWholeWord | boolean | Metin aramasının tam kelimeyle sınırlı olup olmadığını gösteren değer. |
|
|  | useRegularExpression | boolean | Düzenli ifadenin kullanılıp kullanılmadığını gösteren değer. |
|
|  | searchByPages | boolean | Aramanın sayfalara göre yapılıp yapılmadığını gösteren değer. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Sol vurgulama için seçenekler. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Sağ vurgulama için seçenekler. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Yeni bir [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | matchCase | boolean | Metin büyük/küçük harfinin yoksayılmadığını gösteren değer. |
|
|  | matchWholeWord | boolean | Metin aramasının tam kelimeyle sınırlı olup olmadığını gösteren değer. |
|
|  | useRegularExpression | boolean | Düzenli ifadenin kullanılıp kullanılmadığını gösteren değer. |
|
|  | maxPageIndex | int | Aranacak sayfanın maksimum indeksini temsil eden değer |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Sol vurgulama için seçenekler. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Sağ vurgulama için seçenekler. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


Sol ve sağ vurgulama çıkarımı için vurgulama seçenekleriyle arama yapmak üzere kullanılan [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | matchCase | boolean | Metin büyük/küçük harfinin yoksayılmadığını gösteren değer. |
|
|  | matchWholeWord | boolean | Metin aramasının tam kelimeyle sınırlı olup olmadığını gösteren değer. |
|
|  | useRegularExpression | boolean | Düzenli ifadenin kullanılıp kullanılmadığını gösteren değer. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Sol vurgulama için seçenekler. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Sağ vurgulama için seçenekler. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


Sol ve sağ vurgulama çıkarımı için aynı vurgulama seçenekleriyle arama yapmak üzere kullanılan [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | matchCase | boolean | Metin büyük/küçük harfinin yoksayılmadığını gösteren değer. |
|
|  | matchWholeWord | boolean | Metin aramasının tam kelimeyle sınırlı olup olmadığını gösteren değer. |
|
|  | useRegularExpression | boolean | Düzenli ifadenin kullanılıp kullanılmadığını gösteren değer. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | Her iki vurgulama için seçenekler. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


Vurgulama çıkarımı olmadan arama yapmak üzere kullanılan [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | matchCase | boolean | Metin büyük/küçük harfinin yoksayılmadığını gösteren değer. |
|
|  | matchWholeWord | boolean | Metin aramasının tam kelimeyle sınırlı olup olmadığını gösteren değer. |
|
|  | useRegularExpression | boolean | Düzenli ifadenin kullanılıp kullanılmadığını gösteren değer. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


Sayfalara göre ve vurgulama çıkarımı olmadan arama yapmak üzere kullanılan [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | matchCase | boolean | Metin büyük/küçük harfinin yoksayılmadığını gösteren değer. |
|
|  | matchWholeWord | boolean | Metin aramasının tam kelimeyle sınırlı olup olmadığını gösteren değer. |
|
|  | useRegularExpression | boolean | Düzenli ifadenin kullanılıp kullanılmadığını gösteren değer. |
|
|  | searchByPages | boolean | Aramanın sayfalara göre yapılıp yapılmadığını gösteren değer. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Varsayılan değerlerle yeni bir [SearchOptions](../../com.groupdocs.parser.options/searchoptions) sınıfı örneği başlatır. Ayrıntılar için açıklamaları inceleyin.

Aşağıdaki özelliklerin varsayılan değerleri vardır:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Metin durumunun yoksayılmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin büyük/küçük harfi yoksayılmıyorsa; aksi takdirde,  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


Metin aramasının tam kelimeyle sınırlı olup olmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer metin araması tam kelimeyle sınırlıysa; aksi takdirde,  false .

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


Düzenli ifadelerin kullanılıp kullanılmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer düzenli ifade kullanılıyorsa; aksi takdirde,  false .

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


Aramanın sayfalara göre yapılıp yapılmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer arama sayfalara göre yapılırsa; aksi takdirde,  false  ve arama, [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) özelliği değerini [SearchResult](../../com.groupdocs.parser.data/searchresult) sınıfına dahil etmeden tüm belge üzerinde yapılır.

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


Sol vurgulama için seçenekleri alır.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


Sağ vurgulama için seçenekleri alır.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


Aranacak sayfanın maksimum indeksini temsil eden değeri alır.


**Returns:**
int - Aranacak sayfanın maksimum indeksini temsil eden bir tam sayı değeri; ayarlanmamışsa -1;

