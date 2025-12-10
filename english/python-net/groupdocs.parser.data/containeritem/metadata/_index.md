---
title: metadata property
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/containeritem/metadata/
is_root: false
weight: 90
---

## metadata property


Gets the collection of metadata items.

### Remarks 


These metadata refer to a container element itself, not a document. Depending on the container type
metadata can contain the following items:



**Email Attachments** 

| Description |
| :- |
| The MIME type of the attachment content. |


**ZIP Archives** 

| Description |
| :- |
| The time and date at which the file indicated by the Zip Entry was last modified. |
| To detect if image attachment is inline 'disposition' metadata is used. If it's present, it can take 'inline' or 'attachment' values. |


**Outlook Storage** 

| Description |
| :- |
| The time and date at which the Outlook Storage item was last modified. |
| The value of "sender" field. |
| The value of "to" field. |
| The value of "subject" field. |
### Definition:
```python
@property
def metadata(self):
    ...
```

### See Also
* module [`groupdocs.parser.data`](../../)
* class [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem)
