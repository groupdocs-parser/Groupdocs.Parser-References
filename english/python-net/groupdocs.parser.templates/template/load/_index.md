---
title: load method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Loads a template from a file."
type: docs
url: /python-net/groupdocs.parser.templates/template/load/
is_root: false
weight: 1040
---


## load {#file_path}

Loads a template from a file.

```python
def load(cls, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |

**Returns:** Template: An instance of `Template` class with loaded template.

| Raises | Description |
| :- | :- |
| `GroupDocsParserException` | The file does not represent the template in a valid format. |

## load {#stream}

Loads a template from a stream.

```python
def load(cls, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| stream | `io.RawIOBase` | The input stream. |

**Returns:** Template: An instance of `Template` class with loaded template.

| Raises | Description |
| :- | :- |
| `GroupDocsParserException` | The stream does not represent the template in a valid format. |

### See Also
* class [`Template`](/parser/python-net/groupdocs.parser.templates/template/)
