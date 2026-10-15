---
title: "TemplateTable"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "大文字の名前で TemplateTablegroupdocs.parser.templates/templatetable クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

大文字の名前で [`TemplateTable`](../../templatetable) クラスの新しいインスタンスを初期化します。

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| layout | TemplateTableLayout | テーブルレイアウトです。 |
| name | 文字列 | テーブル名です。 |

### 例

テーブルが自動的に検出できない場合、テーブルレイアウトによってテンプレートテーブルが設定されます:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// ドキュメントテンプレートを作成
Template template = new Template(new TemplateItem[] { table });
```

### 関連項目

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

大文字の名前で [`TemplateTable`](../../templatetable) クラスの新しいインスタンスを初期化します。

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| layout | TemplateTableLayout | テーブルレイアウトです。 |
| name | 文字列 | テーブル名です。 |
| pageWidth | Nullable`1 | テンプレート項目の作成に使用されたページの幅です。 |

### 例

テーブルが自動的に検出できない場合、テーブルレイアウトによってテンプレートテーブルが設定されます:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// ドキュメントテンプレートを作成
Template template = new Template(new TemplateItem[] { table });
```

### 関連項目

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

[`TemplateTable`](../../templatetable) クラスの新しいインスタンスを初期化します。

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| layout | TemplateTableLayout | テーブルレイアウトです。 |
| name | 文字列 | テーブル名です。 |
| pageWidth | Nullable`1 | テンプレート項目の作成に使用されたページの幅です。 |
| useUpperCaseName | Boolean | `name` が大文字に変換されたかどうかを示す値です。 |

### 例

テーブルが自動的に検出できない場合、テーブルレイアウトによってテンプレートテーブルが設定されます:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// ドキュメントテンプレートを作成
Template template = new Template(new TemplateItem[] { table });
```

### 関連項目

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

[`TemplateTable`](../../templatetable) クラスの新しいインスタンスを初期化します。

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| パラメータ | TemplateTableParameters | 自動モードでテーブルを検出するためのパラメータです。 |
| name | 文字列 | テーブル名です。 |

### 例

検出器パラメータでテンプレートテーブルが設定されている場合、テーブルは自動的に検出されます:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// ドキュメントテンプレートを作成
Template template = new Template(new TemplateItem[] { table });
```

### 関連項目

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

[`TemplateTable`](../../templatetable) クラスの新しいインスタンスを初期化します。

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| パラメータ | TemplateTableParameters | 自動モードでテーブルを検出するためのパラメータです。 |
| name | 文字列 | テーブル名です。 |
| pageWidth | Nullable`1 | テンプレート項目の作成に使用されたページの幅です。 |

### 例

検出器パラメータでテンプレートテーブルが設定されている場合、テーブルは自動的に検出されます:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// ドキュメントテンプレートを作成
Template template = new Template(new TemplateItem[] { table });
```

### 関連項目

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

[`TemplateTable`](../../templatetable) クラスの新しいインスタンスを初期化します。

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| パラメータ | TemplateTableParameters | 自動モードでテーブルを検出するためのパラメータです。 |
| name | 文字列 | テーブル名です。 |
| pageWidth | Nullable`1 | テンプレート項目の作成に使用されたページの幅です。 |
| useUpperCaseName | Boolean | `name` が大文字に変換されたかどうかを示す値です。 |

### 例

検出器パラメータでテンプレートテーブルが設定されている場合、テーブルは自動的に検出されます:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// ドキュメントテンプレートを作成
Template template = new Template(new TemplateItem[] { table });
```

### 関連項目

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
