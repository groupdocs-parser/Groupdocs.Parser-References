---
title: "SearchOptions"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Инициализирует новый экземпляр класса SearchOptionsgroupdocs.parser.options/searchoptions."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.options/searchoptions/searchoptions/
---

## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Инициализирует новый экземпляр класса [`SearchOptions`](../../searchoptions).

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |
| searchByPages | Boolean | Значение, указывающее, выполняется ли поиск по страницам. |
| leftHighlightOptions | HighlightOptions | Параметры для левого выделения. |
| rightHighlightOptions | HighlightOptions | Параметры для правого выделения. |

### См. также

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, int, HighlightOptions, HighlightOptions) {#constructor_6}

Инициализирует новый экземпляр класса [`SearchOptions`](../../searchoptions) с ограничением по страницам.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    int maxPageIndex, HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |
| maxPageIndex | Int32 | Значение, указывающее, выполняется ли поиск по страницам. |
| leftHighlightOptions | HighlightOptions | Параметры для левого выделения. |
| rightHighlightOptions | HighlightOptions | Параметры для правого выделения. |

### См. также

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Инициализирует новый экземпляр класса [`SearchOptions`](../../searchoptions), который используется для поиска с параметрами выделения для извлечения левого и правого выделения.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |
| leftHighlightOptions | HighlightOptions | Параметры для левого выделения. |
| rightHighlightOptions | HighlightOptions | Параметры для правого выделения. |

### См. также

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Инициализирует новый экземпляр класса [`SearchOptions`](../../searchoptions), который используется для поиска с одинаковыми параметрами выделения для извлечения левого и правого выделения.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |
| highlightOptions | HighlightOptions | Параметры для обоих выделений. |

### См. также

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Инициализирует новый экземпляр класса [`SearchOptions`](../../searchoptions), который используется для поиска без извлечения выделения.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |

### См. также

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Инициализирует новый экземпляр класса [`SearchOptions`](../../searchoptions), который используется для поиска по страницам и без извлечения выделения.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли поиск текста целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |
| searchByPages | Boolean | Значение, указывающее, выполняется ли поиск по страницам. |

### См. также

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Инициализирует новый экземпляр класса [`SearchOptions`](../../searchoptions) со значениями по умолчанию. См. примечания для подробностей.

```csharp
public SearchOptions()
```

### Примечания

Следующие свойства имеют значения по умолчанию:

**[`MatchCase`](../matchcase)**

`false`

**[`MatchWholeWord`](../matchwholeword)**

`false`

**[`UseRegularExpression`](../useregularexpression)**

`false`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`null`

**[`RightHighlightOptions`](../righthighlightoptions)**

`null`

### См. также

* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
