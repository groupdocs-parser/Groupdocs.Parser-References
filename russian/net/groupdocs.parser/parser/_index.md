---
title: Parser
second_title: Справочник по API GroupDocs.Parser для .NET
description: Представляет основной класс управляющий текстом изображениями извлечением контейнеров и функциями синтаксического анализа.
type: docs
weight: 640
url: /ru/net/groupdocs.parser/parser/
---
## Parser class

Представляет основной класс, управляющий текстом, изображениями, извлечением контейнеров и функциями синтаксического анализа.

```csharp
public sealed class Parser : IDisposable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Инициализирует новый экземпляр[`Parser`](../parser) класс для извлечения данных из базы данных. |
| [Parser](parser#constructor)(EmailConnection) | Инициализирует новый экземпляр[`Parser`](../parser) класс для извлечения данных с удаленного почтового сервера. |
| [Parser](parser#constructor_4)(Stream) | Инициализирует новый экземпляр[`Parser`](../parser) класс. |
| [Parser](parser#constructor_8)(string) | Инициализирует новый экземпляр[`Parser`](../parser) класс. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Инициализирует новый экземпляр[`Parser`](../parser) класс для извлечения данных из базы данных. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Инициализирует новый экземпляр[`Parser`](../parser) класс для извлечения данных с удаленного почтового сервера. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Инициализирует новый экземпляр[`Parser`](../parser) класс с[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Инициализирует новый экземпляр[`Parser`](../parser) класс с[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | Инициализирует новый экземпляр[`Parser`](../parser) класс с[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | Инициализирует новый экземпляр[`Parser`](../parser) класс с[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Инициализирует новый экземпляр[`Parser`](../parser) класс с[`LoadOptions`](../../groupdocs.parser.options/loadoptions) и[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Инициализирует новый экземпляр[`Parser`](../parser) класс с[`LoadOptions`](../../groupdocs.parser.options/loadoptions) и[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Получает поддерживаемые функции. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Выполняет определяемые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Получить предварительный просмотр страниц. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Извлекает штрих-коды из документа. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Извлекает штрих-коды со страницы документа. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Извлекает штрих-коды из документа с помощью параметров настройки (для установки прямоугольной области, содержащей штрих-коды). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Извлекает штрих-коды со страницы документа с помощью параметров настройки (для установки прямоугольной области, содержащей штрих-коды). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Извлекает объект-контейнер из документа для работы с форматами, содержащими вложения, ZIP-архивы и т. д. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Возвращает общую информацию о документе. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Извлекает форматированный текст из документа. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Извлекает форматированный текст со страницы документа. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Извлекает выделение из документа. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Извлекает гиперссылки из документа. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Извлекает гиперссылки со страницы документа. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Извлекает гиперссылки из документа с помощью параметров настройки (для установки прямоугольной области, содержащей гиперссылки). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Извлекает гиперссылки со страницы документа с помощью параметров настройки (для установки прямоугольной области, содержащей гиперссылки). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Извлекает изображения из документа. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Извлекает изображения со страницы документа. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Извлекает изображения из документа с помощью параметров настройки (для установки прямоугольной области, содержащей изображения). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Извлекает изображения со страницы документа с помощью параметров настройки (для установки прямоугольной области, содержащей изображения). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Извлекает метаданные из документа. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Извлекает структурированный текст из документа. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Извлекает таблицы из документа. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Извлекает таблицы со страницы документа. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Извлекает текст из документа. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Извлекает текст со страницы документа. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Извлекает текстовую страницу из документа с помощью параметров текста (чтобы включить режим быстрого извлечения необработанного текста). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Извлекает текст со страницы документа с помощью параметров текста (чтобы включить режим быстрого извлечения необработанного текста). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Извлекает текстовые области из документа. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Извлекает текстовые области со страницы документа. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Извлекает текстовые области из документа, используя параметры настройки (регулярное выражение, регистр и т. д.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Извлекает текстовые области со страницы документа, используя параметры настройки (регулярное выражение, регистр и т. д.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Извлекает оглавление из документа. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Разбирает документ по созданному пользователем шаблону. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Разбирает форму документа. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Ищет*keyword* в документе. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Ищет*keyword*в документе с помощью параметров поиска (регулярное выражение, регистр и т. д.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Возвращает общую информацию о файле. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Возвращает общую информацию о файле. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Возвращает общую информацию о файле. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Возвращает общую информацию о файле. |

### Смотрите также

* пространство имен [GroupDocs.Parser](../../groupdocs.parser)
* сборка [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
