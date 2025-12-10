---
title: groupdocs.parser.data
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.data/
is_root: false
weight: 10
---

The namespace provides classes which represent parsing results.

### Classes
| Class | Description |
| :- | :- |
| [`ContainerItem`](/parser/python-net/groupdocs.parser.data/containeritem) | Represents a container item like Zip archive entity, email attachment, PDF Portfolio item and so on. |
| [`DocumentData`](/parser/python-net/groupdocs.parser.data/documentdata) | Represents data of the document. It consists of [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata) objects<br/>which contain field data from document. |
| [`DocumentPageData`](/parser/python-net/groupdocs.parser.data/documentpagedata) | Represents data of the document page. It consists of [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata) objects<br/>which contain field data from the document page. |
| [`FieldData`](/parser/python-net/groupdocs.parser.data/fielddata) | Represents field data such as a name, a page index, a field value and so on.<br/>Depending on the field the value can be a text, an image, a table and so on. |
| [`HighlightItem`](/parser/python-net/groupdocs.parser.data/highlightitem) | Represents a highlight, a part of the text which is usually used to explain the context of the found text in the search functionality. |
| [`MetadataItem`](/parser/python-net/groupdocs.parser.data/metadataitem) | Represents a metadata item which is used in container items and metadata extraction functionality. |
| [`Page`](/parser/python-net/groupdocs.parser.data/page) | Represents the document page information such as page index and page size. <br/>It's used to represent the page that contains inheritors of [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea) class<br/>in the parsing by template functionality. |
| [`PageArea`](/parser/python-net/groupdocs.parser.data/pagearea) | Represents an abstract base class for page areas<br/>which are used to represent blocks on the document page in the parsing by template functionality. |
| [`PageBarcodeArea`](/parser/python-net/groupdocs.parser.data/pagebarcodearea) | Represents a page barcode area which is used to represent a barcode value in the parsing by template functionality. |
| [`PageGroupArea`](/parser/python-net/groupdocs.parser.data/pagegrouparea) | Represents a group of page areas<br/>which is used to group different types of blocks of the document page in the parsing by template functionality. |
| [`PageHyperlinkArea`](/parser/python-net/groupdocs.parser.data/pagehyperlinkarea) | Represents a page area which is used to represent a hyperlink on the page. |
| [`PageImageArea`](/parser/python-net/groupdocs.parser.data/pageimagearea) | Represents a page image area which is used to represent an image on the page in the parsing by template functionality<br/>or an image attachment if images are extracted from emails or Zip archives. |
| [`PageTableArea`](/parser/python-net/groupdocs.parser.data/pagetablearea) | Represents a table page area which is used to represent a table in the parsing by template functionality. |
| [`PageTableAreaCell`](/parser/python-net/groupdocs.parser.data/pagetableareacell) | Represents a table cell which is used in [`PageTableArea`](/parser/python-net/groupdocs.parser.data/pagetablearea) class. |
| [`PageTextArea`](/parser/python-net/groupdocs.parser.data/pagetextarea) | Represents a page text area which is used to represent a text value in the parsing by template or parsing form functionality. |
| [`Point`](/parser/python-net/groupdocs.parser.data/point) | Represents a point. |
| [`Rectangle`](/parser/python-net/groupdocs.parser.data/rectangle) | Represents a rectangular area. |
| [`SearchResult`](/parser/python-net/groupdocs.parser.data/searchresult) | Represents the search result in the search functionality. |
| [`Size`](/parser/python-net/groupdocs.parser.data/size) | Represents a size. |
| [`TextStyle`](/parser/python-net/groupdocs.parser.data/textstyle) | Represents the style of the text such as a font name, a font size and so on. |
| [`TocItem`](/parser/python-net/groupdocs.parser.data/tocitem) | Represents the item which is used in the table of contents extraction functionality. |
| [`WorksheetCell`](/parser/python-net/groupdocs.parser.data/worksheetcell) | Represents a worksheet cell. |
| [`WorksheetInfo`](/parser/python-net/groupdocs.parser.data/worksheetinfo) | Represents a sheet info. |
| [`WorksheetRange`](/parser/python-net/groupdocs.parser.data/worksheetrange) | Provides the range which are used for the worksheet extraction. |


