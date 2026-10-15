---
title: "SearchOptions"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "初始化 SearchOptionsgroupdocs.parser.options/searchoptions 类的新实例。"
type: docs
weight: 10
url: /zh/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

初始化 [`SearchOptions`](../../searchoptions) 类的新实例。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| matchCase | Boolean | 指示文本大小写是否未被忽略的值。 |
| matchWholeWord | Boolean | 指示文本搜索是否受完整单词限制的值。 |
| useRegularExpression | Boolean | 指示是否使用正则表达式的值。 |
| searchByPages | Boolean | 指示搜索是否按页进行的值。 |
| leftHighlightOptions | HighlightOptions | 左侧高亮的选项。 |
| rightHighlightOptions | HighlightOptions | 右侧高亮的选项。 |

### 另请参见

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

使用页面限制初始化 [`SearchOptions`](../../searchoptions) 类的新实例。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| matchCase | Boolean | 指示文本大小写是否未被忽略的值。 |
| matchWholeWord | Boolean | 指示文本搜索是否受完整单词限制的值。 |
| useRegularExpression | Boolean | 指示是否使用正则表达式的值。 |
| maxPageIndex | Int32 | 指示搜索是否按页面执行的值。 |
| leftHighlightOptions | HighlightOptions | 左侧高亮的选项。 |
| rightHighlightOptions | HighlightOptions | 右侧高亮的选项。 |

### 另请参见

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

初始化一个新的 [`SearchOptions`](../../searchoptions) 类实例，该实例用于使用左侧和右侧高亮提取的高亮选项进行搜索。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| matchCase | Boolean | 指示文本大小写是否未被忽略的值。 |
| matchWholeWord | Boolean | 指示文本搜索是否受完整单词限制的值。 |
| useRegularExpression | Boolean | 指示是否使用正则表达式的值。 |
| leftHighlightOptions | HighlightOptions | 左侧高亮的选项。 |
| rightHighlightOptions | HighlightOptions | 右侧高亮的选项。 |

### 另请参见

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

初始化一个新的 [`SearchOptions`](../../searchoptions) 类实例，该实例用于使用左侧和右侧相同的高亮选项进行搜索。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| matchCase | Boolean | 指示文本大小写是否未被忽略的值。 |
| matchWholeWord | Boolean | 指示文本搜索是否受完整单词限制的值。 |
| useRegularExpression | Boolean | 指示是否使用正则表达式的值。 |
| highlightOptions | HighlightOptions | 两个高亮的选项。 |

### 另请参见

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

初始化一个新的 [`SearchOptions`](../../searchoptions) 类实例，该实例用于在不进行高亮提取的情况下搜索。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| matchCase | Boolean | 指示文本大小写是否未被忽略的值。 |
| matchWholeWord | Boolean | 指示文本搜索是否受完整单词限制的值。 |
| useRegularExpression | Boolean | 指示是否使用正则表达式的值。 |

### 另请参见

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

初始化一个新的 [`SearchOptions`](../../searchoptions) 类实例，该实例用于按页面搜索且不进行高亮提取。

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| matchCase | Boolean | 指示文本大小写是否未被忽略的值。 |
| matchWholeWord | Boolean | 指示文本搜索是否受完整单词限制的值。 |
| useRegularExpression | Boolean | 指示是否使用正则表达式的值。 |
| searchByPages | Boolean | 指示搜索是否按页进行的值。 |

### 另请参见

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

使用默认值初始化一个新的 [`SearchOptions`](../../searchoptions) 类实例。详情请参阅备注。

```csharp
public SearchOptions()
```

### 备注

以下属性具有默认值：

**[`MatchCase`](../matchcase)**

`false`

**[`MatchWholeWord`](../matchwholeword)**

`false`

**[`UseRegularExpression`](../useregularexpression)**

`false`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### 另请参见

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
