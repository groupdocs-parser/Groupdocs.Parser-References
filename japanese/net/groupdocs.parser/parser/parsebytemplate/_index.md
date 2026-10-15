---
title: "ParseByTemplate"
second_title: "GroupDocs.Parser for .NET API リファレンス"
description: "ユーザー生成テンプレートでドキュメントを解析します。"
type: docs
weight: 230
url: /ja/net/groupdocs.parser/parser/parsebytemplate/
---

## ParseByTemplate(Template) {#parsebytemplate}

ユーザー作成テンプレートでドキュメントを解析します。

```csharp
public DocumentData ParseByTemplate(Template template)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| テンプレート | テンプレート | ユーザー生成テンプレート。 |

### 戻り値

抽出されたデータを含む [`DocumentData`](../../../groupdocs.parser.data/documentdata) クラスのインスタンス; テンプレートによる解析がサポートされていない場合は `null`。

### 備考

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### 関連項目

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(Template, ParseByTemplateOptions) {#parsebytemplate_1}

カスタマイズオプションを使用してユーザー作成テンプレートでドキュメントを解析します。

```csharp
public DocumentData ParseByTemplate(Template template, ParseByTemplateOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| テンプレート | テンプレート | ユーザー生成テンプレート。 |
| options | ParseByTemplateOptions | カスタマイズオプション。 |

### 戻り値

抽出されたデータを含む [`DocumentData`](../../../groupdocs.parser.data/documentdata) クラスのインスタンス; テンプレートによる解析がサポートされていない場合は `null`。

### 備考

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### 関連項目

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(TemplateCollection, ParseByTemplateOptions) {#parsebytemplate_2}

提供されたコレクションから最適なテンプレートを選択し、選択したテンプレートに対してドキュメントを解析します。

```csharp
public DocumentData ParseByTemplate(TemplateCollection templateCollection, 
    ParseByTemplateOptions options)
```

| Parameter | Type | 説明 |
| --- | --- | --- |
| templateCollection | TemplateCollection | テンプレートコレクション。 |
| options | ParseByTemplateOptions | カスタマイズオプション。 |

### 戻り値

抽出されたデータを含む [`DocumentData`](../../../groupdocs.parser.data/documentdata) クラスのインスタンス; テンプレートによる解析がサポートされていない場合は `null`。

### 関連項目

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [TemplateCollection](../../../groupdocs.parser.templates/templatecollection)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- 編集しないでください: xmldocmd によって GroupDocs.Parser.dll 用に生成されました -->
