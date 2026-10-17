---
title: export method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Exports the collection of metadata to the provided output stream."
type: docs
url: /python-net/groupdocs.parser.export/jsonexporter/export/
is_root: false
weight: 1010
---


## export {#metadata-stream}

Exports the collection of metadata to the provided output stream.

```python
def export(self, metadata, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| metadata | `Iterable[MetadataItem]` | The collection of metadata. |
| stream | `io.RawIOBase` | The output stream. |

## export {#document_info-stream}

Exports the document information to the given stream.

```python
def export(self, document_info, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `IDocumentInfo` | The document information. |
| stream | `io.RawIOBase` | The output stream. |

**Returns:** None.

### Example

```python
import io
from groupdocs.parser import Parser
from groupdocs.parser.export import JsonExporter

parser = Parser("sample.docx")
doc_info = parser.get_document_info()
output = io.BytesIO()

JsonExporter().export(doc_info, output)

json_data = output.getvalue().decode()
print(json_data)
```

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

## export {#tables-stream}

Exports the collection of tables to the provided stream.

```python
def export(self, tables, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| tables | `Iterable[PageTableArea]` | The collection of tables. |
| stream | `io.RawIOBase` | The output stream. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.export import JsonExporter

parser = Parser("sample.docx")
# Assume `get_tables` returns an iterable of Table objects
tables = parser.get_tables()

with open("tables.json", "wb") as out_stream:
    JsonExporter().export(tables, out_stream)
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

**Returns:** None.

### See Also
* class [`JsonExporter`](/parser/python-net/groupdocs.parser.export/jsonexporter/)
