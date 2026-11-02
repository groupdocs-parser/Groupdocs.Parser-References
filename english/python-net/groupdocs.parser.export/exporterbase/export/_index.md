---
title: export method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Exports the collection of metadata to the stream."
type: docs
url: /python-net/groupdocs.parser.export/exporterbase/export/
is_root: false
weight: 1010
---


## export {#metadata-stream}

Exports the collection of metadata to the stream.

```python
def export(self, metadata, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| metadata | `Iterable[MetadataItem]` | The collection of metadata. |
| stream | `io.RawIOBase` | The output stream. |

## export {#metadata-file_name}

Exports the collection of metadata to the file.

```python
def export(self, metadata, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| metadata | `Iterable[MetadataItem]` | The collection of metadata. |
| file_name | `str` | The full path to the output file. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.export import JsonExporter

parser = Parser(file_path)
metadata = parser.get_metadata()
JsonExporter().export(metadata, "metadata.json")
```

## export {#document_info-stream}

Exports the document information to the provided stream.

```python
def export(self, document_info, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `IDocumentInfo` | The document information. |
| stream | `io.RawIOBase` | The output stream. |

## export {#document_info-file_name}

Exports the document information to the specified file.

```python
def export(self, document_info, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `IDocumentInfo` | The document information. |
| file_name | `str` | The full path to the output file. |

## export {#text_areas-stream}

Exports the collection of text areas to the stream.

```python
def export(self, text_areas, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text_areas | `Iterable[PageTextArea]` | The collection of the text areas. |
| stream | `io.RawIOBase` | The output stream. |

## export {#text_areas-file_name}

Exports the collection of text areas to the file.

```python
def export(self, text_areas, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text_areas | `Iterable[PageTextArea]` | The collection of text areas. |
| file_name | `str` | The full path to the output file. |

## export {#tables-stream}

Exports the collection of tables to the stream.

```python
def export(self, tables, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| tables | `Iterable[PageTableArea]` | The collection of tables. |
| stream | `io.RawIOBase` | The output stream. |

## export {#tables-file_name}

Exports the collection of tables to the specified file.

```python
def export(self, tables, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| tables | `Iterable[PageTableArea]` | The collection of tables. |
| file_name | `str` | The full path to the output file. |

### Example

```python
from groupdocs.parser.export import JsonExporter

def export_tables(tables, output_path):
    exporter = JsonExporter()
    exporter.export(tables, output_path)
```

## export {#barcodes-stream}

Exports the collection of barcodes to the stream.

```python
def export(self, barcodes, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| barcodes | `Iterable[PageBarcodeArea]` | The collection of barcodes. |
| stream | `io.RawIOBase` | The output stream. |

## export {#barcodes-file_name}

Exports the collection of barcodes to the file.

```python
def export(self, barcodes, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| barcodes | `Iterable[PageBarcodeArea]` | The collection of barcodes. |
| file_name | `str` | The full path to the output file. |

## export {#document_data-stream}

Exports document data to the provided stream.

```python
def export(self, document_data, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_data | `DocumentData` | Document data. |
| stream | `io.RawIOBase` | The output stream. |

## export {#document_data-file_name}

Exports document data to the file.

```python
def export(self, document_data, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_data | `DocumentData` | Document data. |
| file_name | `str` | The full path to the output file. |

### Aliases

These names call `export` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `export_ienumerable` | `export_ienumerable(metadata, stream)`<br>`export_ienumerable(metadata, file_name)`<br>`export_ienumerable(text_areas, stream)`<br>`export_ienumerable(text_areas, file_name)`<br>`export_ienumerable(tables, stream)`<br>`export_ienumerable(tables, file_name)`<br>`export_ienumerable(barcodes, stream)`<br>`export_ienumerable(barcodes, file_name)` |
| `export_stream` | `export_stream(metadata, stream)`<br>`export_stream(document_info, stream)`<br>`export_stream(text_areas, stream)`<br>`export_stream(tables, stream)`<br>`export_stream(barcodes, stream)`<br>`export_stream(document_data, stream)` |
| `export_streams` | `export_streams(metadata, stream)`<br>`export_streams(document_info, stream)`<br>`export_streams(text_areas, stream)`<br>`export_streams(tables, stream)`<br>`export_streams(barcodes, stream)`<br>`export_streams(document_data, stream)` |
| `export_file` | `export_file(metadata, file_name)`<br>`export_file(document_info, file_name)`<br>`export_file(text_areas, file_name)`<br>`export_file(tables, file_name)`<br>`export_file(barcodes, file_name)`<br>`export_file(document_data, file_name)` |
| `export_string` | `export_string(metadata, file_name)`<br>`export_string(document_info, file_name)`<br>`export_string(text_areas, file_name)`<br>`export_string(tables, file_name)`<br>`export_string(barcodes, file_name)`<br>`export_string(document_data, file_name)` |
| `export_idocument_info` | `export_idocument_info(document_info, stream)`<br>`export_idocument_info(document_info, file_name)` |
| `export_document_data` | `export_document_data(document_data, stream)`<br>`export_document_data(document_data, file_name)` |

### See Also
* class [`ExporterBase`](/parser/python-net/groupdocs.parser.export/exporterbase/)
