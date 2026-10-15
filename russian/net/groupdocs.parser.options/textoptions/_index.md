---
title: "TextOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Предоставляет параметры, используемые для извлечения текста."
type: docs
weight: 610
url: /ru/net/groupdocs.parser.options/textoptions/
---

## TextOptions class

Предоставляет параметры, используемые для извлечения текста.

```csharp
public sealed class TextOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TextOptions](textoptions#constructor)() | Инициализирует новый экземпляр класса [`TextOptions`](../textoptions). |
| [TextOptions](textoptions#constructor_1)(bool) | Инициализирует новый экземпляр класса [`TextOptions`](../textoptions). |
| [TextOptions](textoptions#constructor_2)(bool, bool) | Инициализирует новый экземпляр класса [`TextOptions`](../textoptions) с параметром использования OCR. |
| [TextOptions](textoptions#constructor_3)(bool, bool, OcrOptions) | Инициализирует новый экземпляр класса [`TextOptions`](../textoptions) с возможностью задавать параметры OCR. |

## Свойства

| Имя | Описание |
| --- | --- |
| [IncludeAnnotations](../../groupdocs.parser.options/textoptions/includeannotations) { get; set; } | Возвращает значение, указывающее, включены ли аннотации. Значение по умолчанию — `false`. |
| [OcrOptions](../../groupdocs.parser.options/textoptions/ocroptions) { get; set; } | Возвращает дополнительные параметры для функциональности OCR. |
| [UseOcr](../../groupdocs.parser.options/textoptions/useocr) { get; set; } | Возвращает значение, указывающее, используется ли OCR Connector для извлечения текста. |
| [UseRawModeIfPossible](../../groupdocs.parser.options/textoptions/userawmodeifpossible) { get; set; } | Возвращает значение, указывающее, используется ли необработанный режим. |

### Примечания

Экземпляр класса [`TextOptions`](../textoptions) используется в качестве параметра методов [`GetText`](../../groupdocs.parser/parser/gettext) и [`GetText`](../../groupdocs.parser/parser/gettext). См. примеры использования там.

Используется для указания необработанного режима извлечения текста. Текст в этом режиме извлекается менее точно, но быстрее, чем в стандартном режиме. Если необработанный режим не поддерживает формат документа, этот параметр игнорируется и используется стандартный режим.

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### См. также

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
