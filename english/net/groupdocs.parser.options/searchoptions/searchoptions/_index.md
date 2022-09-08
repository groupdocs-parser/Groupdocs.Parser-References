---
title: SearchOptions
second_title: GroupDocs.Parser for .NET API Reference
description: Initializes a new instance of the SearchOptionsgroupdocs.parser.options/searchoptions class.
type: docs
weight: 10
url: /net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Initializes a new instance of the [`SearchOptions`](../../searchoptions) class.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | Boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | Boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | Boolean | The value that indicates whether a regular expression is used. |
| searchByPages | Boolean | The value that indicates whether the search is performed by pages. |
| leftHighlightOptions | HighlightOptions | The options for the left highlight. |
| rightHighlightOptions | HighlightOptions | The options for the right highlight. |

### See Also

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../searchoptions)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Initializes a new instance of the [`SearchOptions`](../../searchoptions) class which is used to search with the highlight options for the left and the right highlight extraction.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | Boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | Boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | Boolean | The value that indicates whether a regular expression is used. |
| leftHighlightOptions | HighlightOptions | The options for the left highlight. |
| rightHighlightOptions | HighlightOptions | The options for the right highlight. |

### See Also

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../searchoptions)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Initializes a new instance of the [`SearchOptions`](../../searchoptions) class which is used to search with the same highlight options for the left and the right highlight extraction.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | Boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | Boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | Boolean | The value that indicates whether a regular expression is used. |
| highlightOptions | HighlightOptions | The options for both highlights. |

### See Also

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../searchoptions)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Initializes a new instance of the [`SearchOptions`](../../searchoptions) class which is used to search without highlight extraction.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | Boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | Boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | Boolean | The value that indicates whether a regular expression is used. |

### See Also

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../searchoptions)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Initializes a new instance of the [`SearchOptions`](../../searchoptions) class which is used to search by pages and without highlight extraction.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Type | Description |
| --- | --- | --- |
| matchCase | Boolean | The value that indicates whether a text case isn't ignored. |
| matchWholeWord | Boolean | The value that indicates whether text search is limited by a whole word. |
| useRegularExpression | Boolean | The value that indicates whether a regular expression is used. |
| searchByPages | Boolean | The value that indicates whether the search is performed by pages. |

### See Also

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../searchoptions)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Initializes a new instance of the [`SearchOptions`](../../searchoptions) class with default values. See remarks for details.

```csharp
public SearchOptions()
```

### Remarks

The following properties have default values:

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

### See Also

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../searchoptions)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
