---
title: try_parse method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/point/try_parse/
is_root: false
weight: 40
---

## try_parse {#System.String-any}

Converts the string representation of a point to its class equivalent.
A return value indicates whether the conversion is succeeded or failed.


### Returns 


`true` if `s` is converted successfully; otherwise, `false`.


```python
def try_parse(self, s, point):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| s | System.String | A string containing a point to convert. |
| point | any | When the method returns, it contains the instance of [`Point`](/parser/python-net/groupdocs.parser.data/point) class <br/>that is equivalent to the value specified in `s` parameter, if the conversion is succeeded; otherwise, `null`. |



### See Also
* module [`groupdocs.parser.data`](../../)
* class [`Point`](/parser/python-net/groupdocs.parser.data/point)
