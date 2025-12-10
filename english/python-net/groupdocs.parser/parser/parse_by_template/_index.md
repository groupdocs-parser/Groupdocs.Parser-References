---
title: parse_by_template method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/parse_by_template/
is_root: false
weight: 200
---

## parse_by_template {#groupdocs.parser.templates.Template}

Parses the document by the user-generated template.


### Returns 


An instance of [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata) class that contains the extracted data;
`null` if parsing by template isn't supported.


```python
def parse_by_template(self, template):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| template | groupdocs.parser.templates.Template | The user-generated template. |


## parse_by_template {#groupdocs.parser.templates.Template-groupdocs.parser.options.ParseByTemplateOptions}

Parses the document by the user-generated template using customization options.


### Returns 


An instance of [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata) class that contains the extracted data;
`null` if parsing by template isn't supported.


```python
def parse_by_template(self, template, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| template | groupdocs.parser.templates.Template | The user-generated template. |
| options | groupdocs.parser.options.ParseByTemplateOptions | The customization options. |


## parse_by_template {#groupdocs.parser.templates.TemplateCollection-groupdocs.parser.options.ParseByTemplateOptions}

Selects the most suitable template from the provided collection and then parses the document against the selected template.


### Returns 


An instance of [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata) class that contains the extracted data;
`null` if parsing by template isn't supported.


```python
def parse_by_template(self, template_collection, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| template_collection | groupdocs.parser.templates.TemplateCollection | The template collection. |
| options | groupdocs.parser.options.ParseByTemplateOptions | The customization options. |



### See Also
* module [`groupdocs.parser`](../../)
* class [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
