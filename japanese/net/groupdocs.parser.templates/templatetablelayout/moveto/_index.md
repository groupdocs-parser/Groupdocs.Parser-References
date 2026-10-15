---
title: "MoveTo"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ポイント内で同じサイズの区切りと位置を持つ新しいレイアウトを作成します。"
type: docs
weight: 50
url: /ja/net/groupdocs.parser.templates/templatetablelayout/moveto/
---

## TemplateTableLayout.MoveTo method

*point* において同じサイズ、区切り文字、位置を持つ新しいレイアウトを作成します。

```csharp
public TemplateTableLayout MoveTo(Point point)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| point | Point | 新しいレイアウトの位置です。 |

### 戻り値

*point* 内で同じサイズ、区切り、位置を持つ新しいレイアウトです。

### 例

この機能により Table Layout を移動できます。

例えば、ドキュメントの各ページにテーブルがある（またはページにテーブルがある複数のドキュメントがある）場合です。これらのテーブルは位置と内容が異なりますが、列と行は同じです。この場合、ユーザーは `(0, 0)` に一度だけ [`TemplateTableLayout`](../../templatetablelayout) オブジェクトを定義し、特定のテーブルの位置へ移動させることができます。

テーブルの位置がページ上の他のオブジェクトに依存する場合、ユーザーはテンプレートドキュメントに基づいて [`TemplateTableLayout`](../../templatetablelayout) オブジェクトを定義し、アンカーオブジェクトに従って移動させることができます。例えば、これがサマリーテーブルで、続いて詳細テーブル（行数が異なる場合があります）がある場合です。この場合、ユーザーはテンプレートドキュメント上で（既知の詳細テーブルの矩形を持つ）[`TemplateTableLayout`](../../templatetablelayout) オブジェクトを定義し、テンプレートと実際のドキュメントの詳細テーブル矩形の差分に従って [`TemplateTableLayout`](../../templatetablelayout) オブジェクトを移動させます。

`MoveTo` メソッドは現在のオブジェクトのコピーを返します。ユーザーは任意の座標（負の値でも可）を渡すことができ、その場合レイアウトは左または上に移動します。

```csharp
// テーブルレイアウトを作成する
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 0, 25, 150, 180, 230 },
    new double[] { 0, 15, 30, 45, 60, 75 });

// 矩形を印刷する
Rectangle rect = layout.Rectangle;

// 出力: 位置: (0, 0) サイズ: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", rect.Left, rect.Top, rect.Size.Width, rect.Size.Height));

// レイアウトを指定されたテーブル位置へ移動する
TemplateTableLayout movedLayout = layout.MoveTo(new Point(315, 250));

// 最初の区切りが移動されたことを確認してください:
Console.WriteLine(movedLayout.VerticalSeparators[0]); // prints: 315
Console.WriteLine(movedLayout.HorizontalSeparators[0]); // prints: 250

Rectangle movedRect = movedLayout.Rectangle;

// 出力: 位置: (315, 250) サイズ: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", movedRect.Left, movedRect.Top, movedRect.Size.Width, movedRect.Size.Height));

// movedLayout オブジェクトは layout オブジェクトのコピーであるため、元のレイアウトに影響を与えずに区切りを調整できます:
movedLayout.HorizontalSeparators.Add(90);

Console.WriteLine(movedLayout.HorizontalSeparators.Count); // prints: 7
Console.WriteLine(layout.HorizontalSeparators.Count); // prints: 6
```

### 関連項目

* class [Point](../../../groupdocs.parser.data/point)
* class [TemplateTableLayout](../../templatetablelayout)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
