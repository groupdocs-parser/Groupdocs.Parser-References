---
title: RecognizeText
second_title: .NET API 참조용 GroupDocs.Parser
description: 에서 텍스트를 인식합니다.imageStream 스트림.
type: docs
weight: 10
url: /ko/net/groupdocs.parser.options/ocrconnectorbase/recognizetext/
---
## OcrConnectorBase.RecognizeText method

에서 텍스트를 인식합니다.*imageStream* 스트림.

```csharp
public virtual string RecognizeText(Stream imageStream, int pageIndex, OcrOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| imageStream | Stream | 문서 페이지의 이미지 표현입니다. |
| pageIndex | Int32 | 문서의 페이지 인덱스입니다. |
| options | OcrOptions | OCR 옵션. |

### 반환 값

인식된 텍스트를 나타내는 문자열입니다.`없는` 텍스트 인식이 지원되지 않는 경우.

### 또한보십시오

* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* 네임스페이스 [GroupDocs.Parser.Options](../../ocrconnectorbase)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->