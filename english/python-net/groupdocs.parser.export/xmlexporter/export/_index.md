---
title: export method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Exports the collection of metadata to the stream."
type: docs
url: /python-net/groupdocs.parser.export/xmlexporter/export/
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

## export {#document_info-stream}

Exports the document information to the stream.

```python
def export(self, document_info, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `IDocumentInfo` | The document information. |
| stream | `io.RawIOBase` | The output stream. |

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

Exports the collection of tables to the stream.

```python
def export(self, tables, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| tables | `Iterable[PageTableArea]` | The collection of tables. |
| stream | `io.RawIOBase` | The output stream. |

## export {#barcodes-stream}

Exports the collection of barcodes to the provided output stream.

```python
def export(self, barcodes, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| barcodes | `Iterable[PageBarcodeArea]` | Iterable of barcode objects to export. |
| stream | `io.RawIOBase` | An io.RawIOBase stream to write the exported data. |

## export {#document_data-stream}

Exports document data to the stream.

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
* class [`XmlExporter`](/parser/python-net/groupdocs.parser.export/xmlexporter/)
