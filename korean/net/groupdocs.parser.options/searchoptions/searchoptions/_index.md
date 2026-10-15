---
title: "SearchOptions"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "SearchOptionsgroupdocs.parser.options/searchoptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

[`SearchOptions`](../../searchoptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| matchCase | Boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값. |
| matchWholeWord | Boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값입니다. |
| useRegularExpression | Boolean | 정규식이 사용되는지 여부를 나타내는 값입니다. |
| searchByPages | Boolean | 검색이 페이지별로 수행되는지 여부를 나타내는 값입니다. |
| leftHighlightOptions | HighlightOptions | 왼쪽 강조에 대한 옵션입니다. |
| rightHighlightOptions | HighlightOptions | 오른쪽 강조에 대한 옵션입니다. |

### 참고

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

페이지 제한과 함께 [`SearchOptions`](../../searchoptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| matchCase | Boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값. |
| matchWholeWord | Boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값입니다. |
| useRegularExpression | Boolean | 정규식이 사용되는지 여부를 나타내는 값입니다. |
| maxPageIndex | Int32 | 검색이 페이지별로 수행되는지 여부를 나타내는 값입니다. |
| leftHighlightOptions | HighlightOptions | 왼쪽 강조에 대한 옵션입니다. |
| rightHighlightOptions | HighlightOptions | 오른쪽 강조에 대한 옵션입니다. |

### 참고

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

새로운 [`SearchOptions`](../../searchoptions) 클래스 인스턴스를 초기화합니다. 이 클래스는 왼쪽 및 오른쪽 하이라이트 추출을 위한 하이라이트 옵션으로 검색하는 데 사용됩니다.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| matchCase | Boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값. |
| matchWholeWord | Boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값입니다. |
| useRegularExpression | Boolean | 정규식이 사용되는지 여부를 나타내는 값입니다. |
| leftHighlightOptions | HighlightOptions | 왼쪽 강조에 대한 옵션입니다. |
| rightHighlightOptions | HighlightOptions | 오른쪽 강조에 대한 옵션입니다. |

### 참고

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

새로운 [`SearchOptions`](../../searchoptions) 클래스 인스턴스를 초기화합니다. 이 클래스는 왼쪽 및 오른쪽 하이라이트 추출을 위한 동일한 하이라이트 옵션으로 검색하는 데 사용됩니다.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| matchCase | Boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값. |
| matchWholeWord | Boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값입니다. |
| useRegularExpression | Boolean | 정규식이 사용되는지 여부를 나타내는 값입니다. |
| highlightOptions | HighlightOptions | 두 하이라이트에 대한 옵션입니다. |

### 참고

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

새로운 [`SearchOptions`](../../searchoptions) 클래스 인스턴스를 초기화합니다. 이 클래스는 하이라이트 추출 없이 검색하는 데 사용됩니다.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| matchCase | Boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값. |
| matchWholeWord | Boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값입니다. |
| useRegularExpression | Boolean | 정규식이 사용되는지 여부를 나타내는 값입니다. |

### 참고

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

새로운 [`SearchOptions`](../../searchoptions) 클래스 인스턴스를 초기화합니다. 이 클래스는 페이지별로 검색하고 하이라이트 추출 없이 사용됩니다.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| matchCase | Boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값. |
| matchWholeWord | Boolean | 텍스트 검색이 전체 단어로 제한되는지 여부를 나타내는 값입니다. |
| useRegularExpression | Boolean | 정규식이 사용되는지 여부를 나타내는 값입니다. |
| searchByPages | Boolean | 검색이 페이지별로 수행되는지 여부를 나타내는 값입니다. |

### 참고

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

기본값으로 새로운 [`SearchOptions`](../../searchoptions) 클래스 인스턴스를 초기화합니다. 자세한 내용은 주석을 참조하십시오.

```csharp
public SearchOptions()
```

### 비고

다음 속성은 기본값을 가집니다:

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

### 참고

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
