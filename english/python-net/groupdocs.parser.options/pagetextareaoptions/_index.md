---
title: PageTextAreaOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/pagetextareaoptions/
is_root: false
weight: 300
---

## PageTextAreaOptions class

Provides the options which are used for page text areas extraction.



**Inheritance:** [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) → 
[`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions)



The PageTextAreaOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#) | Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class with the OCR usage option. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#bool) | Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class with the OCR usage option. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#bool-groupdocs.parser.options.OcrOptions) | Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class with the ability to set OCR options. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#System.String) | Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class with the regular expression. <br/>Other options are set by default (see remarks for details). |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#System.String-groupdocs.parser.data.Rectangle) | Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class<br/>with the regular expression and rectangular area. <br/>Other options are set by default (see remarks for details). |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#System.String-groupdocs.parser.data.Rectangle-float) | Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class<br/>with the regular expression, rectangular area and the size of the ignored border. <br/>Other options are set by default (see remarks for details). |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#System.String-bool-bool-bool-groupdocs.parser.data.Rectangle) | Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class. |
| [__init__](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/__init__/#System.String-bool-bool-bool-groupdocs.parser.data.Rectangle-float) | Initializes a new instance of the [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class<br/>with the size of the ignored border. |


### Properties
| Property | Description |
| :- | :- |
| [rectangle](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/rectangle) | Gets the rectangular area that contains page areas. |
| [rectangle_tolerance](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/rectangle_tolerance) | Gets the size of the border that is ignored when captured by the rectangular area. It's measured by the fraction of a text item height. |
| [expression](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/expression) | Gets the regular expression. |
| [match_case](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/match_case) | Gets the value that indicates whether a text case isn't ignored. |
| [unite_segments](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/unite_segments) | Gets the value that indicates whether segments are united. |
| [ignore_formatting](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/ignore_formatting) | Gets the value that indicates whether text formatting is ignored. |
| [use_ocr](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/use_ocr) | Gets the value that indicates whether OCR functionality is used to extract text areas. |
| [ocr_options](/parser/python-net/groupdocs.parser.options/pagetextareaoptions/ocr_options) | Gets the additional options for OCR functionality. |



### Remarks 


An instance of [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions) class is used as parameter 
in [`Parser.get_text_areas`](/parser/python-net/groupdocs.parser/parser/get_text_areas) and [`Parser.get_text_areas`](/parser/python-net/groupdocs.parser/parser/get_text_areas) methods.
See the usage examples there.
**Learn more:** |
|
 |

### See Also
* module [`groupdocs.parser.options`](..)
* class [`PageAreaOptions`](/parser/python-net/groupdocs.parser.options/pageareaoptions)
* class [`PageTextAreaOptions`](/parser/python-net/groupdocs.parser.options/pagetextareaoptions)
