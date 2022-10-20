---
title: GetBarcodes
second_title: Справочник по API GroupDocs.Parser для .NET
description: Извлекает штрихкоды из документа.
type: docs
weight: 50
url: /ru/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Извлекает штрих-коды из документа.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Возвращаемое значение

Коллекция[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) объекты; `нулевой` если извлечение штрих-кодов не поддерживается.

### Примеры

В следующем примере показано, как извлечь штрих-коды из документа:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь штрих-коды из документа.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Перебираем штрих-коды
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Печатаем индекс страницы
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Печать значения штрих-кода
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Смотрите также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Извлекает штрих-коды со страницы документа.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |

### Возвращаемое значение

Коллекция[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) объекты; `нулевой` если извлечение штрих-кодов не поддерживается.

### Примеры

В следующем примере показано, как извлечь штрих-коды со страницы документа:

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечение штрих-кодов со второй страницы документа.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Перебираем штрих-коды
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Печатаем индекс страницы
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Печать значения штрих-кода
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Смотрите также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Извлекает штрих-коды из документа с помощью параметров настройки (для установки прямоугольной области, содержащей штрих-коды).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | PageAreaOptions | Варианты извлечения штрих-кодов. |

### Возвращаемое значение

Коллекция[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) объекты; `нулевой` если извлечение штрих-кодов не поддерживается.

### Примеры

В следующем примере показано, как извлечь штрих-коды из правого верхнего угла.

```csharp
// Создаем экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Создаем опции, которые используются для извлечения штрих-кодов
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Извлечение штрих-кодов из правого верхнего угла.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Перебираем штрих-коды
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Печатаем индекс страницы
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Печать значения штрих-кода
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Смотрите также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Извлекает штрих-коды со страницы документа с помощью параметров настройки (для установки прямоугольной области, содержащей штрих-коды).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Индекс страницы с отсчетом от нуля. |
| options | PageAreaOptions | Варианты извлечения штрих-кодов. |

### Возвращаемое значение

Коллекция[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) объекты; `нулевой` если извлечение штрих-кодов не поддерживается.

### Смотрите также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* пространство имен [GroupDocs.Parser](../../parser)
* сборка [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
