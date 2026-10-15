---
title: "PageArea"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Получает значение поля."
type: docs
weight: 30
url: /ru/net/groupdocs.parser.data/fielddata/pagearea/
---

## FieldData.PageArea property

Получает значение поля.

```csharp
public PageArea PageArea { get; }
```

### Property Value

Экземпляр класса [`PageArea`](../../pagearea), представляющий значение поля.

### Примеры

В зависимости от свойства поля `PageArea` оно может содержать любой из наследников класса [`PageArea`](../../pagearea). Например, метод [`ParseForm`](../../../groupdocs.parser/parser/parseform) извлекает только текстовые поля.

```csharp
// Получить данные поля
FieldData field = data[i];
// Проверить, содержит ли данные поля текст
if(field.PageArea is PageTextArea)
{
    // Вывести значение текста поля
    Console.WriteLine(field.Text);
}
```

### См. также

* class [PageArea](../../pagearea)
* class [FieldData](../../fielddata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
