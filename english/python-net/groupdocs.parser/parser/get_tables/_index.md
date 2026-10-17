---
title: get_tables method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts tables from the document."
type: docs
url: /python-net/groupdocs.parser/parser/get_tables/
is_root: false
weight: 1340
---


## get_tables {#options}

Extracts tables from the document.

```python
def get_tables(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `PageTableAreaOptions` | The options for tables extraction. |

**Returns:** Iterable[PageTableArea] or None if table extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("./sample.xlsx") as parser:
    if not parser.features.tables:
        print("Table extraction isn't supported")
    else:
        tables = parser.get_tables(None)
        if tables:
            for i, table in enumerate(tables, 1):
                print(f"\n=== Table {i} ===")
                for row in range(table.row_count):
                    for col in range(table.column_count):
                        cell = table[row, col]
                        if cell:
                            print(cell.text, end=" | ")
                    print()
```

## get_tables {#page_index-options}

Extracts tables from the document page.

```python
def get_tables(self, page_index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |
| options | `PageTableAreaOptions` | The options for tables extraction. |

**Returns:** list[PageTableArea] or None: A collection of `PageTableArea` objects; `None` if tables extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("report.pdf") as parser:
    if not parser.features.tables:
        print("Table extraction not supported")
    else:
        page_index = 0  # first page
        tables = parser.get_tables(page_index, None)
        if tables:
            for table in tables:
                for row in range(table.row_count):
                    for col in range(table.column_count):
                        cell = table[row, col]
                        if cell:
                            print(cell.text, end=" | ")
                    print()
                print()
```

## get_tables

Extracts tables from the document.

```python
def get_tables(self):
    ...
```

**Returns:** Iterable[PageTableArea] or None: A collection of PageTableArea objects; None if table extraction isn't supported.

### Example

```python
    from groupdocs.parser import Parser

    with Parser("./sample.xlsx") as parser:
        if not parser.features.tables:
            print("Table extraction isn't supported")
        else:
            tables = parser.get_tables(None)
            if tables:
                for table in tables:
                    for row in range(table.row_count):
                        for col in range(table.column_count):
                            cell = table[row, col]
                            if cell:
                                print(cell.text, end=" | ")
                        print()
                    print()
    ```

## get_tables {#page_index}

Extracts tables from the document page.

```python
def get_tables(self, page_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| page_index | `int` | The zero-based page index. |

**Returns:** Iterable[PageTableArea] | None: A collection of `PageTableArea` objects; `None` if tables extraction isn't supported.

### Example

```python
from groupdocs.parser import Parser

with Parser("./report.pdf") as parser:
    if not parser.features.tables:
        print("Table extraction not supported")
    else:
        page_index = 0
        tables = parser.get_tables(page_index)
        if tables:
            print(f"Tables on page {page_index + 1}:")
            for table in tables:
                for row in range(table.row_count):
                    for col in range(table.column_count):
                        cell = table[row, col]
                        if cell:
                            print(cell.text, end=" | ")
                    print()
                print()
```

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)
