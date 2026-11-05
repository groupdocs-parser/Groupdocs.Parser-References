---
title: Extract Metadata from Documents
linkTitle: "Extract Metadata from Documents"
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extract metadata (author, title, custom properties) from PDF, Office, images, emails, and other formats using GroupDocs.Parser for Python via .NET."
type: docs
url: /python-net/guides/extract-metadata-from-documents-2/
is_root: false
weight: 90
---


GroupDocs.Parser extracts metadata such as author, title, creation date, and custom properties from supported formats (see [supported formats](https://docs.groupdocs.com/parser/python-net/supported-document-formats/)).

## Extract metadata
{{< tabs "example-1" >}}
{{< tab "Python" >}}

```python
from groupdocs.parser import Parser

with Parser("./sample.pdf") as parser:
    metadata_items = parser.get_metadata()
    if metadata_items is None:
        print("Metadata extraction is not supported for this format.")
    else:
        for item in metadata_items:
            print(f"{item.name}: {item.value}")
```

{{< /tab >}}
{{< tab "sample.pdf" >}}

The following sample file is used in this example: [sample.pdf](https://docs.groupdocs.com/parser/python-net/_sample_files/developer-guide/basic-usage/extract-metadata-from-documents/sample.pdf)

{{< /tab >}}
{{< tab "extract-metadata.txt" >}}  
```text
title: Harbor Lane Provisions - Annual Report 2025
subject: Annual report and financial summary
keywords: annual report, wholesale, Autumn Harvest, revenue, logistics
author: Amara Osei
application: Aspose Pty Ltd.
last-saved-time: 02/16/2026 11:00:00
```
[Download full output](https://docs.groupdocs.com/parser/python-net/_output_files/developer-guide/basic-usage/extract-metadata-from-documents/example-1/extract-metadata.txt)
{{< /tab >}}
{{< /tabs >}}

### Steps

1. Create a [`Parser`](/parser/python-net/groupdocs.parser/parser/) for the target document.  
2. Call `get_metadata()` to receive a collection of metadata items.  
3. Iterate through `name` and `value` pairs and process them as needed.

For deeper parsing (attachments, text, images), combine metadata extraction with other basic usage topics.
