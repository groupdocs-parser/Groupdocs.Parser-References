---
title: "GetText"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает текст из документа."
type: docs
weight: 180
url: /ru/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

Извлекает текст из документа.

```csharp
public TextReader GetText()
```

### Возвращаемое значение

Экземпляр класса TextReader с извлечённым текстом; `null`, если извлечение текста не поддерживается.

### Примечания

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Примеры

В следующем примере показано, как извлечь текст из документа:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Извлечь текст в reader
    using(TextReader reader = parser.GetText())
    {
        // Вывести текст из документа
        // Если извлечение текста не поддерживается, reader будет null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### См. также

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Извлекает страницу текста из документа, используя параметры текста (для включения режима быстрого необработанного извлечения текста).

```csharp
public TextReader GetText(TextOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | TextOptions | Параметры извлечения текста. |

### Возвращаемое значение

Экземпляр класса TextReader с извлечённым текстом; `null`, если извлечение текста не поддерживается.

### Примечания

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Примеры

В следующем примере показано, как извлечь необработанный текст из документа:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Извлечь необработанный текст в reader
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Вывести текст из документа
        // Если извлечение текста не поддерживается, reader будет null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### См. также

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Извлекает текст со страницы документа.

```csharp
public TextReader GetText(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |

### Возвращаемое значение

Экземпляр класса TextReader с извлечённым текстом; `null`, если извлечение текста страницы не поддерживается.

### Примечания

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Примеры

В следующем примере показано, как извлечь текст со страницы документа:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение текста
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Получить информацию о документе
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Проверьте, есть ли у документа страницы
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Перебрать страницы
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Вывести номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Извлечь текст в reader
        using(TextReader reader = parser.GetText(p))
        {
            // Вывести текст из документа
            // Мы игнорируем проверку на null, так как ранее проверили поддержку функции извлечения текста
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### См. также

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Извлекает текст со страницы документа, используя параметры текста (для включения режима быстрого необработанного извлечения текста).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |
| options | TextOptions | Параметры извлечения текста. |

### Возвращаемое значение

Экземпляр класса TextReader с извлечённым текстом; `null`, если извлечение текста страницы не поддерживается.

### Примечания

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Примеры

В следующем примере показано, как извлечь необработанный текст со страницы документа:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Проверьте, поддерживает ли документ извлечение текста
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Получить информацию о документе
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Проверьте, есть ли у документа страницы
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Перебрать страницы
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Вывести номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Извлечь текст в reader
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Вывести текст из документа
            // Мы игнорируем проверку на null, так как ранее проверили поддержку функции извлечения текста
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### См. также

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
