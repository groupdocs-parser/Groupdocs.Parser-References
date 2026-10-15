---
title: "GetHyperlinks"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "문서에서 하이퍼링크를 추출합니다."
type: docs
weight: 120
url: /ko/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

문서에서 하이퍼링크를 추출합니다.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### 반환 값

[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) 객체의 컬렉션; 하이퍼링크 추출을 지원하지 않을 경우 `null`.

### 예제

다음 예제는 전체 문서에서 모든 하이퍼링크를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 문서가 하이퍼링크 추출을 지원하는지 확인합니다
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // 문서에서 하이퍼링크를 추출합니다
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // 하이퍼링크를 반복합니다
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // 하이퍼링크 텍스트를 출력합니다
        Console.WriteLine(h.Text);
        // 하이퍼링크 URL을 출력합니다
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### 참고

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

문서 페이지에서 하이퍼링크를 추출합니다.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |

### 반환 값

[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) 객체의 컬렉션; 하이퍼링크 추출을 지원하지 않을 경우 `null`.

### 예제

다음 예제는 문서 페이지에서 하이퍼링크를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 문서가 하이퍼링크 추출을 지원하는지 확인합니다
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // 문서 정보를 가져옵니다
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 문서에 페이지가 있는지 확인합니다
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // 페이지를 순회합니다
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // 페이지 번호를 출력합니다 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 문서 페이지에서 하이퍼링크를 추출합니다
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // 하이퍼링크를 반복합니다
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // 하이퍼링크 텍스트를 출력합니다
            Console.WriteLine(h.Text);
            // 하이퍼링크 URL을 출력합니다
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### 참고

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

맞춤 옵션을 사용하여 문서에서 하이퍼링크를 추출합니다 (하이퍼링크가 포함된 사각형 영역을 설정하기 위해).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| options | PageAreaOptions | 하이퍼링크 추출 옵션입니다. |

### 반환 값

[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) 객체의 컬렉션; 하이퍼링크 추출을 지원하지 않을 경우 `null`.

### 예제

다음 예제는 문서 페이지 영역에서 하이퍼링크를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 문서가 하이퍼링크 추출을 지원하는지 확인합니다
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // 하이퍼링크 추출에 사용되는 옵션을 생성합니다
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // 문서 페이지 영역에서 하이퍼링크를 추출합니다
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // 하이퍼링크를 반복합니다
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // 하이퍼링크 텍스트를 출력합니다
        Console.WriteLine(h.Text);
        // 하이퍼링크 URL을 출력합니다
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### 참고

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

맞춤 옵션을 사용하여 문서 페이지에서 하이퍼링크를 추출합니다 (하이퍼링크가 포함된 사각형 영역을 설정하기 위해).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |
| options | PageAreaOptions | 하이퍼링크 추출 옵션입니다. |

### 반환 값

[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) 객체의 컬렉션; 하이퍼링크 추출을 지원하지 않을 경우 `null`.

### 예제

다음 예제는 사용자 지정 옵션을 사용하여 문서 페이지 영역에서 하이퍼링크를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 문서가 하이퍼링크 추출을 지원하는지 확인합니다
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // 문서 정보를 가져옵니다
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 문서에 페이지가 있는지 확인합니다
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // 하이퍼링크 추출에 사용되는 옵션을 생성합니다
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // 페이지를 순회합니다
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // 페이지 번호를 출력합니다 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // 문서 페이지 영역에서 하이퍼링크를 추출합니다
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // 하이퍼링크를 반복합니다
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // 하이퍼링크 텍스트를 출력합니다
            Console.WriteLine(h.Text);
            // 하이퍼링크 URL을 출력합니다
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### 참고

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
