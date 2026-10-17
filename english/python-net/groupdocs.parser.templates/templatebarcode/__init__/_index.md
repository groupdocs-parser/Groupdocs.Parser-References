---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the TemplateBarcode class."
type: docs
url: /python-net/groupdocs.parser.templates/templatebarcode/__init__/
is_root: false
weight: 10
---


## __init__ {#rectangle-name}

Initializes a new instance of the [`TemplateBarcode`](/parser/python-net/groupdocs.parser.templates/templatebarcode/) class.

```python
def __init__(self, rectangle, name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains the template barcode field. |
| name | `str` | The barcode field name. |

## __init__ {#rectangle-name-page_width}

Initializes a new TemplateBarcode instance.

```python
def __init__(self, rectangle, name, page_width):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains the template barcode field. |
| name | `str` | The barcode field name. |
| page_width | `Optional[float]` | The width of the page that was used to create the template item. |

## __init__ {#rectangle-name-page_width-use_upper_case_name}

Initializes a new TemplateBarcode instance.

```python
def __init__(self, rectangle, name, page_width, use_upper_case_name):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| rectangle | `Rectangle` | The rectangular area that contains the template barcode field. |
| name | `str` | The barcode field name. |
| page_width | `Optional[float]` | The width of the page that was used to create the template item. |
| use_upper_case_name | `bool` | Indicates whether the `name` is converted to UPPER CASE. |

### See Also
* class [`TemplateBarcode`](/parser/python-net/groupdocs.parser.templates/templatebarcode/)
