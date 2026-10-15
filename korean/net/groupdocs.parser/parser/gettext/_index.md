---
title: "GetText"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "문서에서 텍스트를 추출합니다."
type: docs
weight: 180
url: /ko/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

문서에서 텍스트를 추출합니다.

```csharp
public TextReader GetText()
```

### 반환 값

추출된 텍스트를 가진 TextReader 클래스의 인스턴스; 텍스트 추출이 지원되지 않으면 `null`입니다.

### 비고

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 예제

다음 예제는 문서에서 텍스트를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 텍스트를 리더에 추출
    using(TextReader reader = parser.GetText())
    {
        // 문서에서 텍스트를 출력합니다
        // 텍스트 추출이 지원되지 않으면, 리더는 null입니다
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 참고

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

텍스트 옵션을 사용하여 문서에서 텍스트 페이지를 추출합니다 (원시 빠른 텍스트 추출 모드를 활성화하기 위해).

```csharp
public TextReader GetText(TextOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| options | TextOptions | 텍스트 추출 옵션입니다. |

### 반환 값

추출된 텍스트를 가진 TextReader 클래스의 인스턴스; 텍스트 추출이 지원되지 않으면 `null`입니다.

### 비고

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 예제

다음 예제는 문서에서 원시 텍스트를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 원시 텍스트를 리더에 추출합니다
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // 문서에서 텍스트를 출력합니다
        // 텍스트 추출이 지원되지 않으면, 리더는 null입니다
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### 참고

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

문서 페이지에서 텍스트를 추출합니다.

```csharp
public TextReader GetText(int pageIndex)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |

### 반환 값

추출된 텍스트를 가진 TextReader 클래스의 인스턴스; 텍스트 페이지 추출이 지원되지 않으면 `null`입니다.

### 비고

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### 예제

다음 예제는 문서 페이지에서 텍스트를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 문서가 텍스트 추출을 지원하는지 확인합니다
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // 문서 정보를 가져옵니다
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 문서에 페이지가 있는지 확인합니다
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // 페이지를 순회합니다
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // 페이지 번호를 출력합니다 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // 텍스트를 리더에 추출
        using(TextReader reader = parser.GetText(p))
        {
            // 문서에서 텍스트를 출력합니다
            // 우리는 이전에 텍스트 추출 기능 지원을 확인했으므로 null 검사을 무시합니다
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 참고

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

텍스트 옵션을 사용하여 문서 페이지에서 텍스트를 추출합니다 (원시 빠른 텍스트 추출 모드를 활성화하기 위해).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |
| options | TextOptions | 텍스트 추출 옵션입니다. |

### 반환 값

추출된 텍스트를 가진 TextReader 클래스의 인스턴스; 텍스트 페이지 추출이 지원되지 않으면 `null`입니다.

### 비고

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### 예제

다음 예제는 문서 페이지에서 원시 텍스트를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 문서가 텍스트 추출을 지원하는지 확인합니다
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // 문서 정보를 가져옵니다
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // 문서에 페이지가 있는지 확인합니다
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // 페이지를 순회합니다
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // 페이지 번호를 출력합니다 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // 텍스트를 리더에 추출
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // 문서에서 텍스트를 출력합니다
            // 우리는 이전에 텍스트 추출 기능 지원을 확인했으므로 null 검사을 무시합니다
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 참고

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
