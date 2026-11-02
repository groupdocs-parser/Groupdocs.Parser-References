---
title: export_as_xml method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Exports the collection of metadata to the stream in XML format."
type: docs
url: /python-net/groupdocs.parser.export/extensions/export_as_xml/
is_root: false
weight: 1020
---


## export_as_xml {#metadata-stream}

Exports the collection of metadata to the stream in XML format.

```python
def export_as_xml(cls, metadata, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| metadata | `Iterable[MetadataItem]` | The collection of metadata. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_xml {#metadata-file_name}

Exports the collection of metadata to the file in XML format.

```python
def export_as_xml(cls, metadata, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| metadata | `Iterable[MetadataItem]` | The collection of metadata. |
| file_name | `str` | The full path to the output file. |

## export_as_xml {#document_info-stream}

Exports the document information to the stream in XML format.

```python
def export_as_xml(cls, document_info, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `IDocumentInfo` | The document information. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_xml {#document_info-file_name}

Exports the document information to the file in XML format.

```python
def export_as_xml(cls, document_info, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `IDocumentInfo` | The document information. |
| file_name | `str` | The full path to the output file. |

## export_as_xml {#text_areas-stream}

Exports the collection of text areas to the stream in XML format.

```python
def export_as_xml(cls, text_areas, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text_areas | `Iterable[PageTextArea]` | The collection of the text areas. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_xml {#text_areas-file_name}

Exports the collection of text areas to the file in XML format.

```python
def export_as_xml(cls, text_areas, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text_areas | `Iterable[PageTextArea]` | The collection of text areas. |
| file_name | `str` | The full path to the output file. |

## export_as_xml {#tables-stream}

Exports the collection of tables to the stream in XML format.

```python
def export_as_xml(cls, tables, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| tables | `Iterable[PageTableArea]` | The collection of tables. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_xml {#tables-file_name}

Exports the collection of tables to the file in XML format.

```python
def export_as_xml(cls, tables, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| tables | `Iterable[PageTableArea]` | The collection of tables. |
| file_name | `str` | The full path to the output file. |

## export_as_xml {#barcodes-stream}

Exports the collection of barcodes to the stream in XML format.

```python
def export_as_xml(cls, barcodes, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| barcodes | `Iterable[PageBarcodeArea]` | The collection of barcodes. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_xml {#barcodes-file_name}

Exports the collection of barcodes to the file in XML format.

```python
def export_as_xml(cls, barcodes, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| barcodes | `Iterable[PageBarcodeArea]` | The collection of barcodes. |
| file_name | `str` | The full path to the output file. |

## export_as_xml {#document_data-stream}

Exports document data to the stream in XML format.

```python
def export_as_xml(cls, document_data, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_data | `DocumentData` | Document data. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_xml {#document_data-file_name}

Exports document data to the file in XML format.

```python
def export_as_xml(cls, document_data, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_data | `DocumentData` | Document data. |
| file_name | `str` | The full path to the output file. |

### Aliases

These names call `export_as_xml` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `export_as_xml_ienumerable` | `export_as_xml_ienumerable(metadata, stream)`<br>`export_as_xml_ienumerable(metadata, file_name)`<br>`export_as_xml_ienumerable(text_areas, stream)`<br>`export_as_xml_ienumerable(text_areas, file_name)`<br>`export_as_xml_ienumerable(tables, stream)`<br>`export_as_xml_ienumerable(tables, file_name)`<br>`export_as_xml_ienumerable(barcodes, stream)`<br>`export_as_xml_ienumerable(barcodes, file_name)` |
| `export_as_xml_stream` | `export_as_xml_stream(metadata, stream)`<br>`export_as_xml_stream(document_info, stream)`<br>`export_as_xml_stream(text_areas, stream)`<br>`export_as_xml_stream(tables, stream)`<br>`export_as_xml_stream(barcodes, stream)`<br>`export_as_xml_stream(document_data, stream)` |
| `export_as_xml_streams` | `export_as_xml_streams(metadata, stream)`<br>`export_as_xml_streams(document_info, stream)`<br>`export_as_xml_streams(text_areas, stream)`<br>`export_as_xml_streams(tables, stream)`<br>`export_as_xml_streams(barcodes, stream)`<br>`export_as_xml_streams(document_data, stream)` |
| `export_as_xml_file` | `export_as_xml_file(metadata, file_name)`<br>`export_as_xml_file(document_info, file_name)`<br>`export_as_xml_file(text_areas, file_name)`<br>`export_as_xml_file(tables, file_name)`<br>`export_as_xml_file(barcodes, file_name)`<br>`export_as_xml_file(document_data, file_name)` |
| `export_as_xml_string` | `export_as_xml_string(metadata, file_name)`<br>`export_as_xml_string(document_info, file_name)`<br>`export_as_xml_string(text_areas, file_name)`<br>`export_as_xml_string(tables, file_name)`<br>`export_as_xml_string(barcodes, file_name)`<br>`export_as_xml_string(document_data, file_name)` |
| `export_as_xml_idocument_info` | `export_as_xml_idocument_info(document_info, stream)`<br>`export_as_xml_idocument_info(document_info, file_name)` |
| `export_as_xml_document_data` | `export_as_xml_document_data(document_data, stream)`<br>`export_as_xml_document_data(document_data, file_name)` |

### See Also
* class [`Extensions`](/parser/python-net/groupdocs.parser.export/extensions/)
