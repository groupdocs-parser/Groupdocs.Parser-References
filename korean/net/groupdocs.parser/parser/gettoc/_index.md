---
title: GetToc
second_title: .NET API 참조용 GroupDocs.Parser
description: 문서에서 목차를 추출합니다.
type: docs
weight: 170
url: /ko/net/groupdocs.parser/parser/gettoc/
---
## Parser.GetToc method

문서에서 목차를 추출합니다.

```csharp
public IEnumerable<TocItem> GetToc()
```

### 반환 값

목차 항목 모음; `없는` 목차 추출이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [목차 추출](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents)
* [목차 항목별로 텍스트 추출](https://docs.groupdocs.com/display/parsernet/Extract+text+by+table+of+contents+item)
* [Microsoft Office Word 문서에서 목차 추출](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [EPUB eBook에서 목차 추출](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+EPUB+eBooks)

### 예

다음 예는 CHM 파일에서 목차를 추출하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // 텍스트 추출 지원 여부 확인
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }

    // toc 추출 지원 여부 확인
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
 
    // 목차 가져오기
    IEnumerable<TocItem> toc = parser.GetToc();
    
    // 항목 반복
    foreach (TocItem i in toc)
    {
        // Toc 텍스트 출력
        Console.WriteLine(i.Text);
        // 페이지 인덱스에 값이 있는지 확인
        if (i.PageIndex == null)
        {
            continue;
        }
        // 페이지 텍스트 추출
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### 또한보십시오

* class [TocItem](../../../groupdocs.parser.data/tocitem)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->