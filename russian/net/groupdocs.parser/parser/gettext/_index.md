---
title: GetText
second_title: Справочник по API GroupDocs.Parser для .NET
description: Извлекает текст из документа.
type: docs
weight: 150
url: /ru/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Извлекает текст из документа.

```csharp
public TextReader GetText()
```

### Возвращаемое значение

ЭкземплярTextReader класс с извлеченным текстом; `нулевой` если извлечение текста не поддерживается.

### Примечания

**Узнать больше:**

* [Извлечение текста из документов](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Извлечь текст в точном режиме](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Примеры

В следующем примере показано, как извлечь текст из документа:

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Извлечь текст в ридер
    using(TextReader reader = parser.GetText())
    {
        // Печатаем текст из документа
        // Если извлечение текста не поддерживается, читатель имеет значение null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Смотрите также

* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

Извлекает текстовую страницу из документа с помощью параметров текста (чтобы включить режим быстрого извлечения необработанного текста).

```csharp
public TextReader GetText(TextOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | TextOptions | Параметры извлечения текста. |

### Возвращаемое значение

ЭкземплярTextReader класс с извлеченным текстом; `нулевой` если извлечение текста не поддерживается.

### Примечания

**Узнать больше:**

* [Извлечь текст в точном режиме](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Извлечение текста в режиме Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Примеры

В следующем примере показано, как извлечь необработанный текст из документа:

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Извлечь необработанный текст в ридер
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Печатаем текст из документа
        // Если извлечение текста не поддерживается, читатель имеет значение null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Смотрите также

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Извлекает текст со страницы документа.

```csharp
public TextReader GetText(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |

### Возвращаемое значение

ЭкземплярTextReader класс с извлеченным текстом; `нулевой` если извлечение текстовой страницы не поддерживается.

### Примечания

**Узнать больше:**

* [Извлечь текст в точном режиме](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Примеры

В следующем примере показано, как извлечь текст со страницы документа:

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение текста
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Получить информацию о документе
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Проверяем, есть ли в документе страницы
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Перебираем страницы
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Печатаем номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Извлечь текст в ридер
        using(TextReader reader = parser.GetText(p))
        {
            // Печатаем текст из документа
            // Мы игнорируем проверку на null, так как мы проверили поддержку функции извлечения текста ранее
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Смотрите также

* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

Извлекает текст со страницы документа с помощью параметров текста (чтобы включить режим быстрого извлечения необработанного текста).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |
| options | TextOptions | Параметры извлечения текста. |

### Возвращаемое значение

ЭкземплярTextReader класс с извлеченным текстом; `нулевой` если извлечение текстовой страницы не поддерживается.

### Примечания

**Узнать больше:**

* [Извлечь текст в точном режиме](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Извлечение текста в режиме Raw](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Примеры

В следующем примере показано, как извлечь необработанный текст со страницы документа:

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Проверяем, поддерживает ли документ извлечение текста
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Получить информацию о документе
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Проверяем, есть ли в документе страницы
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Перебираем страницы
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Печатаем номер страницы 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Извлечь текст в ридер
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Печатаем текст из документа
            // Мы игнорируем проверку на null, так как мы проверили поддержку функции извлечения текста ранее
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Смотрите также

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
