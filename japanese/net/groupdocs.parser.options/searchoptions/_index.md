---
title: "SearchOptions"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "テキスト検索に使用されるオプションを提供します。"
type: docs
weight: 590
url: /ja/net/groupdocs.parser.options/searchoptions/
---

## SearchOptions class

テキスト検索に使用されるオプションを提供します。

```csharp
public sealed class SearchOptions
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [SearchOptions](searchoptions#constructor)() | デフォルト値で[`SearchOptions`](../searchoptions)クラスの新しいインスタンスを初期化します。詳細は備考をご覧ください。 |
| [SearchOptions](searchoptions#constructor_1)(bool, bool, bool) | ハイライト抽出なしで検索するために使用される[`SearchOptions`](../searchoptions)クラスの新しいインスタンスを初期化します。 |
| [SearchOptions](searchoptions#constructor_2)(bool, bool, bool, bool) | ページ単位で検索し、ハイライト抽出なしで検索するために使用される[`SearchOptions`](../searchoptions)クラスの新しいインスタンスを初期化します。 |
| [SearchOptions](searchoptions#constructor_4)(bool, bool, bool, HighlightOptions) | 左側と右側のハイライト抽出に同じハイライトオプションを使用して検索するために使用される[`SearchOptions`](../searchoptions)クラスの新しいインスタンスを初期化します。 |
| [SearchOptions](searchoptions#constructor_5)(bool, bool, bool, HighlightOptions, HighlightOptions) | 左側と右側のハイライト抽出のハイライトオプションを使用して検索するために使用される[`SearchOptions`](../searchoptions)クラスの新しいインスタンスを初期化します。 |
| [SearchOptions](searchoptions#constructor_3)(bool, bool, bool, bool, HighlightOptions, HighlightOptions) | [`SearchOptions`](../searchoptions)クラスの新しいインスタンスを初期化します。 |
| [SearchOptions](searchoptions#constructor_6)(bool, bool, bool, int, HighlightOptions, HighlightOptions) | ページ制限付きで[`SearchOptions`](../searchoptions)クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [LeftHighlightOptions](../../groupdocs.parser.options/searchoptions/lefthighlightoptions) { get; set; } | 左側ハイライトのオプションを取得します。 |
| [MatchCase](../../groupdocs.parser.options/searchoptions/matchcase) { get; set; } | テキストの大文字小文字が無視されていないかどうかを示す値を取得します。 |
| [MatchWholeWord](../../groupdocs.parser.options/searchoptions/matchwholeword) { get; set; } | テキスト検索が単語全体で制限されているかどうかを示す値を取得します。 |
| [MaxPageIndex](../../groupdocs.parser.options/searchoptions/maxpageindex) { get; set; } | 検索対象ページの最大インデックスを表す値を取得します。 |
| [RightHighlightOptions](../../groupdocs.parser.options/searchoptions/righthighlightoptions) { get; set; } | 右側ハイライトのオプションを取得します。 |
| [SearchByPages](../../groupdocs.parser.options/searchoptions/searchbypages) { get; set; } | 検索がページ単位で実行されるかどうかを示す値を取得します。 |
| [UseRegularExpression](../../groupdocs.parser.options/searchoptions/useregularexpression) { get; set; } | 正規表現が使用されているかどうかを示す値を取得します。 |

### 備考

[`SearchOptions`](../searchoptions)クラスのインスタンスは[`Search`](../../groupdocs.parser/parser/search)メソッドのパラメーターとして使用されます。使用例はそちらをご覧ください。

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

### 関連項目

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
