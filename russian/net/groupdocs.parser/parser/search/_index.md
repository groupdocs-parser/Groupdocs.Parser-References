---
title: "Search"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Ищет ключевое слово в документе."
type: docs
weight: 250
url: /ru/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

Ищет *keyword* в документе.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ключевое слово | Строка | Ключевое слово для поиска. |

### Возвращаемое значение

Коллекция объектов [`SearchResult`](../../../groupdocs.parser.data/searchresult); `null`, если поиск не поддерживается.

### Примечания

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Примеры

В следующем примере показано, как найти ключевое слово в документе:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Найти ключевое слово:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Проверьте, поддерживается ли поиск
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Перебрать результаты поиска
    foreach(SearchResult s in sr)
    {
        // Вывести индекс и найденный текст:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### См. также

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Ищет *keyword* в документе, используя параметры поиска (регулярные выражения, учет регистра и т.д.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ключевое слово | Строка | Ключевое слово для поиска. |
| options | SearchOptions | Параметры поиска. |

### Возвращаемое значение

Коллекция объектов [`SearchResult`](../../../groupdocs.parser.data/searchresult); `null`, если поиск не поддерживается.

### Примечания

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Примеры

В следующем примере показано, как выполнять поиск с помощью регулярного выражения в документе:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Поиск с регулярным выражением с учётом регистра
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Проверьте, поддерживается ли поиск
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Перебрать результаты поиска
    foreach(SearchResult s in sr)
    {
        // Вывести индекс и найденный текст:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

В следующем примере показано, как искать текст на страницах:

```csharp
// Создайте экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Поиск ключевого слова с номерами страниц
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Проверьте, поддерживается ли поиск
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Перебрать результаты поиска
    foreach(SearchResult s in sr)
    {
        // Вывести индекс, номер страницы и найденный текст:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### См. также

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
