---
title: load method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.templates/template/load/
is_root: false
weight: 20
---

## load {#System.String}

Loads a template from a file.


### Returns 


An instance of [`Template`](/parser/python-net/groupdocs.parser.templates/template) class with loaded template.


```python
def load(self, file_path):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | System.String | The path to the file. |
### Exceptions
| Exception | Description |
| :- | :- |
| [`GroupDocsParserException`](/parser/python-net/groupdocs.parser.exceptions/groupdocsparserexception) | The file does not represent the template in a valid format. |




## load {#io.RawIOBase}

Loads a template from a stream.


### Returns 


An instance of [`Template`](/parser/python-net/groupdocs.parser.templates/template) class with loaded template.


```python
def load(self, stream):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The input stream. |
### Exceptions
| Exception | Description |
| :- | :- |
| [`GroupDocsParserException`](/parser/python-net/groupdocs.parser.exceptions/groupdocsparserexception) | The stream does not represent the template in a valid format. |





### See Also
* module [`groupdocs.parser.templates`](../../)
* class [`GroupDocsParserException`](/parser/python-net/groupdocs.parser.exceptions/groupdocsparserexception)
* class [`Template`](/parser/python-net/groupdocs.parser.templates/template)
