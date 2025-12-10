---
title: move_to method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.templates/templatetablelayout/move_to/
is_root: false
weight: 20
---

## move_to {#groupdocs.parser.data.Point}

Creates a new layout with the same size, separators and position in the `point`.


### Returns 


A new layout with the same size, separators and position in the `point`.


```python
def move_to(self, point):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| point | groupdocs.parser.data.Point | The position of the new layout. |

### Example 


This functionality allows to move Table Layout.




For example, a document has tables on each page (or a set of documents with a table on the page). 
These tables differ by position and content, but have the same columns and rows. In this case a user can define 
[`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout) object at `(0, 0)` once and then move it to the location of the definite table.




If the table position depends on the other object of the page, a user can define [`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout) object based 
on template document and then move it according to an anchor object. For example, if this is a summary table and 
it is followed by details table (which can contain a different count of rows). In this case a user can define 
[`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout) object on template document (with the known details table rectangle) and then move 
[`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout) object according to the difference of details table rectangle of template and real document.



[`TemplateTableLayout.move_to`](/parser/python-net/groupdocs.parser.templates/templatetablelayout/move_to) method returns a copy of the current object. 
A user can pass any coordinates (even negative - then layout will be moved to the left/top).



### See Also
* module [`groupdocs.parser.templates`](../../)
* class [`TemplateTableLayout`](/parser/python-net/groupdocs.parser.templates/templatetablelayout)
