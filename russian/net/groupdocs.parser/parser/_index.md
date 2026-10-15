---
title: "Parser"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Представляет основной класс, который управляет извлечением контейнера изображений текста и функциями парсинга."
type: docs
weight: 30
url: /ru/net/groupdocs.parser/parser/
---

## Parser class

Представляет основной класс, который управляет обработкой текста, изображений, извлечением контейнеров и функциями парсинга.

```csharp
public sealed class Parser : IDisposable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Инициализирует новый экземпляр класса [`Parser`](../parser) для извлечения данных из базы данных. |
| [Parser](parser#constructor)(EmailConnection) | Инициализирует новый экземпляр класса [`Parser`](../parser) для извлечения данных из удалённого почтового сервера. |
| [Parser](parser#constructor_4)(Stream) | Инициализирует новый экземпляр класса [`Parser`](../parser). |
| [Parser](parser#constructor_8)(string) | Инициализирует новый экземпляр класса [`Parser`](../parser). |
| [Parser](parser#constructor_12)(Uri) | Инициализирует новый экземпляр класса [`Parser`](../parser) для извлечения данных из URI. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Инициализирует новый экземпляр класса [`Parser`](../parser) для извлечения данных из базы данных. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Инициализирует новый экземпляр класса [`Parser`](../parser) для извлечения данных из удалённого почтового сервера. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Инициализирует новый экземпляр класса [`Parser`](../parser) с [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Инициализирует новый экземпляр класса [`Parser`](../parser) с [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | Инициализирует новый экземпляр класса [`Parser`](../parser) с [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | Инициализирует новый экземпляр класса [`Parser`](../parser) с [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | Инициализирует новый экземпляр класса [`Parser`](../parser) для извлечения данных из URI с *loadOptions*. |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | Инициализирует новый экземпляр класса [`Parser`](../parser) для извлечения данных из URI с *parserSettings*. |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Инициализирует новый экземпляр класса [`Parser`](../parser) с [`LoadOptions`](../../groupdocs.parser.options/loadoptions) и [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Инициализирует новый экземпляр класса [`Parser`](../parser) с [`LoadOptions`](../../groupdocs.parser.options/loadoptions) и [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | Инициализирует новый экземпляр класса [`Parser`](../parser) для извлечения данных из URI с *loadOptions* и *parserSettings*. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Получает поддерживаемые функции. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Выполняет задачи, определённые приложением, связанные со освобождением, выпуском или сбросом неуправляемых ресурсов. |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | Генерирует поля для автоматической настройки позиции и масштаба шаблона. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Получить предварительный просмотр страниц. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | Извлекает аннотации из документа. Обратите внимание, что в настоящее время поддерживается только формат PDF. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | Извлекает аннотации со страницы документа. Обратите внимание, что в настоящее время поддерживается только формат PDF. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Извлекает штрихкоды из документа. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | Извлекает штрихкоды из документа с использованием параметров настройки. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | Извлекает штрихкоды со страницы документа. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | Извлекает штрихкоды со страницы документа с использованием параметров настройки. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Извлекает объект‑контейнер из документа для работы с форматами, содержащими вложения, ZIP‑архивы и т.п. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Возвращает общую информацию о документе. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Извлекает форматированный текст из документа. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Извлекает форматированный текст со страницы документа. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Извлекает выделение из документа. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Извлекает гиперссылки из документа. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Извлекает гиперссылки со страницы документа. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Извлекает гиперссылки из документа с использованием параметров настройки (для задания прямоугольной области, содержащей гиперссылки). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Извлекает гиперссылки со страницы документа с использованием параметров настройки (для задания прямоугольной области, содержащей гиперссылки). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Извлекает изображения из документа. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Извлекает изображения со страницы документа. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Извлекает изображения из документа с использованием параметров настройки (для задания прямоугольной области, содержащей изображения). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Извлекает изображения со страницы документа с использованием параметров настройки (для задания прямоугольной области, содержащей изображения). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Извлекает метаданные из документа. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | Создаёт предварительный просмотр страницы документа. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | Создаёт предварительный просмотр страницы документа с использованием параметров настройки. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Извлекает структурированный текст из документа. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | Извлекает таблицы из документа. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | Извлекает таблицы со страницы документа. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | Извлекает таблицы из документа. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | Извлекает таблицы со страницы документа. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Извлекает текст из документа. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Извлекает текст со страницы документа. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Извлекает страницу текста из документа, используя параметры текста (для включения режима быстрого необработанного извлечения текста). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Извлекает текст со страницы документа, используя параметры текста (для включения режима быстрого необработанного извлечения текста). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Извлекает области текста из документа. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Извлекает области текста со страницы документа. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Извлекает области текста из документа, используя параметры настройки (регулярные выражения, учет регистра и т.д.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Извлекает области текста со страницы документа, используя параметры настройки (регулярные выражения, учет регистра и т.д.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Извлекает оглавление из документа. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | Извлекает ячейки листа. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | Извлекает ячейки листа, используя параметры настройки. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | Извлекает информацию обо всех листах в электронной таблице. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | Извлекает информацию о листе. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | Разбирает документ с помощью пользовательского шаблона. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | Разбирает документ с помощью пользовательского шаблона, используя параметры настройки. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | Выбирает наиболее подходящий шаблон из предоставленной коллекции, а затем разбирает документ согласно выбранному шаблону. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Разбирает форму документа. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Ищет *keyword* в документе. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Ищет *keyword* в документе, используя параметры поиска (регулярные выражения, учет регистра и т.д.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Возвращает общую информацию о файле. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Возвращает общую информацию о файле. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Возвращает общую информацию о файле. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Возвращает общую информацию о файле. |

### См. также

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
