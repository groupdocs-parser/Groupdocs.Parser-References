---
title: export_as_json method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Exports the collection of metadata to the stream in JSON format."
type: docs
url: /python-net/groupdocs.parser.export/extensions/export_as_json/
is_root: false
weight: 1010
---


## export_as_json {#metadata-stream}

Exports the collection of metadata to the stream in JSON format.

```python
def export_as_json(cls, metadata, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| metadata | `Iterable[MetadataItem]` | The collection of metadata. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_json {#metadata-file_name}

Exports the collection of metadata to the file in JSON format.

```python
def export_as_json(cls, metadata, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| metadata | `Iterable[MetadataItem]` | The collection of metadata. |
| file_name | `str` | The full path to the output file. |

## export_as_json {#document_info-stream}

Exports the document information to the given stream in JSON format.

```python
def export_as_json(cls, document_info, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `IDocumentInfo` | The document information. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_json {#document_info-file_name}

Exports the document information to a file in JSON format.

```python
def export_as_json(cls, document_info, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `IDocumentInfo` | The document information. |
| file_name | `str` | The full path to the output file. |

## export_as_json {#text_areas-stream}

Exports the collection of text areas to the stream in JSON format.

```python
def export_as_json(cls, text_areas, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text_areas | `Iterable[PageTextArea]` | The collection of the text areas. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_json {#text_areas-file_name}

Exports the collection of text areas to the file in JSON format.

```python
def export_as_json(cls, text_areas, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text_areas | `Iterable[PageTextArea]` | The collection of text areas. |
| file_name | `str` | The full path to the output file. |

## export_as_json {#tables-stream}

Exports the collection of tables to the stream in JSON format.

```python
def export_as_json(cls, tables, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| tables | `Iterable[PageTableArea]` | The collecton of tables. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_json {#tables-file_name}

Exports the collection of tables to the file in JSON format.

```python
def export_as_json(cls, tables, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| tables | `Iterable[PageTableArea]` | The collection of tables. |
| file_name | `str` | The full path to the output file. |

## export_as_json {#barcodes-stream}

Exports the collection of barcodes to the stream in JSON format.

```python
def export_as_json(cls, barcodes, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| barcodes | `Iterable[PageBarcodeArea]` | The collection of barcodes. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_json {#barcodes-file_name}

Exports the collection of barcodes to the file in JSON format.

```python
def export_as_json(cls, barcodes, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| barcodes | `Iterable[PageBarcodeArea]` | The collection of barcodes. |
| file_name | `str` | The full path to the output file. |

## export_as_json {#document_data-stream}

Exports document data to the stream in JSON format.

```python
def export_as_json(cls, document_data, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_data | `DocumentData` | Document data. |
| stream | `io.RawIOBase` | The output stream. |

## export_as_json {#document_data-file_name}

Exports document data to the file in JSON format.

```python
def export_as_json(cls, document_data, file_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_data | `DocumentData` | Document data. |
| file_name | `str` | The full path to the output file. |

### Aliases

These names call `export_as_json` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `export_as_json_ienumerable` | `export_as_json_ienumerable(metadata, stream)`<br>`export_as_json_ienumerable(metadata, file_name)`<br>`export_as_json_ienumerable(text_areas, stream)`<br>`export_as_json_ienumerable(text_areas, file_name)`<br>`export_as_json_ienumerable(tables, stream)`<br>`export_as_json_ienumerable(tables, file_name)`<br>`export_as_json_ienumerable(barcodes, stream)`<br>`export_as_json_ienumerable(barcodes, file_name)` |
| `export_as_json_stream` | `export_as_json_stream(metadata, stream)`<br>`export_as_json_stream(document_info, stream)`<br>`export_as_json_stream(text_areas, stream)`<br>`export_as_json_stream(tables, stream)`<br>`export_as_json_stream(barcodes, stream)`<br>`export_as_json_stream(document_data, stream)` |
| `export_as_json_streams` | `export_as_json_streams(metadata, stream)`<br>`export_as_json_streams(document_info, stream)`<br>`export_as_json_streams(text_areas, stream)`<br>`export_as_json_streams(tables, stream)`<br>`export_as_json_streams(barcodes, stream)`<br>`export_as_json_streams(document_data, stream)` |
| `export_as_json_file` | `export_as_json_file(metadata, file_name)`<br>`export_as_json_file(document_info, file_name)`<br>`export_as_json_file(text_areas, file_name)`<br>`export_as_json_file(tables, file_name)`<br>`export_as_json_file(barcodes, file_name)`<br>`export_as_json_file(document_data, file_name)` |
| `export_as_json_string` | `export_as_json_string(metadata, file_name)`<br>`export_as_json_string(document_info, file_name)`<br>`export_as_json_string(text_areas, file_name)`<br>`export_as_json_string(tables, file_name)`<br>`export_as_json_string(barcodes, file_name)`<br>`export_as_json_string(document_data, file_name)` |
| `export_as_json_idocument_info` | `export_as_json_idocument_info(document_info, stream)`<br>`export_as_json_idocument_info(document_info, file_name)` |
| `export_as_json_document_data` | `export_as_json_document_data(document_data, stream)`<br>`export_as_json_document_data(document_data, file_name)` |

### See Also
* class [`Extensions`](/parser/python-net/groupdocs.parser.export/extensions/)
