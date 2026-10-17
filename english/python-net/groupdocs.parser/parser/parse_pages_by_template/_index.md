---
title: parse_pages_by_template method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Parses the document pages using the user-generated template."
type: docs
url: /python-net/groupdocs.parser/parser/parse_pages_by_template/
is_root: false
weight: 1520
---


## parse_pages_by_template {#template}

Parses the document pages using the user-generated template.

```python
def parse_pages_by_template(self, template):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| template | `Template` | The user-generated template. |

**Returns:** list[`DocumentPageData`] – Collection of extracted data, or None if parsing by template isn't supported.

## parse_pages_by_template {#template-options}

Parses the document pages by the user-generated template using customization options.

```python
def parse_pages_by_template(self, template, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| template | `Template` | The user-generated template. |
| options | `ParseByTemplateOptions` | The customization options. |

**Returns:** Iterable[`DocumentPageData`] containing the extracted data, or None if parsing by template isn't supported.

### See Also
* class [`Parser`](/parser/python-net/groupdocs.parser/parser/)
