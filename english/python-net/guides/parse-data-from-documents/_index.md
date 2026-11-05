---
title: Parse Data from Documents
linkTitle: "Parse Data from Documents"
second_title: GroupDocs.Parser for Python via .NET API References
description: "Extract structured data from documents using templates with GroupDocs.Parser for Python via .NET."
type: docs
url: /python-net/guides/parse-data-from-documents/
is_root: false
weight: 100
---


Use template-based parsing to pull structured values (like invoice numbers, dates, tables) from documents.

## Parse data with a template
{{< tabs "example-1" >}}
{{< tab "Python" >}}

```python
from groupdocs.parser import Parser
from groupdocs.parser.templates import Template, TemplateField, TemplateFixedPosition
from groupdocs.parser.data import Rectangle, Point, Size

template = Template([
    TemplateField(
        TemplateFixedPosition(Rectangle(Point(35.0, 135.0), Size(100.0, 10.0))),
        "CompanyName",
    ),
    TemplateField(
        TemplateFixedPosition(Rectangle(Point(440.0, 115.0), Size(110.0, 15.0))),
        "InvoiceNumber",
    ),
])

with Parser("./invoice.pdf") as parser:
    data = parser.parse_by_template(template)
    if data is None:
        print("Parsing by template isn't supported for this format.")
    else:
        # DocumentData exposes extracted fields as an indexed collection.
        for i in range(data.count):
            field = data[i]
            print(f"{field.name}: {field.text}")
```

{{< /tab >}}
{{< tab "invoice.pdf" >}}

The following sample file is used in this example: [invoice.pdf](https://docs.groupdocs.com/parser/python-net/_sample_files/developer-guide/basic-usage/parse-data-from-documents/invoice.pdf)

{{< /tab >}}
{{< tab "parse-data-with-a-template.txt" >}}  
```text
COMPANYNAME: Northwind Coffee
INVOICENUMBER: HLP-2025-0412
```
[Download full output](https://docs.groupdocs.com/parser/python-net/_output_files/developer-guide/basic-usage/parse-data-from-documents/example-1/parse-data-with-a-template.txt)
{{< /tab >}}
{{< /tabs >}}

### Steps

1. Build a [`Template`](/parser/python-net/groupdocs.parser.templates/template/) with fields or tables (fixed positions, regex, linked positions, etc.).  
2. Call `parser.parse_by_template(template)` to receive [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata/).  
3. Iterate through extracted fields by index (`data.count` and `data[i]`) and process each extracted value based on its type (text, table, etc.).

For complex templates (tables, linked fields, regex fields), see the [advanced templates guide](https://docs.groupdocs.com/parser/python-net/developer-guide/advanced-usage/template-based-parsing/).
