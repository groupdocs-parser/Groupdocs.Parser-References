---
title: ParseForm
second_title: .NET API 참조용 GroupDocs.Parser
description: 문서 양식을 구문 분석합니다.
type: docs
weight: 190
url: /ko/net/groupdocs.parser/parser/parseform/
---
## Parser.ParseForm method

문서 양식을 구문 분석합니다.

```csharp
public DocumentData ParseForm()
```

### 반환 값

의 인스턴스[`DocumentData`](../../../groupdocs.parser.data/documentdata) 추출된 데이터를 포함하는 클래스; `없는` 템플릿에 의한 구문 분석이 지원되지 않는 경우.

### 비고

**더 알아보기:**

* [PDF 양식에서 데이터 추출](https://docs.groupdocs.com/display/parsernet/Extract+data+from+PDF+forms)
* [추출된 데이터 작업](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [PDF 문서에서 데이터 구문 분석](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### 예

다음 예제에서는 문서 형식을 구문 분석하는 방법을 보여줍니다.

```csharp
// Parser 클래스의 인스턴스 생성
using (Parser parser = new Parser(filePath))
{
    // PDF 문서에서 데이터 추출
    DocumentData data = parser.ParseForm();
    // 추출된 데이터에 대해 반복
    for (int i = 0; i<data.Count; i++)
    {
        Console.Write(data[i].Name + ": ");
        PageTextArea area = data[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### 또한보십시오

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
