---
title: open_parser method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/containeritem/open_parser/
is_root: false
weight: 40
---

## open_parser {#}

Creates the [`Parser`](/parser/python-net/groupdocs.parser/parser) object for the item content.


### Returns 


An instance of [`Parser`](/parser/python-net/groupdocs.parser/parser) class of the item content.


```python
def open_parser(self):
    ...
```




## open_parser {#groupdocs.parser.options.LoadOptions}

Creates the [`Parser`](/parser/python-net/groupdocs.parser/parser) object for the item content with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions).


### Returns 


An instance of [`Parser`](/parser/python-net/groupdocs.parser/parser) class of the item content.


```python
def open_parser(self, load_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the item content. |


## open_parser {#groupdocs.parser.options.LoadOptions-groupdocs.parser.options.ParserSettings}

Creates the [`Parser`](/parser/python-net/groupdocs.parser/parser) object for the item content with [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)
and [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings).


### Returns 


An instance of [`Parser`](/parser/python-net/groupdocs.parser/parser) class of the item content.


```python
def open_parser(self, load_options, parser_settings):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the item content. |
| parser_settings | groupdocs.parser.options.ParserSettings | The parser settings which are used to customize data extraction. |



### See Also
* module [`groupdocs.parser.data`](../../)
* class [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem)
* class [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
* class [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings)
