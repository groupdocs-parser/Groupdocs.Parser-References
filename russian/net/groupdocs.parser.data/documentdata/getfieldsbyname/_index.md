---
title: "GetFieldsByName"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Возвращает коллекцию данных полей, где имя равно fieldName."
type: docs
weight: 50
url: /ru/net/groupdocs.parser.data/documentdata/getfieldsbyname/
---

## DocumentData.GetFieldsByName method

Возвращает коллекцию данных полей, где имя равно *fieldName*.

```csharp
public IList<FieldData> GetFieldsByName(string fieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldName | Строка | Имя поля. |

### Возвращаемое значение

Коллекция объектов [`FieldData`](../../fielddata); пустая коллекция, если данные полей не найдены.

### Примеры

Найти поля по имени поля:

```csharp
// Получить все поля с именем "Address"
IList<FieldData> addressFields = data.GetFieldsByName("Address");
if(addressFields.Count == 0) {
    Console.WriteLine("Address not found");
}
else {
    Console.WriteLine("Address");
    // Итерировать коллекцию полей.
    for (int i = 0; i < addressFields.Count; i++) {
        PageTextArea area = addressFields[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);       
         
        // Если это связанное поле:
        if(addressFields[i].LinkedField != null) {
            Console.Write("Linked to ");
            PageTextArea linkedArea = addressFields[i].LinkedField.PageArea as PageTextArea;
            Console.WriteLine(area == null ? "Not a template field" : area.Text);           
        }
    }
}
```

[`FieldData`](../../fielddata) class represents field data. Depending on the field [`PageArea`](../../fielddata/pagearea) property can contain any of the inheritors of [`PageArea`](../../pagearea) class. For example, [`ParseForm`](../../../groupdocs.parser/parser/parseform) method extracts only text fields.

### См. также

* class [FieldData](../../fielddata)
* class [DocumentData](../../documentdata)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
