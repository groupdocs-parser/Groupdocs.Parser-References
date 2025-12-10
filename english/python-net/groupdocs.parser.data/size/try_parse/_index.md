---
title: try_parse method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/size/try_parse/
is_root: false
weight: 30
---

## try_parse {#System.String-any}

Converts the string representation of a size to its class equivalent.
A return value indicates whether the conversion is succeeded or failed.


### Returns 


`true` if `s` is converted successfully; otherwise, `false`.


```python
def try_parse(self, s, size):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| s | System.String | A string containing a size to convert. |
| size | any | When the method returns, it contains the instance of [`Size`](/parser/python-net/groupdocs.parser.data/size) class <br/>that is equivalent to the value specified in `s` parameter, if the conversion is succeeded; otherwise, `null`. |



### See Also
* module [`groupdocs.parser.data`](../../)
* class [`Size`](/parser/python-net/groupdocs.parser.data/size)
