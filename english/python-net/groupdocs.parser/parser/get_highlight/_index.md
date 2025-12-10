---
title: get_highlight method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_highlight/
is_root: false
weight: 90
---

## get_highlight {#int-bool-groupdocs.parser.options.HighlightOptions}

Extracts a highlight from the document.


### Returns 


An instance of [`HighlightItem`](/parser/python-net/groupdocs.parser.data/highlightitem) class that represents the extracted highlight;
`null` if highlight extraction isn't supported.


```python
def get_highlight(self, position, is_direct, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| position | int | The start position of the highlight. |
| is_direct | bool | The value that indicates whether highlight extraction is direct.<br/>`true` if the higlight is extracted by the right of `position`; otherwise, `false`. |
| options | groupdocs.parser.options.HighlightOptions | The highlight extraction options. |

### Example 


The following example shows how to extract a highlight that contains 3 words:



### See Also
* module [`groupdocs.parser`](../../)
* class [`HighlightItem`](/parser/python-net/groupdocs.parser.data/highlightitem)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
