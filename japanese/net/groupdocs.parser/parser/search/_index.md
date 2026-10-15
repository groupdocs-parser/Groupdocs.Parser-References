---
title: "Search"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ドキュメント内のキーワードを検索します。"
type: docs
weight: 250
url: /ja/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

ドキュメント内で*keyword*を検索します。

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| キーワード | 文字列 | 検索するキーワードです。 |

### 戻り値

[`SearchResult`](../../../groupdocs.parser.data/searchresult) オブジェクトのコレクション; 検索がサポートされていない場合は `null`。

### 備考

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

### 例

次の例は、ドキュメント内でキーワードを見つける方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // キーワードを検索する:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // 検索がサポートされているか確認する
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 検索結果を反復処理する
    foreach(SearchResult s in sr)
    {
        // インデックスと見つかったテキストを出力する:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### 関連項目

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

検索オプション（正規表現、大小文字の一致など）を使用してドキュメント内で*keyword*を検索します。

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| キーワード | 文字列 | 検索するキーワードです。 |
| options | SearchOptions | 検索オプションです。 |

### 戻り値

[`SearchResult`](../../../groupdocs.parser.data/searchresult) オブジェクトのコレクション; 検索がサポートされていない場合は `null`。

### 備考

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

### 例

次の例は、ドキュメントで正規表現を使用して検索する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // 大文字小文字を区別した正規表現で検索
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // 検索がサポートされているか確認する
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 検索結果を反復処理する
    foreach(SearchResult s in sr)
    {
        // インデックスと見つかったテキストを出力する:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

次の例はページ上でテキストを検索する方法を示しています:

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ページ番号付きでキーワードを検索
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // 検索がサポートされているか確認する
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 検索結果を反復処理する
    foreach(SearchResult s in sr)
    {
        // インデックス、ページ番号、見つかったテキストを出力:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### 関連項目

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
