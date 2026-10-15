---
title: "ExportAsJson"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Экспортирует коллекцию метаданных в поток в формате JSON."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.export/extensions/exportasjson/
---

## ExportAsJson(this IEnumerable&lt;MetadataItem&gt;, Stream) {#exportasjson_4}

Экспортирует коллекцию метаданных в поток в формате JSON.

```csharp
public static void ExportAsJson(this IEnumerable<MetadataItem> metadata, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| метаданные | IEnumerable`1 | Коллекция метаданных. |
| поток | Stream | Выходной поток. |

### См. также

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this IEnumerable&lt;MetadataItem&gt;, string) {#exportasjson_5}

Экспортирует коллекцию метаданных в файл в формате JSON.

```csharp
public static void ExportAsJson(this IEnumerable<MetadataItem> metadata, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| метаданные | IEnumerable`1 | Коллекция метаданных. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this IDocumentInfo, Stream) {#exportasjson_2}

Экспортирует информацию о документе в поток в формате JSON.

```csharp
public static void ExportAsJson(this IDocumentInfo documentInfo, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Информация о документе. |
| поток | Stream | Выходной поток. |

### См. также

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this IDocumentInfo, string) {#exportasjson_3}

Экспортирует информацию о документе в файл в формате JSON.

```csharp
public static void ExportAsJson(this IDocumentInfo documentInfo, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Информация о документе. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this IEnumerable&lt;PageTextArea&gt;, Stream) {#exportasjson_10}

Экспортирует коллекцию текстовых областей в поток в формате JSON.

```csharp
public static void ExportAsJson(this IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Коллекция текстовых областей. |
| поток | Stream | Выходной поток. |

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this IEnumerable&lt;PageTextArea&gt;, string) {#exportasjson_11}

Экспортирует collectiob текстовых областей в файл в формате JSON.

```csharp
public static void ExportAsJson(this IEnumerable<PageTextArea> textAreas, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Коллекция текстовых областей. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this IEnumerable&lt;PageTableArea&gt;, Stream) {#exportasjson_8}

Экспортирует коллекцию таблиц в поток в формате JSON.

```csharp
public static void ExportAsJson(this IEnumerable<PageTableArea> tables, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| таблицы | IEnumerable`1 | Коллекция таблиц. |
| поток | Stream | Выходной поток. |

### См. также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this IEnumerable&lt;PageTableArea&gt;, string) {#exportasjson_9}

Экспортирует коллекцию таблиц в файл в формате JSON.

```csharp
public static void ExportAsJson(this IEnumerable<PageTableArea> tables, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| таблицы | IEnumerable`1 | Коллекция таблиц. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#exportasjson_6}

Экспортирует коллекцию штрихкодов в поток в формате JSON.

```csharp
public static void ExportAsJson(this IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| штрихкоды | IEnumerable`1 | Коллекция штрих‑кодов. |
| поток | Stream | Выходной поток. |

### См. также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this IEnumerable&lt;PageBarcodeArea&gt;, string) {#exportasjson_7}

Экспортирует коллекцию штрихкодов в файл в формате JSON.

```csharp
public static void ExportAsJson(this IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| штрихкоды | IEnumerable`1 | Коллекция штрих‑кодов. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this DocumentData, Stream) {#exportasjson}

Экспортирует данные документа в поток в формате JSON.

```csharp
public static void ExportAsJson(this DocumentData documentData, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentData | DocumentData | Данные документа. |
| поток | Stream | Выходной поток. |

### См. также

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsJson(this DocumentData, string) {#exportasjson_1}

Экспортирует данные документа в файл в формате JSON.

```csharp
public static void ExportAsJson(this DocumentData documentData, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentData | DocumentData | Данные документа. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
