---
title: "Search"
second_title: "GroupDocs.Parser .NET용 API 레퍼런스"
description: "문서에서 키워드를 검색합니다."
type: docs
weight: 250
url: /ko/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

문서에서 *keyword*를 검색합니다.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 키워드 | 문자열 | 검색할 키워드입니다. |

### 반환 값

[`SearchResult`](../../../groupdocs.parser.data/searchresult) 객체의 컬렉션; 검색이 지원되지 않으면 `null`입니다.

### 비고

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

### 예제

다음 예제는 문서에서 키워드를 찾는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 키워드 검색:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // 검색이 지원되는지 확인합니다
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 검색 결과를 순회합니다
    foreach(SearchResult s in sr)
    {
        // 인덱스와 찾은 텍스트를 출력합니다:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### 참고

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

검색 옵션(정규식, 대소문자 구분 등)을 사용하여 문서에서 *keyword*를 검색합니다.

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 키워드 | 문자열 | 검색할 키워드입니다. |
| options | SearchOptions | 검색 옵션입니다. |

### 반환 값

[`SearchResult`](../../../groupdocs.parser.data/searchresult) 객체의 컬렉션; 검색이 지원되지 않으면 `null`입니다.

### 비고

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

### 예제

다음 예제는 문서에서 정규 표현식을 사용하여 검색하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 대소문자 구분을 포함한 정규식으로 검색
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // 검색이 지원되는지 확인합니다
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 검색 결과를 순회합니다
    foreach(SearchResult s in sr)
    {
        // 인덱스와 찾은 텍스트를 출력합니다:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

다음 예제는 페이지에서 텍스트를 검색하는 방법을 보여줍니다:

```csharp
// Parser 클래스의 인스턴스를 생성합니다
using(Parser parser = new Parser(filePath))
{
    // 페이지 번호와 함께 키워드 검색
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // 검색이 지원되는지 확인합니다
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 검색 결과를 순회합니다
    foreach(SearchResult s in sr)
    {
        // 인덱스, 페이지 번호 및 찾은 텍스트를 출력합니다:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### 참고

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
