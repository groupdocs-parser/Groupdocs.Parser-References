---
title: "TemplateTable"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет таблицу шаблона."
type: docs
weight: 20
url: /ru/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Предоставляет таблицу шаблона.

Существует два способа определить таблицу:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable) с именем в ВЕРХНЕМ РЕГИСТРЕ. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable) с именем в ВЕРХНЕМ РЕГИСТРЕ. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable) с именем в ВЕРХНЕМ РЕГИСТРЕ. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getLayout()](#getLayout--) | Получает макет таблицы. |
|
|  | [getParameters()](#getParameters--) | Получает параметры для обнаружения таблицы в автоматическом режиме. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable) с именем в ВЕРХНЕМ РЕГИСТРЕ.

Таблица шаблона задаётся макетом таблицы, если таблицу нельзя обнаружить автоматически:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Макет таблицы. |
|
|  | имя | java.lang.String | Имя таблицы. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой находится таблица шаблона;  null  если таблица шаблона расположена на любой странице. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable) с именем в ВЕРХНЕМ РЕГИСТРЕ.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Макет таблицы. |
|
|  | имя | java.lang.String | Имя таблицы. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой находится таблица шаблона;  null  если таблица шаблона расположена на любой странице. |
|
|  | pageWidth | java.lang.Double | Ширина страницы, использованной для создания элемента шаблона. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Макет таблицы. |
|
|  | имя | java.lang.String | Имя таблицы. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой находится таблица шаблона;  null  если таблица шаблона расположена на любой странице. |
|
|  | useUpperCaseName | boolean | Значение, указывающее, преобразуется ли  name  в ВЕРХНИЙ РЕГИСТР. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Макет таблицы. |
|
|  | имя | java.lang.String | Имя таблицы. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой находится таблица шаблона;  null  если таблица шаблона расположена на любой странице. |
|
|  | pageWidth | java.lang.Double | Ширина страницы, использованной для создания элемента шаблона. |
|
|  | useUpperCaseName | boolean | Значение, указывающее, преобразуется ли  name  в ВЕРХНИЙ РЕГИСТР. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable) с именем в ВЕРХНЕМ РЕГИСТРЕ.

Если таблица шаблона задаётся параметрами детектора, таблица обнаруживается автоматически:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Параметры для обнаружения таблицы в автоматическом режиме. |
|
|  | имя | java.lang.String | Имя таблицы. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой находится таблица шаблона;  null  если таблица шаблона расположена на любой странице. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Параметры для обнаружения таблицы в автоматическом режиме. |
|
|  | имя | java.lang.String | Имя таблицы. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой находится таблица шаблона;  null  если таблица шаблона расположена на любой странице. |
|
|  | pageWidth | java.lang.Double | Ширина страницы, использованной для создания элемента шаблона. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Параметры для обнаружения таблицы в автоматическом режиме. |
|
|  | имя | java.lang.String | Имя таблицы. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой находится таблица шаблона;  null  если таблица шаблона расположена на любой странице. |
|
|  | useUpperCaseName | boolean | Значение, указывающее, преобразуется ли  name  в ВЕРХНИЙ РЕГИСТР. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Инициализирует новый экземпляр класса [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Параметры для обнаружения таблицы в автоматическом режиме. |
|
|  | имя | java.lang.String | Имя таблицы. |
|
|  | pageIndex | java.lang.Integer | Индекс страницы, на которой находится таблица шаблона;  null  если таблица шаблона расположена на любой странице. |
|
|  | pageWidth | java.lang.Double | Ширина страницы, использованной для создания элемента шаблона. |
|
|  | useUpperCaseName | boolean | Значение, указывающее, преобразуется ли  name  в ВЕРХНИЙ РЕГИСТР. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Получает макет таблицы.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Получает параметры для обнаружения таблицы в автоматическом режиме.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Создаёт копию текущего элемента, масштабируя все координаты на заданный коэффициент.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| коэффициент | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
