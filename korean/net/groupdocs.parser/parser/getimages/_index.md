---
title: "GetImages"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "문서에서 이미지를 추출합니다."
type: docs
weight: 130
url: /ko/net/groupdocs.parser/parser/getimages/
---

## GetImages() {#getimages}

문서에서 이미지를 추출합니다.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### 반환 값

이미지 추출을 지원하지 않으면 `null`인 [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 객체 컬렉션입니다.

### 비고

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 예제

다음 예제는 전체 문서에서 모든 이미지를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
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
    // 이미지를 반복 처리
    foreach (PageImageArea image in images)
    {
        // 페이지 인덱스, 사각형 및 이미지 유형을 출력합니다:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 참고

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

맞춤 옵션을 사용하여 문서에서 이미지를 추출합니다 (이미지가 포함된 사각형 영역을 설정하기 위해).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| options | PageAreaOptions | 이미지 추출 옵션입니다. |

### 반환 값

이미지 추출을 지원하지 않으면 `null`인 [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 객체 컬렉션입니다.

### 비고

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 예제

다음 예제는 왼쪽 위 모서리에서만 이미지를 추출하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 이미지 추출에 사용되는 옵션을 생성합니다
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // 페이지의 왼쪽 위 모서리에서 이미지를 추출합니다:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // 이미지 추출이 지원되는지 확인
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // 이미지를 반복 처리
    foreach (PageImageArea image in images)
    {
        // 페이지 인덱스, 사각형 및 이미지 유형을 출력합니다:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 참고

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

문서 페이지에서 이미지를 추출합니다.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |

### 반환 값

이미지 추출을 지원하지 않으면 `null`인 [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 객체 컬렉션입니다.

### 비고

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 예제

문서 페이지에서 이미지를 추출하려면 다음 메서드를 사용합니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using (Parser parser = new Parser(filePath))
{
    // 문서가 이미지 추출을 지원하는지 확인합니다
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // 페이지 번호를 출력합니다 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 이미지를 반복 처리
        // 이미 이미지 추출 기능 지원을 확인했으므로 null 검사을 무시합니다
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // 사각형 및 이미지 유형을 출력합니다
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### 참고

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

맞춤 옵션을 사용하여 문서 페이지에서 이미지를 추출합니다 (이미지가 포함된 사각형 영역을 설정하기 위해).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageIndex | Int32 | 0부터 시작하는 페이지 인덱스입니다. |
| options | PageAreaOptions | 이미지 추출 옵션입니다. |

### 반환 값

이미지 추출을 지원하지 않으면 `null`인 [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 객체 컬렉션입니다.

### 비고

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 참고

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
