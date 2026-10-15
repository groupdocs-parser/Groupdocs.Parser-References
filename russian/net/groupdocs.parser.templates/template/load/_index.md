---
title: "Загрузить"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Загружает шаблон из файла."
type: docs
weight: 20
url: /ru/net/groupdocs.parser.templates/template/load/
---

## Load(string) {#load_1}

Загружает шаблон из файла.

```csharp
public static Template Load(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | Строка | Путь к файлу. |

### Возвращаемое значение

Экземпляр класса [`Template`](../../template) с загруженным шаблоном.

### Exceptions

| exception | condition |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | Файл не представляет шаблон в корректном формате. |

### См. также

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Load(Stream) {#load}

Загружает шаблон из потока.

```csharp
public static Template Load(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Входной поток. |

### Возвращаемое значение

Экземпляр класса [`Template`](../../template) с загруженным шаблоном.

### Exceptions

| exception | condition |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | Поток не представляет шаблон в корректном формате. |

### См. также

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
