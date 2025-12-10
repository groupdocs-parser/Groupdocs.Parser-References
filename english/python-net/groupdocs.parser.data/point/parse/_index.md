---
title: parse method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/point/parse/
is_root: false
weight: 30
---

## parse {#System.String}

Converts the string representation of a point to its class equivalent.


### Returns 


An instance of [`Point`](/parser/python-net/groupdocs.parser.data/point) class that is equivalent to the value specified in `s` parameter.


```python
def parse(self, s):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| s | System.String | A string that contains a point to convert. |
### Exceptions
| Exception | Description |
| :- | :- |
| ArgumentException | `s` does not represent a point in a valid format. |





### See Also
* module [`groupdocs.parser.data`](../../)
* class [`Point`](/parser/python-net/groupdocs.parser.data/point)
