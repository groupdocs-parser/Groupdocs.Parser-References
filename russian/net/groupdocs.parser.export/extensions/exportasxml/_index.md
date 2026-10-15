---
title: "ExportAsXml"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Экспортирует коллекцию метаданных в поток в формате XML."
type: docs
weight: 20
url: /ru/net/groupdocs.parser.export/extensions/exportasxml/
---

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, Stream) {#exportasxml_4}

Экспортирует коллекцию метаданных в поток в формате XML.

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, Stream stream)
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

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, string) {#exportasxml_5}

Экспортирует коллекцию метаданных в файл в формате XML.

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, string fileName)
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

## ExportAsXml(this IDocumentInfo, Stream) {#exportasxml_2}

Экспортирует информацию о документе в поток в формате XML.

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, Stream stream)
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

## ExportAsXml(this IDocumentInfo, string) {#exportasxml_3}

Экспортирует информацию о документе в файл в формате XML.

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, string fileName)
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

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, Stream) {#exportasxml_10}

Экспортирует коллекцию текстовых областей в поток в формате XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, Stream stream)
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

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, string) {#exportasxml_11}

Экспортирует collectiob текстовых областей в файл в формате XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, string fileName)
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

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, Stream) {#exportasxml_8}

Экспортирует коллекцию таблиц в поток в формате XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, Stream stream)
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

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, string) {#exportasxml_9}

Экспортирует коллекцию таблиц в файл в формате XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, string fileName)
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

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#exportasxml_6}

Экспортирует коллекцию штрихкодов в поток в формате XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, Stream stream)
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

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, string) {#exportasxml_7}

Экспортирует коллекцию штрихкодов в файл в формате XML.

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, string fileName)
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

## ExportAsXml(this DocumentData, Stream) {#exportasxml}

Экспортирует данные документа в поток в формате XML.

```csharp
public static void ExportAsXml(this DocumentData documentData, Stream stream)
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

## ExportAsXml(this DocumentData, string) {#exportasxml_1}

Экспортирует данные документа в файл в формате XML.

```csharp
public static void ExportAsXml(this DocumentData documentData, string fileName)
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
