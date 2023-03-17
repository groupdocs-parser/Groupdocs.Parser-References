---
title: GetTextAreas
second_title: GroupDocs.Parser for .NET API リファレンス
description: ドキュメントからテキスト領域を抽出します
type: docs
weight: 160
url: /ja/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

ドキュメントからテキスト領域を抽出します。

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### 戻り値

のコレクション[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)オブジェクト; `ヌル`テキスト領域の抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [テキスト領域を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 例

次の例は、ドキュメント全体からすべてのテキスト領域を抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // テキスト領域を抽出する
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // テキスト領域の抽出がサポートされているかどうかを確認します
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // ページのテキスト領域を繰り返します
    foreach(PageTextArea a in areas)
    {
        // ページ インデックス、四角形、テキスト領域の値を出力します。
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

カスタマイズ オプション (正規表現、大文字と小文字の一致など) を使用してドキュメントからテキスト領域を抽出します。

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| options | PageTextAreaOptions | テキスト領域抽出のオプション。 |

### 戻り値

のコレクション[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)オブジェクト; `ヌル`テキスト領域の抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [テキスト領域を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 例

次の例は、左上隅から数字を含むテキスト領域のみを抽出する方法を示しています。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // テキスト領域の抽出に使用されるオプションを作成します
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // ページの左上隅から数字のみを含むテキスト領域を抽出します。
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // テキスト領域の抽出がサポートされているかどうかを確認します
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // ページのテキスト領域を繰り返します
    foreach(PageTextArea a in areas)
    {
        // ページ インデックス、四角形、テキスト領域の値を出力します。
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

ドキュメント ページからテキスト領域を抽出します。

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | ゼロベースのページ インデックス。 |

### 戻り値

のコレクション[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)オブジェクト; `ヌル`テキスト領域の抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [テキスト領域を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 例

ドキュメント ページからテキスト領域を抽出するには、次の方法を使用します。

```csharp
// Parser クラスのインスタンスを作成します
using(Parser parser = new Parser(filePath))
{
    // ドキュメントがテキスト領域の抽出をサポートしているかどうかを確認します
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // ドキュメント情報を取得する
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // ドキュメントにページがあるかどうかを確認します
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // ページを繰り返す
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // ページ番号を出力 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // ページのテキスト領域を繰り返します
        // テキスト領域抽出機能のサポートを以前に確認したため、null チェックは無視します
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // 四角形とテキスト エリアの値を出力します。
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

カスタマイズ オプション (正規表現、大文字と小文字の一致など) を使用してドキュメント ページからテキスト領域を抽出します。

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| pageIndex | Int32 | ゼロベースのページ インデックス。 |
| options | PageTextAreaOptions | テキスト領域抽出のオプション。 |

### 戻り値

のコレクション[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea)オブジェクト; `ヌル`テキスト領域の抽出がサポートされていない場合.

### 備考

**もっと詳しく知る：**

* [テキスト領域を抽出する](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### 関連項目

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* 名前空間 [GroupDocs.Parser](../../parser)
* 組み立て [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
