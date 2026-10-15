---
title: "GetBarcodes"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Извлекает штрихкоды из документа."
type: docs
weight: 70
url: /ru/net/groupdocs.parser/parser/getbarcodes/
---

## GetBarcodes() {#getbarcodes}

Извлекает штрихкоды из документа.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Возвращаемое значение

Коллекция объектов [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null`, если извлечение штрихкодов не поддерживается.

### Примеры

В следующем примере показано, как извлечь штрихкоды из документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь штрихкоды из документа.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Перебрать штрихкоды
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Вывести индекс страницы
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Вывести значение штрихкода
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### См. также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_3}

Извлекает штрихкоды со страницы документа.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |

### Возвращаемое значение

Коллекция объектов [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null`, если извлечение штрихкодов не поддерживается.

### Примеры

В следующем примере показано, как извлечь штрихкоды со страницы документа:

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Извлечь штрихкоды со второй страницы документа.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Перебрать штрихкоды
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Вывести индекс страницы
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Вывести значение штрихкода
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### См. также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(BarcodeOptions) {#getbarcodes_1}

Извлекает штрихкоды из документа с использованием параметров настройки.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(BarcodeOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | BarcodeOptions | Параметры извлечения штрихкодов. |

### Возвращаемое значение

Коллекция объектов [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null`, если извлечение штрихкодов не поддерживается.

### Примеры

В следующем примере показано, как извлечь штрихкоды из верхнего правого угла.

```csharp
// Создайте экземпляр класса Parser
using (Parser parser = new Parser(filePath))
{
    // Создать параметры, используемые для извлечения штрихкодов
    BarcodeOptions options = new BarcodeOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Извлечь штрихкоды из верхнего правого угла.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Перебрать штрихкоды
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Вывести индекс страницы
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Вывести значение штрихкода
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### См. также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, BarcodeOptions) {#getbarcodes_4}

Извлекает штрихкоды со страницы документа с использованием параметров настройки.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, BarcodeOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | Нулевой индекс страницы. |
| options | BarcodeOptions | Параметры извлечения штрихкодов. |

### Возвращаемое значение

Коллекция объектов [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null`, если извлечение штрихкодов не поддерживается.

### См. также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
