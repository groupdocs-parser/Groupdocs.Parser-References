---
title: Features
second_title: .NET API 참조용 GroupDocs.Parser
description: 지원되는 기능을 가져옵니다.
type: docs
weight: 20
url: /ko/net/groupdocs.parser/parser/features/
---
## Parser.Features property

지원되는 기능을 가져옵니다.

```csharp
public Features Features { get; }
```

### 자산 가치

인스턴스[`Features`](../../../groupdocs.parser.options/features) 지원되는 기능을 나타내는 클래스입니다.

### 비고

**더 알아보기:**

* [지원되는 기능 가져오기](https://docs.groupdocs.com/display/parsernet/Get+supported+features)

### 예

기능이 지원되지 않는 경우 메서드는 다음을 반환합니다.`없는` 값 대신. 일부 작업은 상당한 시간을 소비할 수 있습니다. 따라서 기능에 대한 지원을 확인하기 위해 메소드를 호출하는 것이 최적이 아닙니다. 이를 위해 기능 속성이 사용됩니다.

```csharp
using(Parser parser = new Parser("doc.zip"))
{
    if(!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported");
        return;
    }
 
    using(TextReader reader = parser.GetText())
    {
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

### 또한보십시오

* class [Features](../../../groupdocs.parser.options/features)
* class [Parser](../../parser)
* 네임스페이스 [GroupDocs.Parser](../../parser)
* 집회 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->