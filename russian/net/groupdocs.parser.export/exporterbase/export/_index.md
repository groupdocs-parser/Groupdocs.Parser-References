---
title: "Экспорт"
second_title: "GroupDocs.Parser для .NET справочник API"
description: "Экспортирует коллекцию метаданных в поток."
type: docs
weight: 10
url: /ru/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Экспортирует коллекцию метаданных в поток.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| метаданные | IEnumerable`1 | Коллекция метаданных. |
| поток | Stream | Выходной поток. |

### См. также

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

Экспортирует коллекцию метаданных в файл.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| метаданные | IEnumerable`1 | Коллекция метаданных. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Экспортирует информацию о документе в поток.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Информация о документе. |
| поток | Stream | Выходной поток. |

### См. также

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

Экспортирует информацию о документе в файл.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Информация о документе. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Экспортирует коллекцию текстовых областей в поток.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Коллекция текстовых областей. |
| поток | Stream | Выходной поток. |

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

Экспортирует коллекцию текстовых областей в файл.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Коллекция текстовых областей. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Экспортирует коллекцию таблиц в поток.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| таблицы | IEnumerable`1 | Коллекция таблиц. |
| поток | Stream | Выходной поток. |

### См. также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

Экспортирует коллекцию таблиц в файл.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| таблицы | IEnumerable`1 | Коллекция таблиц. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Экспортирует коллекцию штрихкодов в поток.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| штрихкоды | IEnumerable`1 | Коллекция штрих‑кодов. |
| поток | Stream | Выходной поток. |

### См. также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

Экспортирует коллекцию штрихкодов в файл.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| штрихкоды | IEnumerable`1 | Коллекция штрих‑кодов. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Экспортирует данные документа в поток.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentData | DocumentData | Данные документа. |
| поток | Stream | Выходной поток. |

### См. также

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

Экспортирует данные документа в файл.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documentData | DocumentData | Данные документа. |
| fileName | Строка | Полный путь к выходному файлу. |

### См. также

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для GroupDocs.Parser.dll -->
