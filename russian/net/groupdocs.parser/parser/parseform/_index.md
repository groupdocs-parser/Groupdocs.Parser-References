---
title: "ParseForm"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Разбирает форму документа."
type: docs
weight: 240
url: /ru/net/groupdocs.parser/parser/parseform/
---

## Parser.ParseForm method

Разбирает форму документа.

```csharp
public DocumentData ParseForm()
```

### Возвращаемое значение

Экземпляр класса [`DocumentData`](../../../groupdocs.parser.data/documentdata), содержащего извлечённые данные; `null`, если разбор по шаблону не поддерживается.

### Примечания

**Learn more:**

* [Extract data from PDF forms](https://docs.groupdocs.com/display/parsernet/Extract+data+from+PDF+forms)
* [Working with extracted data](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### Примеры

В следующем примере показано, как разобрать форму документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь данные из PDF‑документа
    DocumentData data = parser.ParseForm();
    // Итерировать извлечённые данные
    for (int i = 0; i<data.Count; i++)
    {
        Console.Write(data[i].Name + ": ");
        PageTextArea area = data[i].PageArea as PageTextArea;
        Console.WriteLine(area == null ? "Not a template field" : area.Text);
    }
}
```

### См. также

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
