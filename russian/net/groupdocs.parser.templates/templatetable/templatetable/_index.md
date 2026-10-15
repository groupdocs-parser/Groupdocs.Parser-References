---
title: "TemplateTable"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Инициализирует новый экземпляр класса TemplateTablegroupdocs.parser.templates/templatetable с именем в верхнем регистре."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

Инициализирует новый экземпляр класса [`TemplateTable`](../../templatetable) с именем в верхнем регистре.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| layout | TemplateTableLayout | Макет таблицы. |
| имя | Строка | Имя таблицы. |

### Примеры

Таблица шаблона задаётся макетом таблицы, если таблицу нельзя определить автоматически:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Создать шаблон документа
Template template = new Template(new TemplateItem[] { table });
```

### См. также

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

Инициализирует новый экземпляр класса [`TemplateTable`](../../templatetable) с именем в верхнем регистре.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| layout | TemplateTableLayout | Макет таблицы. |
| имя | Строка | Имя таблицы. |
| pageWidth | Nullable`1 | Ширина страницы, использованной для создания элемента шаблона. |

### Примеры

Таблица шаблона задаётся макетом таблицы, если таблицу нельзя определить автоматически:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Создать шаблон документа
Template template = new Template(new TemplateItem[] { table });
```

### См. также

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

Инициализирует новый экземпляр класса [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| layout | TemplateTableLayout | Макет таблицы. |
| имя | Строка | Имя таблицы. |
| pageWidth | Nullable`1 | Ширина страницы, использованной для создания элемента шаблона. |
| useUpperCaseName | Boolean | Значение, указывающее, преобразуется ли `name` в ВЕРХНИЙ РЕГИСТР. |

### Примеры

Таблица шаблона задаётся макетом таблицы, если таблицу нельзя определить автоматически:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// Создать шаблон документа
Template template = new Template(new TemplateItem[] { table });
```

### См. также

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

Инициализирует новый экземпляр класса [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| параметры | TemplateTableParameters | Параметры для обнаружения таблицы в автоматическом режиме. |
| имя | Строка | Имя таблицы. |

### Примеры

Если таблица шаблона задаётся параметрами детектора, таблица обнаруживается автоматически:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// Создать шаблон документа
Template template = new Template(new TemplateItem[] { table });
```

### См. также

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

Инициализирует новый экземпляр класса [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| параметры | TemplateTableParameters | Параметры для обнаружения таблицы в автоматическом режиме. |
| имя | Строка | Имя таблицы. |
| pageWidth | Nullable`1 | Ширина страницы, использованной для создания элемента шаблона. |

### Примеры

Если таблица шаблона задаётся параметрами детектора, таблица обнаруживается автоматически:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Создать шаблон документа
Template template = new Template(new TemplateItem[] { table });
```

### См. также

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

Инициализирует новый экземпляр класса [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| параметры | TemplateTableParameters | Параметры для обнаружения таблицы в автоматическом режиме. |
| имя | Строка | Имя таблицы. |
| pageWidth | Nullable`1 | Ширина страницы, использованной для создания элемента шаблона. |
| useUpperCaseName | Boolean | Значение, указывающее, преобразуется ли `name` в ВЕРХНИЙ РЕГИСТР. |

### Примеры

Если таблица шаблона задаётся параметрами детектора, таблица обнаруживается автоматически:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Создать шаблон документа
Template template = new Template(new TemplateItem[] { table });
```

### См. также

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
