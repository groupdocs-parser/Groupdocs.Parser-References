---
title: "GetFormattedText"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает форматированный текст из документа."
type: docs
weight: 100
url: /ru/net/groupdocs.parser/parser/getformattedtext/
---

## GetFormattedText(FormattedTextOptions) {#getformattedtext}

Извлекает форматированный текст из документа.

```csharp
public TextReader GetFormattedText(FormattedTextOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | FormattedTextOptions | Параметры извлечения форматированного текста. |

### Возвращаемое значение

Экземпляр класса TextReader с извлечённым текстом; `null`, если извлечение форматированного текста не поддерживается.

### Примечания

**Learn more:**

* [Extract formatted text from document](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Примеры

В следующем примере показано, как извлечь текст документа в виде HTML:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь форматированный текст в reader
    using (TextReader reader = parser.GetFormattedText(new FormattedTextOptions(FormattedTextMode.Html)))
    {
        // Вывести форматированный текст из документа
        // Если извлечение форматированного текста не поддерживается, reader будет null
        Console.WriteLine(reader == null ? "Formatted text extraction isn't suppported" : reader.ReadToEnd());
    }
}
```

### См. также

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFormattedText(int, FormattedTextOptions) {#getformattedtext_1}

Извлекает форматированный текст со страницы документа.

```csharp
public TextReader GetFormattedText(int pageIndex, FormattedTextOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |
| options | FormattedTextOptions | Параметры извлечения форматированного текста. |

### Возвращаемое значение

Экземпляр класса TextReader с извлечённым текстом; `null`, если извлечение форматированного текста страницы не поддерживается.

### Примечания

**Learn more:**

* [Extract formatted text from document page](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Примеры

В следующем примере показано, как извлечь текст страницы документа в виде Markdown:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение форматированного текста
    if (!parser.Features.FormattedText)
    {
        Console.WriteLine("Document isn't supports formatted text extraction.");
        return;
    }
    
    // Получить информацию о документе
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Проверьте, есть ли у документа страницы
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Перебрать страницы
    for (int p = 0; p<documentInfo.PageCount; p++)
    {
        // Вывести номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
        // Извлечь форматированный текст в reader
        using (TextReader reader = parser.GetFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown)))
        {
            // Вывести форматированный текст из документа
            // Мы игнорируем проверку на null, так как ранее проверили поддержку функции извлечения форматированного текста
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### См. также

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
