---
title: "Элемент"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Возвращает данные поля по индексу."
type: docs
weight: 20
url: /ru/net/groupdocs.parser.data/documentdata/item/
---

## DocumentData indexer

Возвращает данные поля по индексу.

```csharp
public FieldData this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс поля, начинающийся с нуля. |

### Возвращаемое значение

Экземпляр класса [`FieldData`](../../fielddata).

### Примеры

Итерация по всем полям:

```csharp
for (int i = 0; i < data.Count; i++)
{
    Console.Write(data[i].Name + ": ");
    PageTextArea area = data[i].PageArea as PageTextArea;
    Console.WriteLine(area == null ? "Not a template field" : area.Text);
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields:

```csharp
// Создать парсер
using (Parser parser = new Parser(filePath))
{
    // Извлечь данные из PDF-формы
    DocumentData data = parser.ParseForm();
    // Итерировать извлечённые поля
    for (int i = 0; i < data.Count; i++)
    {
        // Получить извлечённое поле
        FieldData field = data[i];
        // Вывести имя поля
        Console.Write(field.Name + ": ");
        // Проверить, является ли значение поля текстом, и вывести его
        PageTextArea area = field.PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### См. также

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
