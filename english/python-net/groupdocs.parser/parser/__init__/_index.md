---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the Parser class to extract data from a URI."
type: docs
url: /python-net/groupdocs.parser/parser/__init__/
is_root: false
weight: 10
---


## __init__ {#uri}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class to extract data from a URI.

```python
def __init__(self, uri):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| uri | `str` | The Uri the request is sent to. |

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

## __init__ {#uri-load_options}

Initializes a new Parser instance to extract data from a URI with the specified load options.

```python
def __init__(self, uri, load_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| uri | `str` | The URI the request is sent to. |
| load_options | `LoadOptions` | The options to open the file. |

### Example

```python
from groupdocs.parser import Parser

with Parser("https://example.com/document.pdf") as parser:
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

## __init__ {#uri-parser_settings}

Initializes a new Parser to extract data from a URI using the specified parser settings.

```python
def __init__(self, uri, parser_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| uri | `str` | The URI the request is sent to. |
| parser_settings | `ParserSettings` | The parser settings used to customize data extraction. |

### Example

```python
import io
import urllib.request

from groupdocs.parser import Parser
from groupdocs.parser.options import ParserSettings

# A str is a file path; to read a document from a URL, download it
# and pass the bytes as a stream.
data = urllib.request.urlopen("https://example.com/document.pdf").read()
settings = ParserSettings(lambda level, message, exception: print(level, message))
with Parser(io.BytesIO(data), settings) as parser:
    text = parser.get_text()
    if text is not None:
        print(text)
```

## __init__ {#uri-load_options-parser_settings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class to extract data from a URI with the specified load options and parser settings.

```python
def __init__(self, uri, load_options, parser_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| uri | `str` | The URI the request is sent to. |
| load_options | `LoadOptions` | The options to open the file. |
| parser_settings | `ParserSettings` | The parser settings used to customize data extraction. |

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

## __init__ {#connection}

Initializes a new Parser instance to extract data from a database.

Learn more:
- https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases

```python
def __init__(self, connection):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| connection | `System.Data.Common.DbConnection` | The database connection. |

## __init__ {#connection-parser_settings}

Initializes a new Parser instance to extract data from a database.

Learn more:
- Extract data from databases: https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases
- Logging: https://docs.groupdocs.com/display/parsernet/Logging

```python
def __init__(self, connection, parser_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| connection | `System.Data.Common.DbConnection` | The database connection. |
| parser_settings | `ParserSettings` | The parser settings which customize data extraction. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import ParserSettings

# `connection` is an open ADO.NET DbConnection. A Python sqlite3
# connection is not one: the engine reads databases through .NET.
settings = ParserSettings(lambda level, message, exception: print(level, message))
with Parser(connection, settings) as parser:
    for table in parser.get_toc() or []:
        print(table.text)  # a table name
```

## __init__ {#connection}

Initializes a new Parser instance to extract data from a remote email server.

Learn more:
- [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

```python
def __init__(self, connection):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| connection | `EmailConnection` | The email connection. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import EmailEwsConnection

# Create the connection object for Exchange Web Services protocol
connection = EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password"
)

with Parser(connection) as parser:
    if not parser.features.container:
        print("Container extraction isn't supported.")
    else:
        emails = parser.get_container()
        for item in emails:
            with item.open_parser() as email_parser:
                with email_parser.get_text() as reader:
                    print(reader.read_to_end() if reader is not None else "Text extraction isn't supported.")
```

## __init__ {#connection-parser_settings}

Initializes a new Parser to extract data from a remote email server.

```python
def __init__(self, connection, parser_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| connection | `EmailConnection` | The email connection. |
| parser_settings | `ParserSettings` | The parser settings which are used to customize data extraction. Learn more: - [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols) - [Logging](https://docs.groupdocs.com/display/parsernet/Logging) |

## __init__ {#file_path}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class.

Learn more:
- [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

```python
def __init__(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

## __init__ {#file_path-load_options}

Initializes a new Parser with the specified file path and load options.

Learn more:
- Loading specific file formats
- Loading password-protected documents
- Load document from local disk

```python
def __init__(self, file_path, load_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |
| load_options | `LoadOptions` | The options to open the file. |

| Raises | Description |
| :- | :- |
| `InvalidPasswordException` | The document password is incorrect or empty. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions

load_options = LoadOptions(password="myPassword")
with Parser("./protected.pdf", load_options) as parser:
    if not parser.features.text:
        print("Text extraction isn't supported.")
    else:
        text_reader = parser.get_text()
        if text_reader:
            print(text_reader.read_to_end())
```

## __init__ {#file_path-parser_settings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class with [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/).

```python
def __init__(self, file_path, parser_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |
| parser_settings | `ParserSettings` | The parser settings which are used to customize data extraction. |

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

## __init__ {#file_path-load_options-parser_settings}

Initializes a new [`Parser`](/parser/python-net/groupdocs.parser/parser/) instance with the specified file path, optional load options, and parser settings.

Learn more:
- Loading specific file formats
- Loading password-protected documents
- Logging
- Load document from local disk

```python
def __init__(self, file_path, load_options, parser_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The path to the file. |
| load_options | `LoadOptions` | The options to open the file. |
| parser_settings | `ParserSettings` | The parser settings which are used to customize data extraction. |

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

## __init__ {#document}

Initializes a new [`Parser`](/parser/python-net/groupdocs.parser/parser/) instance.

Learn more:
- Load document from stream: https://docs.groupdocs.com/display/parsernet/Load+document+from+stream

```python
def __init__(self, document):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | The source input stream. |

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

## __init__ {#document-load_options}

Initializes a new Parser instance with the specified load options.

Learn more:
- Loading specific file formats: https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats
- Loading password-protected documents: https://docs.groupdocs.com/display/parsernet/Password-protected+documents
- Load document from stream: https://docs.groupdocs.com/display/parsernet/Load+document+from+stream

```python
def __init__(self, document, load_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | The source input stream. |
| load_options | `LoadOptions` | The options to open the file. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions, FileFormat
from groupdocs.parser.exceptions import InvalidPasswordException

# Load a markdown document from a stream with explicit file format
with open("doc.md", "rb") as stream:
    with Parser(stream, LoadOptions(FileFormat.Markup)) as parser:
        if parser.features.text:
            with parser.get_text() as reader:
                print(reader.read_to_end())

# Load a password‑protected document
try:
    with Parser("protected.docx", LoadOptions(password="secret")) as parser:
        if parser.features.text:
            with parser.get_text() as reader:
                print(reader.read_to_end())
except InvalidPasswordException:
    print("Invalid password")
```

## __init__ {#document-parser_settings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser/) class with [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/).

```python
def __init__(self, document, parser_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | The source input stream. |
| parser_settings | `ParserSettings` | The parser settings which are used to customize data extraction. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import ParserSettings

with open("./sample.pdf", "rb") as stream:
    settings = ParserSettings(lambda level, message, exception: print(level, message))
    with Parser(stream, settings) as parser:
        text_reader = parser.get_text()
        if text_reader is not None:
            print(text_reader.read_to_end())
```

## __init__ {#document-load_options-parser_settings}

Initializes a new Parser instance with the given document stream, load options, and parser settings.

Learn more:
- https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats
- https://docs.groupdocs.com/display/parsernet/Password-protected+documents
- https://docs.groupdocs.com/display/parsernet/Load+document+from+stream
- https://docs.groupdocs.com/display/parsernet/Logging

```python
def __init__(self, document, load_options, parser_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | The source input stream. |
| load_options | `LoadOptions` | The options to open the file. |
| parser_settings | `ParserSettings` | The parser settings which are used to customize data extraction. |

### Example

```python
from groupdocs.parser import Parser
from groupdocs.parser.options import LoadOptions, ParserSettings

with open("sample.pdf", "rb") as stream:
    parser = Parser(stream, LoadOptions(), ParserSettings(lambda level, message, exception: print(level, message)))
    text_reader = parser.get_text()
    if text_reader is not None:
        print(text_reader.read_to_end())
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)
