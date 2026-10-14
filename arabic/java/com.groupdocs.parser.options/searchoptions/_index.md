---
title: "SearchOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة للبحث النصي."
type: docs
weight: 35
url: /ar/java/com.groupdocs.parser.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

يوفر الخيارات المستخدمة للبحث النصي.

يُستخدم مثيل من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) كمعامل في طريقة [Parser.search(String, SearchOptions)](../../com.groupdocs.parser/parser#search-String--SearchOptions-).
انظر أمثلة الاستخدام هناك.

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

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions). |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-) | يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) الذي يُستخدم للبحث مع خيارات التمييز لاستخراج التمييز الأيسر والأيمن. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)](#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-) | يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) الذي يُستخدم للبحث مع نفس خيارات التمييز لاستخراج التمييز الأيسر والأيمن. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)](#SearchOptions-boolean-boolean-boolean-) | يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) الذي يُستخدم للبحث دون استخراج التمييز. |
|
|  | [SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)](#SearchOptions-boolean-boolean-boolean-boolean-) | يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) الذي يُستخدم للبحث حسب الصفحات ودون استخراج التمييز. |
|
|  | [SearchOptions()](#SearchOptions--) | يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) بالقيم الافتراضية. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [isMatchCase()](#isMatchCase--) | يحصل على القيمة التي تشير إلى ما إذا كانت حالة النص غير متجاهلة. |
|
|  | [isMatchWholeWord()](#isMatchWholeWord--) | يحصل على القيمة التي تشير إلى ما إذا كان البحث النصي مقيدًا بكلمة كاملة. |
|
|  | [isUseRegularExpression()](#isUseRegularExpression--) | يحصل على القيمة التي تشير إلى ما إذا كان يتم استخدام تعبير نمطي. |
|
|  | [isSearchByPages()](#isSearchByPages--) | يحصل على القيمة التي تشير إلى ما إذا كان البحث يتم حسب الصفحات. |
|
|  | [getLeftHighlightOptions()](#getLeftHighlightOptions--) | يحصل على خيارات التمييز الأيسر. |
|
|  | [getRightHighlightOptions()](#getRightHighlightOptions--) | يحصل على خيارات التمييز الأيمن. |
|
|  | [getMaxPageIndex()](#getMaxPageIndex--) | يحصل على القيمة التي تمثل الحد الأقصى لفهرس الصفحة للبحث. |
|
### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | مطابقة الحالة | boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
|
|  | matchWholeWord | boolean | القيمة التي تشير إلى ما إذا كان البحث النصي مقيدًا بكلمة كاملة. |
|
|  | useRegularExpression | boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
|
|  | searchByPages | boolean | القيمة التي تشير إلى ما إذا كان البحث يتم حسب الصفحات. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | الخيارات لتسليط الضوء على اليسار. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | الخيارات لتسليط الضوء على اليمين. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-int-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | مطابقة الحالة | boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
|
|  | matchWholeWord | boolean | القيمة التي تشير إلى ما إذا كان البحث النصي مقيدًا بكلمة كاملة. |
|
|  | useRegularExpression | boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
|
|  | maxPageIndex | int | القيمة التي تمثل الحد الأقصى لفهرس الصفحة للبحث. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | الخيارات لتسليط الضوء على اليسار. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | الخيارات لتسليط الضوء على اليمين. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```


يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) الذي يُستخدم للبحث مع خيارات التمييز لاستخراج التمييز الأيسر والأيمن.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | مطابقة الحالة | boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
|
|  | matchWholeWord | boolean | القيمة التي تشير إلى ما إذا كان البحث النصي مقيدًا بكلمة كاملة. |
|
|  | useRegularExpression | boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
|
|  | leftHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | الخيارات لتسليط الضوء على اليسار. |
|
|  | rightHighlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | الخيارات لتسليط الضوء على اليمين. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions) {#SearchOptions-boolean-boolean-boolean-com.groupdocs.parser.options.HighlightOptions-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, HighlightOptions highlightOptions)
```


يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) الذي يُستخدم للبحث مع نفس خيارات التمييز لاستخراج التمييز الأيسر والأيمن.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | مطابقة الحالة | boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
|
|  | matchWholeWord | boolean | القيمة التي تشير إلى ما إذا كان البحث النصي مقيدًا بكلمة كاملة. |
|
|  | useRegularExpression | boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
|
|  | highlightOptions | [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) | الخيارات لكلا التسلطين. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression) {#SearchOptions-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression)
```


يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) الذي يُستخدم للبحث دون استخراج التمييز.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | مطابقة الحالة | boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
|
|  | matchWholeWord | boolean | القيمة التي تشير إلى ما إذا كان البحث النصي مقيدًا بكلمة كاملة. |
|
|  | useRegularExpression | boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
|

### SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages) {#SearchOptions-boolean-boolean-boolean-boolean-}
```
public SearchOptions(boolean matchCase, boolean matchWholeWord, boolean useRegularExpression, boolean searchByPages)
```


يُنشئ مثيلًا جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) الذي يُستخدم للبحث حسب الصفحات ودون استخراج التمييز.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | مطابقة الحالة | boolean | القيمة التي تشير إلى ما إذا كان تمييز حالة النص غير متجاهل. |
|
|  | matchWholeWord | boolean | القيمة التي تشير إلى ما إذا كان البحث النصي مقيدًا بكلمة كاملة. |
|
|  | useRegularExpression | boolean | القيمة التي تشير إلى ما إذا تم استخدام تعبير نمطي. |
|
|  | searchByPages | boolean | القيمة التي تشير إلى ما إذا كان البحث يتم حسب الصفحات. |
|

### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


ينشئ مثيلاً جديدًا من الفئة [SearchOptions](../../com.groupdocs.parser.options/searchoptions) بالقيم الافتراضية. راجع الملاحظات للحصول على التفاصيل.

الخصائص التالية لها قيم افتراضية:

* MatchCase:  false 
* MatchWholeWord:  false 
* UseRegularExpression:  false 
* LeftHighlightOptions:  null 
* RightHighlightOptions:  null 


### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


يحصل على القيمة التي تشير إلى ما إذا كانت حالة النص غير متجاهلة.


**Returns:**
boolean -  true  إذا لم يتم تجاهل حالة النص؛ وإلا،  false .

### isMatchWholeWord() {#isMatchWholeWord--}
```
public boolean isMatchWholeWord()
```


يحصل على القيمة التي تشير إلى ما إذا كان البحث النصي مقيدًا بكلمة كاملة.


**Returns:**
منطقي - true إذا كان البحث النصي مقيدًا بكلمة كاملة؛ وإلا false.

### isUseRegularExpression() {#isUseRegularExpression--}
```
public boolean isUseRegularExpression()
```


يحصل على القيمة التي تشير إلى ما إذا كان يتم استخدام تعبير نمطي.


**Returns:**
منطقي - true إذا تم استخدام تعبير نمطي؛ وإلا false.

### isSearchByPages() {#isSearchByPages--}
```
public boolean isSearchByPages()
```


يحصل على القيمة التي تشير إلى ما إذا كان البحث يتم حسب الصفحات.


**Returns:**
منطقي - true إذا تم تنفيذ البحث حسب الصفحات؛ وإلا false ويتم تنفيذ البحث على المستند بالكامل دون تضمين قيمة الخاصية [SearchResult.getPageIndex()](../../com.groupdocs.parser.data/searchresult#getPageIndex--) في الفئة [SearchResult](../../com.groupdocs.parser.data/searchresult).

### getLeftHighlightOptions() {#getLeftHighlightOptions--}
```
public HighlightOptions getLeftHighlightOptions()
```


يحصل على خيارات التمييز الأيسر.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getRightHighlightOptions() {#getRightHighlightOptions--}
```
public HighlightOptions getRightHighlightOptions()
```


يحصل على خيارات التمييز الأيمن.


**Returns:**
[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) - An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class;  nill  if it isn't set.

### getMaxPageIndex() {#getMaxPageIndex--}
```
public int getMaxPageIndex()
```


يحصل على القيمة التي تمثل الحد الأقصى لفهرس الصفحة للبحث.


**Returns:**
عدد صحيح - قيمة عددية تمثل الحد الأقصى لفهرس الصفحة للبحث؛ -1 إذا لم يتم تعيينه؛

