---
title: LoadOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Provides the options which are used to open a file."
type: docs
url: /python-net/groupdocs.parser.options/loadoptions/
is_root: false
weight: 240
---


## LoadOptions class

Provides the options which are used to open a file.

An instance of this class is used as a parameter in [`Parser`](/parser/python-net/groupdocs.parser/parser/) constructors:
- [`Parser`](/parser/python-net/groupdocs.parser/parser/) accepting a stream and [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions/)
- [`Parser`](/parser/python-net/groupdocs.parser/parser/) accepting a file path and [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions/)

See the usage examples there.

Learn more:
- https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats
- https://docs.groupdocs.com/display/parsernet/Password-protected+documents

The LoadOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/) | Initializes a new LoadOptions instance with an empty password, unknown file format, and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#timeout) | Initializes a new LoadOptions instance with a timeout. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#password) | Initializes a new LoadOptions instance with the file format set to `FileFormat.Unknown` and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#file_format) | Initializes a new LoadOptions instance with an empty password and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#file_format-password) | Initializes a new LoadOptions instance with the specified password and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#file_format-password-encoding-default_ansi_encoding) | Initializes a new instance of LoadOptions with custom encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#file_format-password-encoding-default_ansi_encoding-timeout) | Initializes a new instance of LoadOptions with full customization. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#file_type) | Initializes a new instance of the LoadOptions class with an empty password and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#file_type-password) | Initializes a new LoadOptions instance with the specified file type and password, using default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#file_type-password-encoding-default_ansi_encoding) | Initializes a new LoadOptions instance with custom encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#file_type-password-encoding-default_ansi_encoding-timeout) | Initializes a fully customized LoadOptions instance. |

### Properties
| Property | Description |
| :- | :- |
| [default_ansi_encoding](/parser/python-net/groupdocs.parser.options/loadoptions/default_ansi_encoding/) | The default ANSI encoding used for encoding detection. |
| [encoding](/parser/python-net/groupdocs.parser.options/loadoptions/encoding/) | The encoding of the document. |
| [file_format](/parser/python-net/groupdocs.parser.options/loadoptions/file_format/) | The file format as a `FileFormat` enumeration. |
| [file_type](/parser/python-net/groupdocs.parser.options/loadoptions/file_type/) | The file type. |
| [password](/parser/python-net/groupdocs.parser.options/loadoptions/password/) | The password used to open a password‑protected file. This property is a string value representing the password. |
| [timeout](/parser/python-net/groupdocs.parser.options/loadoptions/timeout/) | The timeout as a `timedelta` representing the number of milliseconds to wait. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

options = LoadOptions("123456")  # password for the protected document

with Parser("protected.pdf", options) as parser:
    reader = parser.get_text()
    text = reader.read_to_end() if reader is not None else None
    print(text if text is not None else "Text extraction isn't supported.")
```

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)
