---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "OCR 사용 옵션으로 PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

OCR 사용 옵션으로 [`PageTextAreaOptions`](../../pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PageTextAreaOptions()
```

### 참고

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

OCR 사용 옵션으로 [`PageTextAreaOptions`](../../pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| useOcr | Boolean | 텍스트 영역을 추출하기 위해 OCR 기능이 사용되는지 여부를 나타내는 값. |

### 참고

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

OCR 옵션을 설정할 수 있는 기능을 포함하여 [`PageTextAreaOptions`](../../pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| useOcr | Boolean | 텍스트 영역을 추출하기 위해 OCR 기능이 사용되는지 여부를 나타내는 값. |
| ocrOptions | OcrOptions | OCR 기능을 위한 추가 옵션입니다. |

### 참고

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

정규 표현식을 사용하여 [`PageTextAreaOptions`](../../pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다. 다른 옵션은 기본값으로 설정됩니다(자세한 내용은 주석을 참조하십시오).

```csharp
public PageTextAreaOptions(string expression)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 표현식 | 문자열 | 정규 표현식. |

### 비고

다음 속성은 기본값을 가집니다:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### 참고

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

정규 표현식과 사각형 영역을 사용하여 [`PageTextAreaOptions`](../../pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다. 다른 옵션은 기본값으로 설정됩니다(자세한 내용은 주석을 참조하십시오).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 표현식 | 문자열 | 정규 표현식. |
| rectangle | Rectangle | 페이지 영역을 포함하는 직사각형 영역. |

### 비고

다음 속성은 기본값을 가집니다:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### 참고

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

정규 표현식, 사각형 영역 및 무시된 경계의 크기를 사용하여 [`PageTextAreaOptions`](../../pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다. 다른 옵션은 기본값으로 설정됩니다(자세한 내용은 주석을 참조하십시오).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 표현식 | 문자열 | 정규 표현식. |
| rectangle | Rectangle | 페이지 영역을 포함하는 직사각형 영역. |
| rectangleTolerance | Double | 직사각형 영역에 의해 캡처될 때 무시되는 테두리의 크기입니다. 텍스트 항목 높이의 비율로 측정됩니다. |

### 참고

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

[`PageTextAreaOptions`](../../pagetextareaoptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 표현식 | 문자열 | 정규 표현식. |
| matchCase | Boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값. |
| uniteSegments | Boolean | 세그먼트가 결합되는지 여부를 나타내는 값. |
| ignoreFormatting | Boolean | 텍스트 서식이 무시되는지 여부를 나타내는 값. |
| rectangle | Rectangle | 페이지 영역을 포함하는 직사각형 영역. |

### 참고

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

[`PageTextAreaOptions`](../../pagetextareaoptions) 클래스의 새 인스턴스를 무시된 테두리 크기와 함께 초기화합니다.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 표현식 | 문자열 | 정규 표현식. |
| matchCase | Boolean | 텍스트 대소문자를 무시하지 않는지 여부를 나타내는 값. |
| uniteSegments | Boolean | 세그먼트가 결합되는지 여부를 나타내는 값. |
| ignoreFormatting | Boolean | 텍스트 서식이 무시되는지 여부를 나타내는 값. |
| rectangle | Rectangle | 페이지 영역을 포함하는 직사각형 영역. |
| rectangleTolerance | Double | 직사각형 영역에 의해 캡처될 때 무시되는 테두리의 크기입니다. 텍스트 항목 높이의 비율로 측정됩니다. |

### 참고

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
