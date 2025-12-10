---
title: parse_pages_by_template method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/parse_pages_by_template/
is_root: false
weight: 220
---

## parse_pages_by_template {#groupdocs.parser.templates.Template}

Parses the document pages by the user-generated template.


### Returns 


A collection of [`DocumentPageData`](/parser/python-net/groupdocs.parser.data/documentpagedata) objects that contains the extracted data;
`null` if parsing by template isn't supported.


```python
def parse_pages_by_template(self, template):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| template | groupdocs.parser.templates.Template | The user-generated template. |


## parse_pages_by_template {#groupdocs.parser.templates.Template-groupdocs.parser.options.ParseByTemplateOptions}

Parses the document pages by the user-generated template using customization options.


### Returns 


A collection of [`DocumentPageData`](/parser/python-net/groupdocs.parser.data/documentpagedata) objects that contains the extracted data;
`null` if parsing by template isn't supported.


```python
def parse_pages_by_template(self, template, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| template | groupdocs.parser.templates.Template | The user-generated template. |
| options | groupdocs.parser.options.ParseByTemplateOptions | The customization options. |



### See Also
* module [`groupdocs.parser`](../../)
* class [`DocumentPageData`](/parser/python-net/groupdocs.parser.data/documentpagedata)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
