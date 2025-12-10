---
title: features property
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/features/
is_root: false
weight: 250
---

## features property


Gets the supported features.

### Remarks 


**Learn more:** |
|
 |

### Example 


If the feature isn't supported, the method returns `null` instead of the value. 
Some operations may consume significant time. So it's not optimal to call the method to just check the support for the feature. 
For this purpose Features property is used:
### Definition:
```python
@property
def features(self):
    ...
```

### See Also
* module [`groupdocs.parser`](../../)
* class [`Features`](/parser/python-net/groupdocs.parser.options/features)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
