---
title: "OcrOptions"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "직사각형 영역으로 OcrOptionsgroupdocs.parser.options/ocroptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/groupdocs.parser.options/ocroptions/ocroptions/
---

## OcrOptions() {#constructor}

직사각형 영역으로 [`OcrOptions`](../../ocroptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public OcrOptions()
```

### 참고

* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(PagePreviewOptions) {#constructor_6}

직사각형 영역으로 [`OcrOptions`](../../ocroptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pagePreviewOptions | PagePreviewOptions | [`PagePreviewOptions`](../pagepreviewoptions) 클래스의 인스턴스로, 문서 페이지 미리보기 생성을 위한 속성을 설정합니다. |

### 참고

* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle) {#constructor_1}

직사각형 영역으로 [`OcrOptions`](../../ocroptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public OcrOptions(Rectangle rectangle)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rectangle | Rectangle | 텍스트 인식에 사용되는 페이지 영역을 제한하는 직사각형 영역. |

### 참고

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(OcrEventHandler) {#constructor_5}

[`OcrEventHandler`](../../ocreventhandler) 객체와 함께 [`OcrOptions`](../../ocroptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public OcrOptions(OcrEventHandler handler)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| handler | OcrEventHandler | OCR 이벤트를 포착하기 위한 [`OcrEventHandler`](../../ocreventhandler) 인스턴스. |

### 참고

* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler) {#constructor_2}

직사각형 영역과 [`OcrEventHandler`](../../ocreventhandler) 객체와 함께 [`OcrOptions`](../../ocroptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rectangle | Rectangle | 텍스트 인식에 사용되는 페이지 영역을 제한하는 직사각형 영역. |
| handler | OcrEventHandler | OCR 이벤트를 포착하기 위한 [`OcrEventHandler`](../../ocreventhandler) 인스턴스. |

### 참고

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool) {#constructor_3}

[`OcrOptions`](../../ocroptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rectangle | Rectangle | 텍스트 인식에 사용되는 페이지 영역을 제한하는 직사각형 영역. |
| handler | OcrEventHandler | OCR 이벤트를 포착하기 위한 [`OcrEventHandler`](../../ocreventhandler) 인스턴스. |
| pagePreviewOptions | PagePreviewOptions | [`PagePreviewOptions`](../pagepreviewoptions) 클래스의 인스턴스로, 문서 페이지 미리보기 생성을 위한 속성을 설정합니다. |
| useSpellCheker | Boolean | 맞춤법 검사기가 사용되는지 여부를 나타내는 값입니다. |

### 참고

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## OcrOptions(Rectangle, OcrEventHandler, PagePreviewOptions, bool, Language) {#constructor_4}

[`OcrOptions`](../../ocroptions) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, 
    PagePreviewOptions pagePreviewOptions, bool useSpellCheker, Language language)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rectangle | Rectangle | 텍스트 인식에 사용되는 페이지 영역을 제한하는 직사각형 영역. |
| handler | OcrEventHandler | OCR 이벤트를 포착하기 위한 [`OcrEventHandler`](../../ocreventhandler) 인스턴스. |
| pagePreviewOptions | PagePreviewOptions | [`PagePreviewOptions`](../pagepreviewoptions) 클래스의 인스턴스로, 문서 페이지 미리보기 생성을 위한 속성을 설정합니다. |
| useSpellCheker | Boolean | 맞춤법 검사기가 사용되는지 여부를 나타내는 값입니다. |
| language | 언어 | OCR에 사용되는 언어입니다. |

### 참고

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [OcrEventHandler](../../ocreventhandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* enum [Language](../../language)
* class [OcrOptions](../../ocroptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
