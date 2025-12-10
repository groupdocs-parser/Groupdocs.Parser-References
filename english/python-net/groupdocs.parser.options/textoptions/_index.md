---
title: TextOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/textoptions/
is_root: false
weight: 360
---

## TextOptions class

Provides the options which are used for text extraction.



The TextOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/textoptions/__init__/#) | Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions) class. |
| [__init__](/parser/python-net/groupdocs.parser.options/textoptions/__init__/#bool) | Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions) class. |
| [__init__](/parser/python-net/groupdocs.parser.options/textoptions/__init__/#bool-bool) | Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions) class with the OCR usage option. |
| [__init__](/parser/python-net/groupdocs.parser.options/textoptions/__init__/#bool-bool-groupdocs.parser.options.OcrOptions) | Initializes a new instance of the [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions) class with the ability to set OCR options. |


### Properties
| Property | Description |
| :- | :- |
| [use_raw_mode_if_possible](/parser/python-net/groupdocs.parser.options/textoptions/use_raw_mode_if_possible) | Gets the value that indicates whether the raw mode is used. |
| [use_ocr](/parser/python-net/groupdocs.parser.options/textoptions/use_ocr) | Gets the value that indicates whether the OCR Connector is used to extract a text. |
| [ocr_options](/parser/python-net/groupdocs.parser.options/textoptions/ocr_options) | Gets the additional options for OCR functionality. |



### Remarks 


An instance of [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions) class is used as parameter
in [`Parser.get_text`](/parser/python-net/groupdocs.parser/parser/get_text) and [`Parser.get_text`](/parser/python-net/groupdocs.parser/parser/get_text) methods. See the usage examples there.




It's used to specify the raw mode of text extraction. 
A text in this mode is extracted in a non-accurate way but faster than in the standard mode. 
If the raw mode doesn't support the document format, then this parameter is ignored and the standard mode is used.


**Learn more:** |
|
 |
 |

### See Also
* module [`groupdocs.parser.options`](..)
* class [`TextOptions`](/parser/python-net/groupdocs.parser.options/textoptions)
