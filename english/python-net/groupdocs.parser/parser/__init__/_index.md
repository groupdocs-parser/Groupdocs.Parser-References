---
title: Parser constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/__init__/
is_root: false
weight: 10
---

## __init__ {#System.Uri}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from an URI.



```python
def __init__(self, uri):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| uri | System.Uri | The Uri the request is sent to. |


## __init__ {#groupdocs.parser.options.EmailConnection}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from a remote email server.



```python
def __init__(self, connection):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| connection | groupdocs.parser.options.EmailConnection | The email connection. |

### Example 


The following example shows how to extract emails from Exchange Server:


## __init__ {#System.String}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class.



```python
def __init__(self, file_path):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | System.String | The path to the file. |

### Example 


The following example shows how to load the document from the local disk:


## __init__ {#io.RawIOBase}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class.



```python
def __init__(self, document):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | The source input stream. |

### Example 


The following example shows how to load the document from the stream:


## __init__ {#System.Uri-groupdocs.parser.options.LoadOptions}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from an URI with `load_options`.



```python
def __init__(self, uri, load_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| uri | System.Uri | The Uri the request is sent to. |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the file. |


## __init__ {#System.Uri-groupdocs.parser.options.ParserSettings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from an URI with `parser_settings`.



```python
def __init__(self, uri, parser_settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| uri | System.Uri | The Uri the request is sent to. |
| parser_settings | groupdocs.parser.options.ParserSettings | The parser settings which are used to customize data extraction. |


## __init__ {#groupdocs.parser.options.EmailConnection-groupdocs.parser.options.ParserSettings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from a remote email server.



```python
def __init__(self, connection, parser_settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| connection | groupdocs.parser.options.EmailConnection | The email connection. |
| parser_settings | groupdocs.parser.options.ParserSettings | The parser settings which are used to customize data extraction. |

### Example 


The following example shows how to extract emails from Exchange Server:


## __init__ {#System.String-groupdocs.parser.options.LoadOptions}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions).



```python
def __init__(self, file_path, load_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | System.String | The path to the file. |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the file. |

### Example 


The document password is passed by LoadOptions class:


## __init__ {#System.String-groupdocs.parser.options.ParserSettings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings).



```python
def __init__(self, file_path, parser_settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | System.String | The path to the file. |
| parser_settings | groupdocs.parser.options.ParserSettings | The parser settings which are used to customize data extraction. |


## __init__ {#io.RawIOBase-groupdocs.parser.options.LoadOptions}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions).



```python
def __init__(self, document, load_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | The source input stream. |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the file. |

### Example 


In some cases it's necessary to define [`FileFormat`](/parser/python-net/groupdocs.parser.options/fileformat). 
Both for special cases (databases, email server) and for detecting file types by the content:


The document password is passed by [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class:


## __init__ {#io.RawIOBase-groupdocs.parser.options.ParserSettings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings).



```python
def __init__(self, document, parser_settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | The source input stream. |
| parser_settings | groupdocs.parser.options.ParserSettings | The parser settings which are used to customize data extraction. |


## __init__ {#System.Uri-groupdocs.parser.options.LoadOptions-groupdocs.parser.options.ParserSettings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class to extract data from an URI with `load_options` and `parser_settings`.



```python
def __init__(self, uri, load_options, parser_settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| uri | System.Uri | The Uri the request is sent to. |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the file. |
| parser_settings | groupdocs.parser.options.ParserSettings | The parser settings which are used to customize data extraction. |


## __init__ {#System.String-groupdocs.parser.options.LoadOptions-groupdocs.parser.options.ParserSettings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)
and [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings).



```python
def __init__(self, file_path, load_options, parser_settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | System.String | The path to the file. |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the file. |
| parser_settings | groupdocs.parser.options.ParserSettings | The parser settings which are used to customize data extraction. |

### Example 


The following example shows how to receive the information via [`ILogger`](/parser/python-net/groupdocs.parser.options/ilogger) interface:


## __init__ {#io.RawIOBase-groupdocs.parser.options.LoadOptions-groupdocs.parser.options.ParserSettings}

Initializes a new instance of the [`Parser`](/parser/python-net/groupdocs.parser/parser) class with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)
and [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings).



```python
def __init__(self, document, load_options, parser_settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | The source input stream. |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the file. |
| parser_settings | groupdocs.parser.options.ParserSettings | The parser settings which are used to customize data extraction. |

### Example 


The following example shows how to receive the information via [`ILogger`](/parser/python-net/groupdocs.parser.options/ilogger) interface:



### See Also
* module [`groupdocs.parser`](../../)
* class [`FileFormat`](/parser/python-net/groupdocs.parser.options/fileformat)
* class [`ILogger`](/parser/python-net/groupdocs.parser.options/ilogger)
* class [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
* class [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings)
