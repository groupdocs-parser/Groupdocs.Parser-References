---
title: GetImages
second_title: .NET API 참조용 GroupDocs.Parser
description: 문서에서 이미지를 추출합니다.
type: docs
weight: 110
url: /ko/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

문서에서 이미지를 추출합니다.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### 반환 값

컬렉션[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 객체; `없는` 이미지 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [이미지를 파일로 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Microsoft Office Word 문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel 스프레드시트에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint 프레젠테이션에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [이메일에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF 문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 예

다음 예제는 전체 문서에서 모든 이미지를 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // 이미지 추출
    IEnumerable<PageImageArea> images = parser.GetImages();
    // 이미지 추출이 지원되는지 확인
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // 이미지 반복
    foreach (PageImageArea image in images)
    {
        // 페이지 인덱스, 사각형 및 이미지 유형을 인쇄합니다.
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 또한보십시오

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

사용자 지정 옵션 (이미지가 포함된 직사각형 영역 설정)를 사용하여 문서에서 이미지를 추출합니다.

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| options | PageAreaOptions | 이미지 추출 옵션. |

### 반환 값

컬렉션[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 객체; `없는` 이미지 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [이미지를 파일로 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [문서 페이지 영역에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Microsoft Office Word 문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel 스프레드시트에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint 프레젠테이션에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [이메일에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF 문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 예

다음 예는 왼쪽 위 모서리에서 이미지만 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // 이미지 추출에 사용되는 옵션 생성
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // 페이지의 왼쪽 상단 모서리에서 이미지를 추출합니다.
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // 이미지 추출이 지원되는지 확인
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // 이미지 반복
    foreach (PageImageArea image in images)
    {
        // 페이지 인덱스, 사각형 및 이미지 유형을 인쇄합니다.
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 또한보십시오

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

문서 페이지에서 이미지를 추출합니다.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |

### 반환 값

컬렉션[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 객체; `없는` 이미지 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [이미지를 파일로 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [문서 페이지에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Microsoft Office Word 문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel 스프레드시트에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint 프레젠테이션에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [이메일에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF 문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 예

문서 페이지에서 이미지를 추출하려면 다음 방법이 사용됩니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // 문서가 이미지 추출을 지원하는지 확인
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
        return;
    }
    
    // 문서 정보 가져오기
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 문서에 페이지가 있는지 확인
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // 페이지를 반복
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // 페이지 번호 출력 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 이미지 반복
        // 이전에 이미지 추출 기능 지원 여부를 확인했으므로 null 검사는 무시합니다.
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // 사각형 및 이미지 유형을 인쇄합니다.
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### 또한보십시오

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

사용자 지정 옵션 (이미지가 포함된 직사각형 영역 설정)를 사용하여 문서 페이지에서 이미지를 추출합니다.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |
| options | PageAreaOptions | 이미지 추출 옵션. |

### 반환 값

컬렉션[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 객체; `없는` 이미지 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [이미지를 파일로 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [문서 페이지에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [문서 페이지 영역에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Microsoft Office Word 문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel 스프레드시트에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint 프레젠테이션에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [이메일에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [PDF 문서에서 이미지 추출](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 또한보십시오

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
