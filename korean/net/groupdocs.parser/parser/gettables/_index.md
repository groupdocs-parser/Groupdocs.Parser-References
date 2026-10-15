---
title: "GetTables"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "문서에서 표를 추출합니다."
type: docs
weight: 170
url: /ko/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

문서에서 표를 추출합니다.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| options | PageTableAreaOptions | 표 추출을 위한 옵션입니다. |

### 반환 값

[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) 객체의 컬렉션; 표 추출이 지원되지 않으면 `null`입니다.

### 예제

다음 예제는 전체 문서에서 표를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 문서가 표 추출을 지원하는지 확인합니다
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // 표 레이아웃을 생성합니다
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // 표 추출 옵션을 생성합니다
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // 문서에서 표를 추출합니다
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // 테이블을 반복합니다
    foreach (PageTableArea t in tables)
    {
        // 행을 순회합니다
        for (int row = 0; row < t.RowCount; row++)
        {
            // 열을 순회합니다
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // 표 셀을 가져옵니다
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // 표 셀 텍스트를 출력합니다
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### 참고

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

문서 페이지에서 표를 추출합니다.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |
| options | PageTableAreaOptions | 표 추출을 위한 옵션입니다. |

### 반환 값

[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) 객체의 컬렉션; 표 추출이 지원되지 않으면 `null`입니다.

### 예제

다음 예제는 문서 페이지에서 표를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 문서가 표 추출을 지원하는지 확인합니다
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // 표 레이아웃을 생성합니다
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // 표 추출 옵션을 생성합니다
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // 문서 정보를 가져옵니다
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 문서에 페이지가 있는지 확인합니다
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // 페이지를 순회합니다
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // 페이지 번호를 출력합니다 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 문서 페이지에서 표를 추출합니다
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // 테이블을 반복합니다
        foreach (PageTableArea t in tables)
        {
            // 행을 순회합니다
            for (int row = 0; row < t.RowCount; row++)
            {
                // 열을 순회합니다
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // 표 셀을 가져옵니다
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // 표 셀 텍스트를 출력합니다
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### 참고

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

문서에서 표를 추출합니다.

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### 반환 값

[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) 객체의 컬렉션; 표 추출이 지원되지 않으면 `null`입니다.

### 예제

다음 예제는 전체 문서에서 표를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 문서가 표 추출을 지원하는지 확인합니다
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // 문서에서 표를 추출합니다
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // 테이블을 반복합니다
    foreach (PageTableArea t in tables)
    {
        // 행을 순회합니다
        for (int row = 0; row < t.RowCount; row++)
        {
            // 열을 순회합니다
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // 표 셀을 가져옵니다
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // 표 셀 텍스트를 출력합니다
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### 참고

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

문서 페이지에서 표를 추출합니다.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |

### 반환 값

[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) 객체의 컬렉션; 표 추출이 지원되지 않으면 `null`입니다.

### 예제

다음 예제는 문서 페이지에서 표를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 문서가 표 추출을 지원하는지 확인합니다
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // 문서 정보를 가져옵니다
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 문서에 페이지가 있는지 확인합니다
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // 페이지를 순회합니다
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // 페이지 번호를 출력합니다 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 문서 페이지에서 표를 추출합니다
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // 테이블을 반복합니다
        foreach (PageTableArea t in tables)
        {
            // 행을 순회합니다
            for (int row = 0; row < t.RowCount; row++)
            {
                // 열을 순회합니다
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // 표 셀을 가져옵니다
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // 표 셀 텍스트를 출력합니다
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### 참고

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
