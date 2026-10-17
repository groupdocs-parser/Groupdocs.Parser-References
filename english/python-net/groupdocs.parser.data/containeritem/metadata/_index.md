---
title: metadata property
second_title: GroupDocs.Parser for Python via .NET API References
description: "The collection of metadata items."
type: docs
url: /python-net/groupdocs.parser.data/containeritem/metadata/
is_root: false
weight: 2030
---


## metadata property

The collection of metadata items.

These metadata refer to a container element itself, not a document. Depending on the container type, metadata can contain the following items:

Email Attachments
- content-type: The MIME type of the attachment content.

ZIP Archives
- date: The time and date at which the file indicated by the Zip Entry was last modified.
- disposition: To detect if an image attachment is inline, the `disposition` metadata is used. If present, it can take `inline` or `attachment` values.

Outlook Storage
- date: The time and date at which the Outlook Storage item was last modified.
- email-sender: The value of the "sender" field.
- email-to: The value of the "to" field.
- subject: The value of the "subject" field.

### Definition:
```python
@property
def metadata(self):
    ...
```

### See Also
* class [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem/)
