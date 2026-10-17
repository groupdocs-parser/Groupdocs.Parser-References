---
title: IDocumentInfo class
second_title: GroupDocs.Parser for Python via .NET API References
description: "Represents the document information."
type: docs
url: /python-net/groupdocs.parser.options/idocumentinfo/
is_root: false
weight: 190
---


## IDocumentInfo class

Represents the document information.

Objects implementing this interface are returned by [`Parser.get_document_info`](/parser/python-net/groupdocs.parser/parser/get_document_info/) method. See the usage examples there.

Learn more:
- [Get document info](https://docs.groupdocs.com/display/parsernet/Get+document+info)
- [Detect encoding](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

The IDocumentInfo type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [file_type](/parser/python-net/groupdocs.parser.options/idocumentinfo/file_type/) | The document type. |
| [page_count](/parser/python-net/groupdocs.parser.options/idocumentinfo/page_count/) | The total number of document pages. An integer value that represents a total number of pages. |
| [pages](/parser/python-net/groupdocs.parser.options/idocumentinfo/pages/) | The collection of page information, including index and page size, as [`PageInfo`](/parser/python-net/groupdocs.parser.options/pageinfo/) instances. |
| [raw_page_count](/parser/python-net/groupdocs.parser.options/idocumentinfo/raw_page_count/) | The total number of document raw pages. |
| [size](/parser/python-net/groupdocs.parser.options/idocumentinfo/size/) | The size of the document in bytes. An integer value that represents the size of the document in bytes. |

### See Also
* module [`groupdocs.parser.options`](/parser/python-net/groupdocs.parser.options/)
