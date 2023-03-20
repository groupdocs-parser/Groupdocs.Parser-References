---
title: Search
second_title: Справочник по API GroupDocs.Parser для .NET
description: Ищетkeyword в документе.
type: docs
weight: 200
url: /ru/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

Ищет*keyword* в документе.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| keyword | String | Ключевое слово для поиска. |

### Возвращаемое значение

Коллекция[`SearchResult`](../../../groupdocs.parser.data/searchresult) объекты; `нулевой` если поиск не поддерживается.

### Примечания

**Узнать больше:**

* [Поиск текста](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Поиск текста в документах Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Поиск текста в электронных таблицах Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Поиск текста в презентациях Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Поиск текста в документах PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Искать текст в электронных письмах](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Поиск текста в электронных книгах EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Поиск текста в документах HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Поиск текста в разделах Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Примеры

В следующем примере показано, как найти ключевое слово в документе:

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Поиск по ключевому слову:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Проверяем, поддерживается ли поиск
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Перебираем результаты поиска
    foreach(SearchResult s in sr)
    {
        // Печатаем индекс и найденный текст:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Смотрите также

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Ищет*keyword*в документе с помощью параметров поиска (регулярное выражение, регистр и т. д.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| keyword | String | Ключевое слово для поиска. |
| options | SearchOptions | Параметры поиска. |

### Возвращаемое значение

Коллекция[`SearchResult`](../../../groupdocs.parser.data/searchresult) объекты; `нулевой` если поиск не поддерживается.

### Примечания

**Узнать больше:**

* [Поиск текста](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Поиск текста в документах Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Поиск текста в электронных таблицах Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Поиск текста в презентациях Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Поиск текста в документах PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Искать текст в электронных письмах](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Поиск текста в электронных книгах EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Поиск текста в документах HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Поиск текста в разделах Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Примеры

В следующем примере показано, как выполнять поиск с помощью регулярного выражения в документе:

В следующем примере показано, как искать текст на страницах:

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Поиск по регулярному выражению с учетом регистра
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Проверяем, поддерживается ли поиск
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Перебираем результаты поиска
    foreach(SearchResult s in sr)
    {
        // Печатаем индекс и найденный текст:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Создаем экземпляр класса Parser
using(Parser parser = new Parser(filePath))
{
    // Поиск по ключевому слову с номерами страниц
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Проверяем, поддерживается ли поиск
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Перебираем результаты поиска
    foreach(SearchResult s in sr)
    {
        // Распечатать индекс, номер страницы и найденный текст:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Смотрите также

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
