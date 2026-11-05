---
title: Extract Data from Attachments and ZIP Archives
linkTitle: "Extract Data from Attachments"
second_title: GroupDocs.Parser for Python via .NET API References
description: "Work with containers such as ZIP archives, email stores, and PDF portfolios using GroupDocs.Parser for Python via .NET."
type: docs
url: /python-net/guides/extract-data-from-attachments-and-zip-archives/
is_root: false
weight: 110
---


Use container extraction to open archive-like formats (ZIP, RAR, TAR), Outlook stores (PST/OST), PDF portfolios, and email attachments, then parse their contents.

## Extract and parse attachments
{{< tabs "example-1" >}}
{{< tab "Python" >}}

```python
from groupdocs.parser import Parser
from groupdocs.parser.exceptions import UnsupportedDocumentFormatException

with Parser("./archive.zip") as parser:
    attachments = parser.get_container()
    if attachments is None:
        print("Container extraction isn't supported for this format.")
    else:
        for item in attachments:
            print(item.file_path)
            try:
                with item.open_parser() as attachment_parser:
                    reader = attachment_parser.get_text()
                    print(reader.read_to_end() if reader is not None else "No text available.")
            except UnsupportedDocumentFormatException:
                print("Item format is not supported.")
```

{{< /tab >}}
{{< tab "archive.zip" >}}

The following sample file is used in this example: [archive.zip](https://docs.groupdocs.com/parser/python-net/_sample_files/developer-guide/basic-usage/extract-data-from-attachments-and-zip-archives/archive.zip)

{{< /tab >}}
{{< tab "extract-and-parse-attachments.txt" >}}  
```text
finance/invoice-HLP-2025-0412.pdf
                                                                                           INVOICE

   FROM                                                                     Invoice Number      HLP-2025-0412
   Northwind Coffee Roasters                                                Invoice Date        4 November 2025
   4 Roastery Lane, Millbrook                                               Due Date            4 December 2025
   alex.chen@northwindroa
[TRUNCATED]
```
[Download full output](https://docs.groupdocs.com/parser/python-net/_output_files/developer-guide/basic-usage/extract-data-from-attachments-and-zip-archives/example-1/extract-and-parse-attachments.txt)
{{< /tab >}}
{{< /tabs >}}

### Steps

1. Instantiate [`Parser`](/parser/python-net/groupdocs.parser/parser/) for the container file.  
2. Call `get_container()` to list [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem/) entries.  
3. For each item, use `open_parser()` to create a [`Parser`](/parser/python-net/groupdocs.parser/parser/) over the embedded content and reuse standard extraction methods (`get_text`, `get_images`, `get_metadata`, etc.).  
4. Handle unsupported formats with [`UnsupportedDocumentFormatException`](/parser/python-net/groupdocs.parser.exceptions/unsupporteddocumentformatexception/).

For working with attachments in complex scenarios (nested containers, load options), see the [advanced containers guide](https://docs.groupdocs.com/parser/python-net/developer-guide/advanced-usage/working-with-archives/).
