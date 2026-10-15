---
title: "РазборПоШаблону"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Разбирает документ с помощью пользовательского шаблона."
type: docs
weight: 230
url: /ru/net/groupdocs.parser/parser/parsebytemplate/
---

## ParseByTemplate(Template) {#parsebytemplate}

Разбирает документ с помощью пользовательского шаблона.

```csharp
public DocumentData ParseByTemplate(Template template)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| шаблон | Шаблон | Пользовательский шаблон. |

### Возвращаемое значение

Экземпляр класса [`DocumentData`](../../../groupdocs.parser.data/documentdata), содержащего извлечённые данные; `null`, если разбор по шаблону не поддерживается.

### Примечания

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### См. также

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(Template, ParseByTemplateOptions) {#parsebytemplate_1}

Разбирает документ с помощью пользовательского шаблона, используя параметры настройки.

```csharp
public DocumentData ParseByTemplate(Template template, ParseByTemplateOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| шаблон | Шаблон | Пользовательский шаблон. |
| options | ParseByTemplateOptions | Параметры настройки. |

### Возвращаемое значение

Экземпляр класса [`DocumentData`](../../../groupdocs.parser.data/documentdata), содержащего извлечённые данные; `null`, если разбор по шаблону не поддерживается.

### Примечания

**Learn more:**

* [Parse data from documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+documents)
* [Working with templates](https://docs.groupdocs.com/display/parsernet/Working+with+templates)
* [Working with data extracted by template](https://docs.groupdocs.com/display/parsernet/Working+with+data+extracted+by+template)
* [Parse data from PDF documents](https://docs.groupdocs.com/display/parsernet/Parse+data+from+PDF+documents)

### См. также

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Template](../../../groupdocs.parser.templates/template)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## ParseByTemplate(TemplateCollection, ParseByTemplateOptions) {#parsebytemplate_2}

Выбирает наиболее подходящий шаблон из предоставленной коллекции, а затем разбирает документ согласно выбранному шаблону.

```csharp
public DocumentData ParseByTemplate(TemplateCollection templateCollection, 
    ParseByTemplateOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| templateCollection | TemplateCollection | Коллекция шаблонов. |
| options | ParseByTemplateOptions | Параметры настройки. |

### Возвращаемое значение

Экземпляр класса [`DocumentData`](../../../groupdocs.parser.data/documentdata), содержащего извлечённые данные; `null`, если разбор по шаблону не поддерживается.

### См. также

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [TemplateCollection](../../../groupdocs.parser.templates/templatecollection)
* class [ParseByTemplateOptions](../../../groupdocs.parser.options/parsebytemplateoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
