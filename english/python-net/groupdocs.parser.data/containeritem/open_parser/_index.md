---
title: open_parser method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Creates the Parser object for the item content."
type: docs
url: /python-net/groupdocs.parser.data/containeritem/open_parser/
is_root: false
weight: 1060
---


## open_parser

Creates the [`Parser`](/parser/python-net/groupdocs.parser/parser/) object for the item content.

```python
def open_parser(self):
    ...
```

**Returns:** An instance of `Parser` class of the item content.

### Example

```python
    from groupdocs.parser import Parser
    from groupdocs.parser.exceptions import UnsupportedDocumentFormatException

    with Parser("portfolio.pdf") as parser:
        container = parser.get_container()
        if container:
            for item in container:
                try:
                    with item.open_parser() as inner_parser:
                        text = inner_parser.get_text().read_to_end()
                        print(f"{item.file_path}: {text if text else '[no text]'}")
                except UnsupportedDocumentFormatException:
                    print(f"{item.file_path}: format is not supported.")
    ```

## open_parser {#load_options}

Creates a [`Parser`](/parser/python-net/groupdocs.parser/parser/) object for the item content with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions/).

```python
def open_parser(self, load_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| load_options | `LoadOptions` | The options to open the item content. |

**Returns:** Parser: An instance of the parser for the item content.

### Example

```python
with item.open_parser() as inner_parser:
    text = inner_parser.get_text().read_to_end()
    print(text)
```

## open_parser {#load_options-parser_settings}

Creates a [`Parser`](/parser/python-net/groupdocs.parser/parser/) object for the item content with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions/) and [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/).

```python
def open_parser(self, load_options, parser_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| load_options | `LoadOptions` | The options to open the item content. |
| parser_settings | `ParserSettings` | The parser settings which are used to customize data extraction. |

**Returns:** An instance of `Parser` for the item content.

### Example

```python
from groupdocs.parser import Parser

with Parser("portfolio.pdf") as parser:
    container = parser.get_container()
    if container:
        for item in container:
            with item.open_parser() as inner_parser:
                text = inner_parser.get_text().read_to_end()
                print(f"{item.file_path}: {text if text else '[no text]'}")
```

### See Also
* class [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem/)
