---
title: LoadOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/loadoptions/
is_root: false
weight: 210
---

## LoadOptions class

Provides the options which are used to open a file.



The LoadOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class<br/>with empty [`LoadOptions.password`](/parser/python-net/groupdocs.parser.options/loadoptions#password), [`LoadOptions.file_format`](/parser/python-net/groupdocs.parser.options/loadoptions#file_format) equal to [`FileFormat.UNKNOWN`](/parser/python-net/groupdocs.parser.options/fileformat#UNKNOWN)<br/>and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#System.TimeSpan) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with `timeout`. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#System.String) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class<br/>with [`LoadOptions.file_format`](/parser/python-net/groupdocs.parser.options/loadoptions#file_format) equal to [`FileFormat.UNKNOWN`](/parser/python-net/groupdocs.parser.options/fileformat#UNKNOWN)<br/>and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#groupdocs.parser.options.FileFormat) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class<br/>with empty [`LoadOptions.password`](/parser/python-net/groupdocs.parser.options/loadoptions#password) and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#groupdocs.parser.options.FileFormat-System.String) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with the password and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#groupdocs.parser.options.FileFormat-System.String-System.Text.Encoding-System.Text.Encoding) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with custom encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#groupdocs.parser.options.FileFormat-System.String-System.Text.Encoding-System.Text.Encoding-System.TimeSpan) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) fully customized class. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#groupdocs.parser.options.FileType) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class<br/>with empty [`LoadOptions.password`](/parser/python-net/groupdocs.parser.options/loadoptions#password) and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#groupdocs.parser.options.FileType-System.String) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with the password and default encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#groupdocs.parser.options.FileType-System.String-System.Text.Encoding-System.Text.Encoding) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) class with custom encodings. |
| [__init__](/parser/python-net/groupdocs.parser.options/loadoptions/__init__/#groupdocs.parser.options.FileType-System.String-System.Text.Encoding-System.Text.Encoding-System.TimeSpan) | Initializes a new instance of the [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions) fully customized class. |


### Properties
| Property | Description |
| :- | :- |
| [file_format](/parser/python-net/groupdocs.parser.options/loadoptions/file_format) | Gets the file format. |
| [file_type](/parser/python-net/groupdocs.parser.options/loadoptions/file_type) | Gets the file type. |
| [password](/parser/python-net/groupdocs.parser.options/loadoptions/password) | Gets the password. |
| [encoding](/parser/python-net/groupdocs.parser.options/loadoptions/encoding) | Gets the encoding of the document. |
| [default_ansi_encoding](/parser/python-net/groupdocs.parser.options/loadoptions/default_ansi_encoding) | Gets the default ANSI encoding which is used for encoding detection. |
| [timeout](/parser/python-net/groupdocs.parser.options/loadoptions/timeout) | Gets the value that represents the number of milliseconds to wait. |



### Remarks 


An instance of this class is used as parameter in [`Parser`](/parser/python-net/groupdocs.parser/parser) class constructors:
|
|
 |
 |


See the usage examples there.

**Learn more:** |
|
 |
 |

### See Also
* module [`groupdocs.parser.options`](..)
* class [`LoadOptions`](/parser/python-net/groupdocs.parser.options/loadoptions)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
