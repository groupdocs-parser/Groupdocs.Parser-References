---
title: "Search"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "在文档中搜索关键字。"
type: docs
weight: 250
url: /zh/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

在文档中搜索 *keyword*。

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 关键字 | 字符串 | 要搜索的关键字。 |

### 返回值

[`SearchResult`](../../../groupdocs.parser.data/searchresult) 对象的集合；如果不支持搜索，则为 `null`。

### 备注

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

### 示例

下面的示例展示了如何在文档中查找关键字：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 搜索关键字：
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // 检查是否支持搜索
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 遍历搜索结果
    foreach(SearchResult s in sr)
    {
        // 打印索引和找到的文本：
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### 另请参见

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

使用搜索选项（正则表达式、区分大小写等）在文档中搜索 *keyword*。

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 关键字 | 字符串 | 要搜索的关键字。 |
| options | SearchOptions | 搜索选项。 |

### 返回值

[`SearchResult`](../../../groupdocs.parser.data/searchresult) 对象的集合；如果不支持搜索，则为 `null`。

### 备注

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

### 示例

下面的示例展示了如何在文档中使用正则表达式进行搜索：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 使用区分大小写的正则表达式搜索
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // 检查是否支持搜索
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 遍历搜索结果
    foreach(SearchResult s in sr)
    {
        // 打印索引和找到的文本：
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

下面的示例展示了如何在页面上搜索文本：

```csharp
// 创建 Parser 类的实例
using(Parser parser = new Parser(filePath))
{
    // 搜索带有页码的关键字
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // 检查是否支持搜索
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 遍历搜索结果
    foreach(SearchResult s in sr)
    {
        // 打印索引、页码和找到的文本：
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### 另请参见

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
