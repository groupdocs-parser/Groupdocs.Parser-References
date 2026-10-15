---
title: "GetHighlight"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает выделение из документа."
type: docs
weight: 110
url: /ru/net/groupdocs.parser/parser/gethighlight/
---

## Parser.GetHighlight method

Извлекает выделение из документа.

```csharp
public HighlightItem GetHighlight(int position, bool isDirect, HighlightOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| позиция | Int32 | Начальная позиция выделения. |
| isDirect | Boolean | Значение, указывающее, является ли извлечение выделения прямым. `true`, если выделение извлекается справа от *position*; иначе `false`. |
| options | HighlightOptions | Опции извлечения выделения. |

### Возвращаемое значение

Экземпляр класса [`HighlightItem`](../../../groupdocs.parser.data/highlightitem), представляющий извлечённое выделение; `null`, если извлечение выделения не поддерживается.

### Примечания

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### Примеры

Следующий пример показывает, как извлечь выделение, содержащее 3 слова:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь выделение:
    HighlightItem hl = parser.GetHighlight(2, true, new HighlightOptions(3));
    
    // Проверьте, поддерживается ли извлечение выделения
    if (hl == null)
    {
        Console.WriteLine("Highlight extraction isn't supported");
        return;
    }
    
    // Выведите извлечённое выделение
    Console.WriteLine(string.Format("At {0}: {1}", hl.Position, hl.Text));
}
```

### См. также

* class [HighlightItem](../../../groupdocs.parser.data/highlightitem)
* class [HighlightOptions](../../../groupdocs.parser.options/highlightoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
