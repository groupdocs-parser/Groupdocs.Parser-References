---
title: GetBarcodes
second_title: .NET API 참조용 GroupDocs.Parser
description: 문서에서 바코드를 추출합니다.
type: docs
weight: 50
url: /ko/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

문서에서 바코드를 추출합니다.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### 반환 값

컬렉션[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) 객체; `없는` 바코드 추출이 지원되지 않는 경우.

### 예

다음 예는 문서에서 바코드를 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // 문서에서 바코드를 추출합니다.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // 바코드 반복
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // 페이지 인덱스 출력
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // 바코드 값 출력
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### 또한보십시오

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

문서 페이지에서 바코드를 추출합니다.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |

### 반환 값

컬렉션[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) 객체; `없는` 바코드 추출이 지원되지 않는 경우.

### 예

다음 예는 문서 페이지에서 바코드를 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // 두 번째 문서 페이지에서 바코드를 추출합니다.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // 바코드 반복
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // 페이지 인덱스 출력
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // 바코드 값 출력
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### 또한보십시오

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

사용자 지정 옵션 (바코드가 포함된 직사각형 영역 설정)를 사용하여 문서에서 바코드를 추출합니다.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| options | PageAreaOptions | 바코드 추출 옵션입니다. |

### 반환 값

컬렉션[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) 객체; `없는` 바코드 추출이 지원되지 않는 경우.

### 예

다음 예제는 오른쪽 상단에서 바코드를 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // 바코드 추출에 사용되는 옵션 생성
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // 오른쪽 상단에서 바코드를 추출합니다.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // 바코드 반복
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // 페이지 인덱스 출력
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // 바코드 값 출력
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### 또한보십시오

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

사용자 지정 옵션 (바코드가 포함된 직사각형 영역 설정)를 사용하여 문서 페이지에서 바코드를 추출합니다.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |
| options | PageAreaOptions | 바코드 추출 옵션입니다. |

### 반환 값

컬렉션[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) 객체; `없는` 바코드 추출이 지원되지 않는 경우.

### 또한보십시오

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
