---
title: TemplateTable constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.templates/templatetable/__init__/
is_root: false
weight: 10
---

## __init__ {#groupdocs.parser.templates.TemplateTableLayout-System.String}

Initializes a new instance of the [`TemplateTable`](/parser/python-net/groupdocs.parser.templates/templatetable) class with the UPPER CASE name.



```python
def __init__(self, layout, name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| layout | groupdocs.parser.templates.TemplateTableLayout | The table layout. |
| name | System.String | The table name. |

### Example 


Template table is set by table layout if the table can't be detected automatically:


## __init__ {#groupdocs.parser.templates.TemplateTableParameters-System.String}

Initializes a new instance of the [`TemplateTable`](/parser/python-net/groupdocs.parser.templates/templatetable) class.



```python
def __init__(self, parameters, name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| parameters | groupdocs.parser.templates.TemplateTableParameters | The parameters to detect the table in the automatic mode. |
| name | System.String | The table name. |

### Example 


If a template table is set by detector parameters, the table is detected automatically:


## __init__ {#groupdocs.parser.templates.TemplateTableLayout-System.String-System.Nullable`1[[System.Double]]}

Constructs a new instance of TemplateTable



```python
def __init__(self, layout, name, page_width):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| layout | groupdocs.parser.templates.TemplateTableLayout |  |
| name | System.String |  |
| page_width | System.Nullable`1[[System.Double]] |  |


## __init__ {#groupdocs.parser.templates.TemplateTableParameters-System.String-System.Nullable`1[[System.Double]]}

Constructs a new instance of TemplateTable



```python
def __init__(self, parameters, name, page_width):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| parameters | groupdocs.parser.templates.TemplateTableParameters |  |
| name | System.String |  |
| page_width | System.Nullable`1[[System.Double]] |  |


## __init__ {#groupdocs.parser.templates.TemplateTableLayout-System.String-System.Nullable`1[[System.Double]]-bool}

Constructs a new instance of TemplateTable



```python
def __init__(self, layout, name, page_width, use_upper_case_name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| layout | groupdocs.parser.templates.TemplateTableLayout |  |
| name | System.String |  |
| page_width | System.Nullable`1[[System.Double]] |  |
| use_upper_case_name | bool |  |


## __init__ {#groupdocs.parser.templates.TemplateTableParameters-System.String-System.Nullable`1[[System.Double]]-bool}

Constructs a new instance of TemplateTable



```python
def __init__(self, parameters, name, page_width, use_upper_case_name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| parameters | groupdocs.parser.templates.TemplateTableParameters |  |
| name | System.String |  |
| page_width | System.Nullable`1[[System.Double]] |  |
| use_upper_case_name | bool |  |



### See Also
* module [`groupdocs.parser.templates`](../../)
* class [`TemplateTable`](/parser/python-net/groupdocs.parser.templates/templatetable)
