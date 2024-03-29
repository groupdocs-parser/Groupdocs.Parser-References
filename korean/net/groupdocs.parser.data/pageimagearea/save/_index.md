---
title: Save
second_title: .NET API 참조용 GroupDocs.Parser
description: 이미지를 파일에 저장합니다.
type: docs
weight: 50
url: /ko/net/groupdocs.parser.data/pageimagearea/save/
---
## Save(string) {#save}

이미지를 파일에 저장합니다.

```csharp
public void Save(string filePath)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일의 경로입니다. |

### 예

다음 예에서는 이미지를 파일에 저장하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // 문서에서 이미지 추출
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // 이미지 추출이 지원되는지 확인
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // 이미지 반복
    foreach (PageImageArea image in images)
    {
        // 이미지를 파일에 저장
        image.Save(Guid.NewGuid().ToString() + image.FileType.Extension);
    }
}
```

### 또한보십시오

* class [PageImageArea](../../pageimagearea)
* 네임스페이스 [GroupDocs.Parser.Data](../../pageimagearea)
* 집회 [GroupDocs.Parser](../../../)

---

## Save(string, ImageOptions) {#save_1}

이미지를 다른 형식의 파일로 저장합니다.

```csharp
public void Save(string filePath, ImageOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일의 경로입니다. |
| options | ImageOptions | 이미지를 저장하는 데 사용되는 옵션입니다. |

### 예

다음 예에서는 이미지를 다른 형식의 파일에 저장하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // 문서에서 이미지 추출
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // 이미지 추출이 지원되는지 확인
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // 이미지를 PNG 형식으로 저장하는 옵션 생성
    ImageOptions options = new ImageOptions(ImageFormat.Png);
    
    // 이미지 반복
    foreach (PageImageArea image in images)
    {
        // 이미지를 png 파일로 저장
        image.Save(Guid.NewGuid().ToString() + ".png", options);
    }
}
```

### 또한보십시오

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* 네임스페이스 [GroupDocs.Parser.Data](../../pageimagearea)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
