---
title: Search
second_title: GroupDocs.Parser for .NET API リファレンス
description: 検索しますkeywordドキュメント内.
type: docs
weight: 200
url: /ja/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

検索します*keyword*ドキュメント内.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| keyword | String | 検索するキーワード。 |

### 戻り値

のコレクション[`SearchResult`](../../../groupdocs.parser.data/searchresult)オブジェクト; `ヌル`検索がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [テキスト検索](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Microsoft Office Word 文書のテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Microsoft Office Excel スプレッドシートのテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint プレゼンテーションのテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [PDF ドキュメント内のテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [メール内のテキストを検索](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [EPUB 電子書籍のテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [HTML ドキュメント内のテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Microsoft OneNote セクションのテキストを検索](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### 例

次の例は、ドキュメント内のキーワードを検索する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // キーワードを検索:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // 検索がサポートされているかどうかを確認します
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 検索結果を繰り返す
    foreach(SearchResult s in sr)
    {
        // インデックスと見つかったテキストを出力します:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### 関連項目

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

検索します*keyword*検索オプション (正規表現、大文字と小文字の一致など) を使用してドキュメント内で。

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| keyword | String | 検索するキーワード。 |
| options | SearchOptions | 検索オプション。 |

### 戻り値

のコレクション[`SearchResult`](../../../groupdocs.parser.data/searchresult)オブジェクト; `ヌル`検索がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [テキスト検索](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Microsoft Office Word 文書のテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Microsoft Office Excel スプレッドシートのテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint プレゼンテーションのテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [PDF ドキュメント内のテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [メール内のテキストを検索](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [EPUB 電子書籍のテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [HTML ドキュメント内のテキストを検索する](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Microsoft OneNote セクションのテキストを検索](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### 例

次の例は、ドキュメント内で正規表現を使用して検索する方法を示しています。

次の例は、ページ上のテキストを検索する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // 大文字と小文字を一致させた正規表現で検索
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // 検索がサポートされているかどうかを確認します
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 検索結果を繰り返す
    foreach(SearchResult s in sr)
    {
        // インデックスと見つかったテキストを出力します:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ページ番号でキーワードを検索
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // 検索がサポートされているかどうかを確認します
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // 検索結果を繰り返す
    foreach(SearchResult s in sr)
    {
        // インデックス、ページ番号、見つかったテキストを表示:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### 関連項目

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
