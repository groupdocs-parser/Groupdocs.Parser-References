---
title: "Возможности"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Получает поддерживаемые функции."
type: docs
weight: 20
url: /ru/net/groupdocs.parser/parser/features/
---

## Parser.Features property

Получает поддерживаемые функции.

```csharp
public Features Features { get; }
```

### Property Value

Экземпляр класса [`Features`](../../../groupdocs.parser.options/features), представляющий поддерживаемые функции.

### Примечания

**Learn more:**

* [Get supported features](https://docs.groupdocs.com/display/parsernet/Get+supported+features)

### Примеры

Если функция не поддерживается, метод возвращает `null` вместо значения. Некоторые операции могут занимать значительное время. Поэтому нецелесообразно вызывать метод только для проверки поддержки функции. Для этой цели используется свойство Features:

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

### См. также

* class [Features](../../../groupdocs.parser.options/features)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
