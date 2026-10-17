---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new LoadOptions instance with an empty password, unknown file format, and default encodings."
type: docs
url: /python-net/groupdocs.parser.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new LoadOptions instance with an empty password, unknown file format, and default encodings.

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

options = LoadOptions("123456")  # password for protected document
with Parser("protected.pdf", options) as parser:
    reader = parser.get_text()
    text = reader.read_to_end() if reader is not None else None
    print(text if text is not None else "Text extraction isn't supported.")
```

## __init__ {#timeout}

Initializes a new LoadOptions instance with a timeout.

```python
def __init__(self, timeout):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| timeout | `timedelta` | The timedelta that represents the number of milliseconds to wait. |

## __init__ {#password}

Initializes a new LoadOptions instance with the file format set to `FileFormat.Unknown` and default encodings.

```python
def __init__(self, password):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| password | `str` | The password to open the password-protected file. |

### Example

```python
    from groupdocs.parser import Parser
    from groupdocs.parser.options import LoadOptions

    options = LoadOptions("123456")
    with Parser("protected.pdf", options) as parser:
        reader = parser.get_text()
        text = reader.read_to_end() if reader is not None else None
        print(text if text is not None else "Text extraction isn't supported.")
    ```

## __init__ {#file_format}

Initializes a new LoadOptions instance with an empty password and default encodings.

```python
def __init__(self, file_format):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_format | `FileFormat` | The format of the file. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

options = LoadOptions("123456")

with Parser("protected.pdf", options) as parser:
    reader = parser.get_text()
    text = reader.read_to_end() if reader is not None else None
    print(text if text is not None else "Text extraction isn't supported.")
```

## __init__ {#file_format-password}

Initializes a new LoadOptions instance with the specified password and default encodings.

```python
def __init__(self, file_format, password):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_format | `FileFormat` | The format of the file. |
| password | `str` | The password to open the password-protected file. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

options = LoadOptions(password="123456")

with Parser("protected.pdf", options) as parser:
    reader = parser.get_text()
    text = reader.read_to_end() if reader is not None else None
    print(text if text is not None else "Text extraction isn't supported.")
```

## __init__ {#file_format-password-encoding-default_ansi_encoding}

Initializes a new instance of LoadOptions with custom encodings.

```python
def __init__(self, file_format, password, encoding, default_ansi_encoding):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_format | `FileFormat` | The format of the file. |
| password | `str` | The password to open the password‑protected file. |
| encoding | `System.Text.Encoding` | The encoding of the document. |
| default_ansi_encoding | `System.Text.Encoding` | The default ANSI encoding which is used for encoding detection. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

options = LoadOptions("123456")  # password only; other parameters are optional
with Parser("protected.pdf", options) as parser:
    reader = parser.get_text()
    text = reader.read_to_end() if reader is not None else None
    print(text if text is not None else "Text extraction isn't supported.")
```

## __init__ {#file_format-password-encoding-default_ansi_encoding-timeout}

Initializes a new instance of LoadOptions with full customization.

```python
def __init__(self, file_format, password, encoding, default_ansi_encoding, timeout):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_format | `FileFormat` | The format of the file. |
| password | `str` | The password to open the password‑protected file. |
| encoding | `System.Text.Encoding` | The encoding of the document. |
| default_ansi_encoding | `System.Text.Encoding` | The default ANSI encoding which is used for encoding detection. |
| timeout | `timedelta` | The TimeSpan that represents the number of milliseconds to wait. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

options = LoadOptions("123456")  # password for a protected PDF
with Parser("protected.pdf", options) as parser:
    reader = parser.get_text()
    text = reader.read_to_end() if reader is not None else None
    print(text if text is not None else "Text extraction isn't supported.")
```

## __init__ {#file_type}

Initializes a new instance of the LoadOptions class with an empty password and default encodings.

```python
def __init__(self, file_type):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_type | `FileType` | The type of the file. |

### Example

```python
    from groupdocs.parser import Parser
    from groupdocs.parser.options import LoadOptions

    # Load a password‑protected PDF using a password string
    options = LoadOptions("123456")
    with Parser("protected.pdf", options) as parser:
        reader = parser.get_text()
        text = reader.read_to_end() if reader is not None else None
        print(text if text is not None else "Text extraction isn't supported.")
    ```

## __init__ {#file_type-password}

Initializes a new LoadOptions instance with the specified file type and password, using default encodings.

```python
def __init__(self, file_type, password):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_type | `FileType` | The type of the file. |
| password | `str` | The password to open the password‑protected file. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

options = LoadOptions("123456")
with Parser("protected.pdf", options) as parser:
    reader = parser.get_text()
    text = reader.read_to_end() if reader is not None else None
    print(text if text is not None else "Text extraction isn't supported.")
```

## __init__ {#file_type-password-encoding-default_ansi_encoding}

Initializes a new LoadOptions instance with custom encodings.

```python
def __init__(self, file_type, password, encoding, default_ansi_encoding):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_type | `FileType` | The type of the file. |
| password | `str` | The password to open the password-protected file. |
| encoding | `System.Text.Encoding` | The encoding of the document. |
| default_ansi_encoding | `System.Text.Encoding` | The default ANSI encoding which is used for encoding detection. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

options = LoadOptions(password="123456")
with Parser("protected.pdf", options) as parser:
    reader = parser.get_text()
    text = reader.read_to_end() if reader else None
    print(text or "Text extraction isn't supported.")
```

## __init__ {#file_type-password-encoding-default_ansi_encoding-timeout}

Initializes a fully customized LoadOptions instance.

```python
def __init__(self, file_type, password, encoding, default_ansi_encoding, timeout):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_type | `FileType` | The type of the file. |
| password | `str` | The password to open the password‑protected file. |
| encoding | `System.Text.Encoding` | The encoding of the document. |
| default_ansi_encoding | `System.Text.Encoding` | The default ANSI encoding which is used for encoding detection. |
| timeout | `timedelta` | The time span that represents the number of milliseconds to wait. |

### Example

```python
from groupdocs.parser.options import LoadOptions

# Load a password‑protected PDF using its password
options = LoadOptions(password="123456")
```

### See Also
* class [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions/)
