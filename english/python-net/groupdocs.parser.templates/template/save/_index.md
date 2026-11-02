---
title: save method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Saves a template to a file."
type: docs
url: /python-net/groupdocs.parser.templates/template/save/
is_root: false
weight: 1040
---


## save {#file_path}

Saves a template to a file.

```python
def save(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |

## save {#stream}

Saves a template to a stream.

```python
def save(self, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| stream | `io.RawIOBase` | The output stream. |

### Aliases

These names call `save` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `save_file` | `save_file(file_path)` |
| `save_string` | `save_string(file_path)` |
| `save_stream` | `save_stream(stream)` |
| `save_streams` | `save_streams(stream)` |

### See Also
* class [`Template`](/parser/python-net/groupdocs.parser.templates/template/)
