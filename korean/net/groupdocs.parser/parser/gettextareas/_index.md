---
title: "GetTextAreas"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "문서에서 텍스트 영역을 추출합니다."
type: docs
weight: 190
url: /ko/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

문서에서 텍스트 영역을 추출합니다.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### 반환 값

텍스트 영역 추출이 지원되지 않을 경우 `null`; [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) 객체의 컬렉션입니다.

### 비고

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 예제

다음 예제는 전체 문서에서 모든 텍스트 영역을 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 텍스트 영역 추출
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // 텍스트 영역 추출이 지원되는지 확인합니다
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // 페이지 텍스트 영역을 반복합니다
    foreach(PageTextArea a in areas)
    {
        // 페이지 인덱스, 사각형 및 텍스트 영역 값을 출력합니다:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 참고

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

맞춤 옵션(정규식, 대소문자 구분 등)을 사용하여 문서에서 텍스트 영역을 추출합니다.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| options | PageTextAreaOptions | 텍스트 영역 추출 옵션입니다. |

### 반환 값

텍스트 영역 추출이 지원되지 않을 경우 `null`; [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) 객체의 컬렉션입니다.

### 비고

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 예제

다음 예제는 왼쪽 위 모서리에서 숫자를 포함한 텍스트 영역만 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 텍스트 영역 추출에 사용되는 옵션을 생성합니다
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // 페이지의 왼쪽 위 모서리에서 숫자만 포함된 텍스트 영역을 추출합니다:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // 텍스트 영역 추출이 지원되는지 확인합니다
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // 페이지 텍스트 영역을 반복합니다
    foreach(PageTextArea a in areas)
    {
        // 페이지 인덱스, 사각형 및 텍스트 영역 값을 출력합니다:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 참고

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

문서 페이지에서 텍스트 영역을 추출합니다.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |

### 반환 값

텍스트 영역 추출이 지원되지 않을 경우 `null`; [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) 객체의 컬렉션입니다.

### 비고

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 예제

문서 페이지에서 텍스트 영역을 추출하려면 다음 메서드를 사용합니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 문서가 텍스트 영역 추출을 지원하는지 확인합니다
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
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
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // 페이지 번호를 출력합니다 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // 페이지 텍스트 영역을 반복합니다
        // 이미 텍스트 영역 추출 기능 지원을 확인했으므로 null 검사을 무시합니다
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // 사각형 및 텍스트 영역 값을 출력합니다:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### 참고

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

맞춤 옵션(정규식, 대소문자 구분 등)을 사용하여 문서 페이지에서 텍스트 영역을 추출합니다.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |
| options | PageTextAreaOptions | 텍스트 영역 추출 옵션입니다. |

### 반환 값

텍스트 영역 추출이 지원되지 않을 경우 `null`; [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) 객체의 컬렉션입니다.

### 비고

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 참고

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
