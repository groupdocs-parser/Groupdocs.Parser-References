---
title: extract_text method
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extracts a text from the document to which TocItem object refers."
type: docs
url: /python-net/groupdocs.parser.data/tocitem/extract_text/
is_root: false
weight: 1010
---


## extract_text

Extracts a text from the document to which [`TocItem`](/parser/python-net/groupdocs.parser.data/tocitem/) object refers.

```python
def extract_text(self):
    ...
```

**Returns:** io.TextIOBase: An instance with the extracted text.

### Example

```python
    from groupdocs.parser import Parser

    with Parser("./sample.docx") as parser:
        toc_items = parser.get_toc()
        if toc_items is None:
            print("Table of contents extraction isn't supported")
        else:
            for toc_item in toc_items:
                with toc_item.extract_text() as reader:
                    print("----")
                    print(reader.read())
    ```

### See Also
* class [`TocItem`](/parser/python-net/groupdocs.parser.data/tocitem/)
