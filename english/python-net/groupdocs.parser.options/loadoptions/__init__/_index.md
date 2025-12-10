---
title: LoadOptions constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/loadoptions/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class
with empty [`LoadOptions.password`](/parser/python-net/groupdocs.parser.options/loadoptions#password), [`LoadOptions.file_format`](/parser/python-net/groupdocs.parser.options/loadoptions#file_format) equal to [`FileFormat.UNKNOWN`](/parser/python-net/groupdocs.parser.options/fileformat#UNKNOWN)
and default encodings.



```python
def __init__(self):
    ...
```




## __init__ {#System.TimeSpan}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with `timeout`.



```python
def __init__(self, timeout):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| timeout | System.TimeSpan | The TimeSpan that represents the number of milliseconds to wait. |


## __init__ {#System.String}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class
with [`LoadOptions.file_format`](/parser/python-net/groupdocs.parser.options/loadoptions#file_format) equal to [`FileFormat.UNKNOWN`](/parser/python-net/groupdocs.parser.options/fileformat#UNKNOWN)
and default encodings.



```python
def __init__(self, password):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| password | System.String | The password to open the password-protected file. |


## __init__ {#groupdocs.parser.options.FileFormat}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class
with empty [`LoadOptions.password`](/parser/python-net/groupdocs.parser.options/loadoptions#password) and default encodings.



```python
def __init__(self, file_format):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_format | groupdocs.parser.options.FileFormat | The format of the file. |


## __init__ {#groupdocs.parser.options.FileType}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class
with empty [`LoadOptions.password`](/parser/python-net/groupdocs.parser.options/loadoptions#password) and default encodings.



```python
def __init__(self, file_type):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_type | groupdocs.parser.options.FileType | The type of the file. |


## __init__ {#groupdocs.parser.options.FileFormat-System.String}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with the password and default encodings.



```python
def __init__(self, file_format, password):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_format | groupdocs.parser.options.FileFormat | The format of the file. |
| password | System.String | The password to open the password-protected file. |


## __init__ {#groupdocs.parser.options.FileType-System.String}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with the password and default encodings.



```python
def __init__(self, file_type, password):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_type | groupdocs.parser.options.FileType | The type of the file. |
| password | System.String | The password to open the password-protected file. |


## __init__ {#groupdocs.parser.options.FileFormat-System.String-System.Text.Encoding-System.Text.Encoding}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with custom encodings.



```python
def __init__(self, file_format, password, encoding, default_ansi_encoding):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_format | groupdocs.parser.options.FileFormat | The format of the file. |
| password | System.String | The password to open the password-protected file. |
| encoding | System.Text.Encoding | The encoding of the document. |
| default_ansi_encoding | System.Text.Encoding | The default ANSI encoding which is used for encoding detection. |


## __init__ {#groupdocs.parser.options.FileType-System.String-System.Text.Encoding-System.Text.Encoding}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with custom encodings.



```python
def __init__(self, file_type, password, encoding, default_ansi_encoding):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_type | groupdocs.parser.options.FileType | The type of the file. |
| password | System.String | The password to open the password-protected file. |
| encoding | System.Text.Encoding | The encoding of the document. |
| default_ansi_encoding | System.Text.Encoding | The default ANSI encoding which is used for encoding detection. |


## __init__ {#groupdocs.parser.options.FileFormat-System.String-System.Text.Encoding-System.Text.Encoding-System.TimeSpan}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) fully customized class.



```python
def __init__(self, file_format, password, encoding, default_ansi_encoding, timeout):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_format | groupdocs.parser.options.FileFormat | The format of the file. |
| password | System.String | The password to open the password-protected file. |
| encoding | System.Text.Encoding | The encoding of the document. |
| default_ansi_encoding | System.Text.Encoding | The default ANSI encoding which is used for encoding detection. |
| timeout | System.TimeSpan | The TimeSpan that represents the number of milliseconds to wait. |


## __init__ {#groupdocs.parser.options.FileType-System.String-System.Text.Encoding-System.Text.Encoding-System.TimeSpan}

Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) fully customized class.



```python
def __init__(self, file_type, password, encoding, default_ansi_encoding, timeout):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_type | groupdocs.parser.options.FileType | The type of the file. |
| password | System.String | The password to open the password-protected file. |
| encoding | System.Text.Encoding | The encoding of the document. |
| default_ansi_encoding | System.Text.Encoding | The default ANSI encoding which is used for encoding detection. |
| timeout | System.TimeSpan | The TimeSpan that represents the number of milliseconds to wait. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)
