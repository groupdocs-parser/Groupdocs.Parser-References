---
title: GetText
second_title: .NET API 참조용 GroupDocs.Parser
description: 문서에서 텍스트를 추출합니다.
type: docs
weight: 150
url: /ko/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

문서에서 텍스트를 추출합니다.

```csharp
public TextReader GetText()
```

### 반환 값

의 인스턴스TextReader 추출된 텍스트가 있는 클래스; `없는` 텍스트 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [문서에서 텍스트 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [정확 모드에서 텍스트 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 예

다음 예제에서는 문서에서 텍스트를 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using(Parser parser = new Parser(filePath))
{
    // 리더에 텍스트 추출
    using(TextReader reader = parser.GetText())
    {
        // 문서에서 텍스트 출력
        // 텍스트 추출이 지원되지 않는 경우 판독기는 null입니다.
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 또한보십시오

* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

텍스트 옵션을 사용하여 문서에서 텍스트 페이지를 추출합니다(원시 빠른 텍스트 추출 모드 활성화).

```csharp
public TextReader GetText(TextOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| options | TextOptions | 텍스트 추출 옵션. |

### 반환 값

의 인스턴스TextReader 추출된 텍스트가 있는 클래스; `없는` 텍스트 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [정확 모드에서 텍스트 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [원시 모드에서 텍스트 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 예

다음 예는 문서에서 원시 텍스트를 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using(Parser parser = new Parser(filePath))
{
    // 원시 텍스트를 판독기로 추출합니다.
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // 문서에서 텍스트 출력
        // 텍스트 추출이 지원되지 않는 경우 판독기는 null입니다.
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 또한보십시오

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

문서 페이지에서 텍스트를 추출합니다.

```csharp
public TextReader GetText(int pageIndex)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |

### 반환 값

의 인스턴스TextReader 추출된 텍스트가 있는 클래스; `없는` 텍스트 페이지 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [정확 모드에서 텍스트 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 예

다음 예는 문서 페이지에서 텍스트를 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using(Parser parser = new Parser(filePath))
{
    // 문서가 텍스트 추출을 지원하는지 확인
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // 문서 정보 가져오기
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 문서에 페이지가 있는지 확인
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // 페이지를 반복
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // 페이지 번호 출력 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // 리더에 텍스트 추출
        using(TextReader reader = parser.GetText(p))
        {
            // 문서에서 텍스트 출력
            // 앞에서 텍스트 추출 기능 지원 여부를 확인했으므로 null 검사는 무시합니다.
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 또한보십시오

* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

텍스트 옵션을 사용하여 문서 페이지에서 텍스트를 추출합니다(원시 빠른 텍스트 추출 모드 활성화).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |
| options | TextOptions | 텍스트 추출 옵션. |

### 반환 값

의 인스턴스TextReader 추출된 텍스트가 있는 클래스; `없는` 텍스트 페이지 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [정확 모드에서 텍스트 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [원시 모드에서 텍스트 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 예

다음 예는 문서 페이지에서 원시 텍스트를 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using(Parser parser = new Parser(filePath))
{
    // 문서가 텍스트 추출을 지원하는지 확인
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // 문서 정보 가져오기
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // 문서에 페이지가 있는지 확인
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // 페이지를 반복
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // 페이지 번호 출력 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // 리더에 텍스트 추출
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // 문서에서 텍스트 출력
            // 앞에서 텍스트 추출 기능 지원 여부를 확인했으므로 null 검사는 무시합니다.
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 또한보십시오

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
