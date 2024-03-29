---
title: PageTextAreaOptions
second_title: .NET API 참조용 GroupDocs.Parser
description: 페이지 텍스트 영역 추출에 사용되는 옵션을 제공합니다.
type: docs
weight: 550
url: /ko/net/groupdocs.parser.options/pagetextareaoptions/
---
## PageTextAreaOptions class

페이지 텍스트 영역 추출에 사용되는 옵션을 제공합니다.

```csharp
public sealed class PageTextAreaOptions : PageAreaOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PageTextAreaOptions](pagetextareaoptions#constructor)(bool) | 의 새 인스턴스를 초기화합니다.[`PageTextAreaOptions`](../pagetextareaoptions) OCR 사용 옵션이 있는 클래스. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_2)(string) | 의 새 인스턴스를 초기화합니다.[`PageTextAreaOptions`](../pagetextareaoptions) 정규 표현식이 있는 클래스. 다른 옵션은 기본적으로 설정됩니다(자세한 내용은 비고 참조). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_1)(bool, OcrOptions) | 의 새 인스턴스를 초기화합니다.[`PageTextAreaOptions`](../pagetextareaoptions) OCR 옵션을 설정할 수 있는 클래스. |
| [PageTextAreaOptions](pagetextareaoptions#constructor_4)(string, Rectangle) | 의 새 인스턴스를 초기화합니다.[`PageTextAreaOptions`](../pagetextareaoptions) class 정규 표현식 및 직사각형 영역 포함. 다른 옵션은 기본적으로 설정됩니다(자세한 내용은 비고 참조). |
| [PageTextAreaOptions](pagetextareaoptions#constructor_3)(string, bool, bool, bool, Rectangle) | 의 새 인스턴스를 초기화합니다.[`PageTextAreaOptions`](../pagetextareaoptions) 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Expression](../../groupdocs.parser.options/pagetextareaoptions/expression) { get; } | 정규식을 가져옵니다. |
| [IgnoreFormatting](../../groupdocs.parser.options/pagetextareaoptions/ignoreformatting) { get; } | 텍스트 서식이 무시되는지 여부를 나타내는 값을 가져옵니다. |
| [MatchCase](../../groupdocs.parser.options/pagetextareaoptions/matchcase) { get; } | 텍스트 대소문자가 무시되지 않는지 여부를 나타내는 값을 가져옵니다. |
| [OcrOptions](../../groupdocs.parser.options/pagetextareaoptions/ocroptions) { get; } | OCR 기능에 대한 추가 옵션을 가져옵니다. |
| [Rectangle](../../groupdocs.parser.options/pageareaoptions/rectangle) { get; } | 페이지 영역을 포함하는 직사각형 영역을 가져옵니다. |
| [UniteSegments](../../groupdocs.parser.options/pagetextareaoptions/unitesegments) { get; } | 세그먼트가 통합되었는지 여부를 나타내는 값을 가져옵니다. |
| [UseOcr](../../groupdocs.parser.options/pagetextareaoptions/useocr) { get; } | 텍스트 영역을 추출하는 데 OCR 기능이 사용되는지 여부를 나타내는 값을 가져옵니다. |

### 비고

의 인스턴스[`PageTextAreaOptions`](../pagetextareaoptions) 클래스는 매개변수 로 사용됩니다.[`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) 그리고[`GetTextAreas`](../../groupdocs.parser/parser/gettextareas) 방법. 사용 예를 참조하십시오. **더 알아보기:**

* [텍스트 영역 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 또한보십시오

* class [PageAreaOptions](../pageareaoptions)
* 네임스페이스 [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* 집회 [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
