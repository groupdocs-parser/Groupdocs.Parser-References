---
title: GetTextAreas
second_title: .NET API 참조용 GroupDocs.Parser
description: 문서에서 텍스트 영역을 추출합니다.
type: docs
weight: 160
url: /ko/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

문서에서 텍스트 영역을 추출합니다.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### 반환 값

컬렉션[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) 객체; `없는` 텍스트 영역 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [텍스트 영역 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 예

다음 예는 전체 문서에서 모든 텍스트 영역을 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using(Parser parser = new Parser(filePath))
{
    // 텍스트 영역 추출
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // 텍스트 영역 추출이 지원되는지 확인
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // 페이지 텍스트 영역을 반복합니다.
    foreach(PageTextArea a in areas)
    {
        // 페이지 인덱스, 사각형 및 텍스트 영역 값을 인쇄합니다.
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 또한보십시오

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

사용자 지정 옵션(정규식, 대/소문자 구분 등)을 사용하여 문서에서 텍스트 영역을 추출합니다.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| options | PageTextAreaOptions | 텍스트 영역 추출 옵션. |

### 반환 값

컬렉션[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) 객체; `없는` 텍스트 영역 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [텍스트 영역 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 예

다음 예는 왼쪽 위 모서리에서 숫자가 있는 텍스트 영역만 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using(Parser parser = new Parser(filePath))
{
    // 텍스트 영역 추출에 사용되는 옵션 생성
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // 페이지의 왼쪽 위 모서리에서 숫자만 포함하는 텍스트 영역을 추출합니다.
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // 텍스트 영역 추출이 지원되는지 확인
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // 페이지 텍스트 영역을 반복합니다.
    foreach(PageTextArea a in areas)
    {
        // 페이지 인덱스, 사각형 및 텍스트 영역 값을 인쇄합니다.
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 또한보십시오

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

문서 페이지에서 텍스트 영역을 추출합니다.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |

### 반환 값

컬렉션[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) 객체; `없는` 텍스트 영역 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [텍스트 영역 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 예

문서 페이지에서 텍스트 영역을 추출하려면 다음 방법이 사용됩니다.

```csharp
// Parser 클래스의 인스턴스 생성
using(Parser parser = new Parser(filePath))
{
    // 문서가 텍스트 영역 추출을 지원하는지 확인
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
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
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // 페이지 번호 출력 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // 페이지 텍스트 영역을 반복합니다.
        // 이전에 텍스트 영역 추출 기능 지원을 확인했으므로 null 검사를 무시합니다.
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // 사각형 및 텍스트 영역 값을 인쇄합니다.
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### 또한보십시오

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

사용자 지정 옵션(정규식, 대/소문자 구분 등)을 사용하여 문서 페이지에서 텍스트 영역을 추출합니다.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |
| options | PageTextAreaOptions | 텍스트 영역 추출 옵션. |

### 반환 값

컬렉션[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) 객체; `없는` 텍스트 영역 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [텍스트 영역 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 또한보십시오

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
