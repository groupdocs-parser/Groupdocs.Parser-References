---
title: HighlightOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used to extract a highlight a block of text aroud found text in search scenarios.
type: docs
weight: 22
url: /java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Provides the options which are used to extract a highlight (a block of text aroud found text in search scenarios).

An instance of [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class is used as parameter in [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser\#getHighlight-int--boolean--HighlightOptions-) method. See the usage examples there.

**Learn more:**

 *  [Extract highlights][]


[Extract highlights]: https://docs.groupdocs.com/display/parserjava/Extract+highlights
## Constructors

| Constructor | Description |
| --- | --- |
| [HighlightOptions()](#HighlightOptions--) | Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class with no limits set. |
| [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class which is used to extract a fixed-length highlight. |
| [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class which is used to extract a line-limited highlight. |
| [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class which is used to extract a highlight with the fixed word count. |
| [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getMaxLength()](#getMaxLength--) | Gets a maximum text length. |
| [getWordCount()](#getWordCount--) | Gets a maximum word count. |
| [isLineLimited()](#isLineLimited--) | Gets value that indicates whether highlight extraction is limited by the start (or the end) of a text line. |
| [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Sets a maximum text length. |
| [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Sets a maximum word count. |
| [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Sets the value that indicates whether highlight extraction is limited by the start (or the end) of a text line. |
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class with no limits set. Set at least one of \#setMaxLength(Integer).setMaxLength(Integer), \#setWordCount(Integer).setWordCount(Integer), \#setLineLimited(boolean).setLineLimited(boolean) before passing to the parser.

### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class which is used to extract a fixed-length highlight.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxLength | int | The maximum text length. |

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class which is used to extract a line-limited highlight.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxLength | java.lang.Integer | The maximum text length. |
| isLineLimited | boolean | The value that indicates whether the highlight extraction is limited by the start (or the end) of a text line. |

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class which is used to extract a highlight with the fixed word count.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxLength | java.lang.Integer | The maximum text length. |
| wordCount | int | The maximum word count. |

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Initializes a new instance of the [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxLength | java.lang.Integer | The maximum text length. |
| wordCount | java.lang.Integer | The maximum word count. |
| isLineLimited | boolean | The value that indicates whether the highlight extraction is limited by the start (or the end) of a text line. |

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Gets a maximum text length.

**Returns:**
java.lang.Integer - A positive integer value that represents the maximum text length;  null  if the text length isn't limited.
### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Gets a maximum word count.

**Returns:**
java.lang.Integer - A positive integer value that represents the maximum word count;  null  if the word count isn't limited.
### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Gets value that indicates whether highlight extraction is limited by the start (or the end) of a text line.

**Returns:**
boolean -  true  if highlight extraction is limited by the start (or the end) of a text line; otherwise,  false .
### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Sets a maximum text length.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxLength | java.lang.Integer | A non-negative integer;  null  to remove the length limit. |

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Sets a maximum word count.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| wordCount | java.lang.Integer | A non-negative integer;  null  to remove the word-count limit. |

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Sets the value that indicates whether highlight extraction is limited by the start (or the end) of a text line.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| lineLimited | boolean |  true  to limit by line bounds. |

