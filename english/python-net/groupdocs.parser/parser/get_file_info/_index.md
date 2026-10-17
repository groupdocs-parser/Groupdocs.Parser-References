---
title: get_file_info method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Returns the general information about a file."
type: docs
url: /python-net/groupdocs.parser/parser/get_file_info/
is_root: false
weight: 1140
---


## get_file_info {#file_path}

Returns the general information about a file.

```python
def get_file_info(cls, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |

**Returns:** FileInfo: An instance containing file information.

### Example

```python
    from groupdocs.parser import Parser

    info = Parser.get_file_info("./sample.pdf")
    print("Password is required" if info.is_encrypted else "")
    ```

## get_file_info {#file_path-load_options}

Returns the general information about a file.

```python
def get_file_info(cls, file_path, load_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |
| load_options | `LoadOptions` | The options to open the file. |

**Returns:** FileInfo: An instance of `FileInfo`.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

# Get file info, providing a password if the document is protected
file_info = Parser.get_file_info("./sample.pdf", LoadOptions("password"))

# Check if the document is encrypted
if file_info.is_encrypted:
    print("Password is required")

# Print the detected file type
print(file_info.file_type)
```

## get_file_info {#document}

Returns the general information about a file.

```python
def get_file_info(cls, document):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | The source input stream. |

**Returns:** FileInfo: General information about the file.

### Example

```python
    from groupdocs.parser import Parser

    # Get file information
    file_info = Parser.get_file_info("./sample.pdf")
    print(f"File type: {file_info.file_type}")

    # Check if the document is password-protected
    if file_info.is_encrypted:
        print("Password is required")
    ```

## get_file_info {#document-load_options}

Returns the general information about a file.

```python
def get_file_info(cls, document, load_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | The source input stream. |
| load_options | `LoadOptions` | The options to open the file. |

**Returns:** FileInfo: An instance containing file information.

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

with open("sample.pdf", "rb") as stream:
    file_info = Parser.get_file_info(stream, LoadOptions())
    print("Password is required" if file_info.is_encrypted else "")
    print(file_info.file_type)
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)
