---
title: export_as_xml method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Exports the collection of metadata to the stream in XML format."
type: docs
url: /python-net/groupdocs.parser.export/extensions/export_as_xml/
is_root: false
weight: 1090
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

### See Also
* class [`Extensions`](/parser/python-net/groupdocs.parser.export/extensions/)
