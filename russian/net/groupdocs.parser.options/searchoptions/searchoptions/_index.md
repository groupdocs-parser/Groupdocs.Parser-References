---
title: SearchOptions
second_title: Справочник по API GroupDocs.Parser для .NET
description: Инициализирует новый экземплярSearchOptionsgroupdocs.parser.options/searchoptions класс.
type: docs
weight: 10
url: /ru/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Инициализирует новый экземпляр[`SearchOptions`](../../searchoptions) класс.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли текстовый поиск целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |
| searchByPages | Boolean | Значение, указывающее, выполняется ли поиск по страницам. |
| leftHighlightOptions | HighlightOptions | Параметры для левой подсветки. |
| rightHighlightOptions | HighlightOptions | Варианты правильной подсветки. |

### Смотрите также

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* пространство имен [GroupDocs.Parser.Options](../../searchoptions)
* сборка [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Инициализирует новый экземпляр[`SearchOptions`](../../searchoptions) класс, который используется для search с параметрами выделения для выделения левого и правого выделения.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли текстовый поиск целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |
| leftHighlightOptions | HighlightOptions | Параметры для левой подсветки. |
| rightHighlightOptions | HighlightOptions | Варианты правильной подсветки. |

### Смотрите также

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* пространство имен [GroupDocs.Parser.Options](../../searchoptions)
* сборка [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Инициализирует новый экземпляр[`SearchOptions`](../../searchoptions) класс, который используется для search с одинаковыми параметрами выделения для выделения левого и правого выделения.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли текстовый поиск целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |
| highlightOptions | HighlightOptions | Варианты для обоих основных моментов. |

### Смотрите также

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* пространство имен [GroupDocs.Parser.Options](../../searchoptions)
* сборка [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Инициализирует новый экземпляр[`SearchOptions`](../../searchoptions) класс, который используется для search без извлечения выделения.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли текстовый поиск целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |

### Смотрите также

* class [SearchOptions](../../searchoptions)
* пространство имен [GroupDocs.Parser.Options](../../searchoptions)
* сборка [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Инициализирует новый экземпляр[`SearchOptions`](../../searchoptions) класс, который используется для поиска по страницам и без извлечения выделения.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| matchCase | Boolean | Значение, указывающее, не игнорируется ли регистр текста. |
| matchWholeWord | Boolean | Значение, указывающее, ограничен ли текстовый поиск целым словом. |
| useRegularExpression | Boolean | Значение, указывающее, используется ли регулярное выражение. |
| searchByPages | Boolean | Значение, указывающее, выполняется ли поиск по страницам. |

### Смотрите также

* class [SearchOptions](../../searchoptions)
* пространство имен [GroupDocs.Parser.Options](../../searchoptions)
* сборка [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Инициализирует новый экземпляр[`SearchOptions`](../../searchoptions) класс со значениями по умолчанию. Подробнее см. в примечаниях.

```csharp
public SearchOptions()
```

### Примечания

Следующие свойства имеют значения по умолчанию:

**[`MatchCase`](../matchcase)**

`ЛОЖЬ`

**[`MatchWholeWord`](../matchwholeword)**

`ЛОЖЬ`

**[`UseRegularExpression`](../useregularexpression)**

`ЛОЖЬ`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`нулевой`

**[`RightHighlightOptions`](../righthighlightoptions)**

`нулевой`

### Смотрите также

* class [SearchOptions](../../searchoptions)
* пространство имен [GroupDocs.Parser.Options](../../searchoptions)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
