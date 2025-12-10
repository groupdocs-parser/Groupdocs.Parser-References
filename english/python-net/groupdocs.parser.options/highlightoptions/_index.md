---
title: HighlightOptions class
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/highlightoptions/
is_root: false
weight: 140
---

## HighlightOptions class

Provides the options which are used to extract a highlight (a block of text aroud found text in search scenarios).



The HighlightOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/#) | Initializes a new instance of the [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions) class which is used to extract a fixed-length highlight. |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/#int) | Initializes a new instance of the [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions) class which is used to extract a fixed-length highlight. |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/#System.Nullable`1[[System.Int32]]-bool) | Constructs a new instance of HighlightOptions |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/#System.Nullable`1[[System.Int32]]-int) | Constructs a new instance of HighlightOptions |
| [__init__](/parser/python-net/groupdocs.parser.options/highlightoptions/__init__/#System.Nullable`1[[System.Int32]]-System.Nullable`1[[System.Int32]]-bool) | Constructs a new instance of HighlightOptions |


### Properties
| Property | Description |
| :- | :- |
| [max_length](/parser/python-net/groupdocs.parser.options/highlightoptions/max_length) | Gets a maximum text length. |
| [word_count](/parser/python-net/groupdocs.parser.options/highlightoptions/word_count) | Gets a maximum word count. |
| [is_line_limited](/parser/python-net/groupdocs.parser.options/highlightoptions/is_line_limited) | Gets value that indicates whether highlight extraction is limited by the start (or the end) of a text line. |



### Remarks 


An instance of [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions) class is used as parameter 
in [`Parser.get_highlight`](/parser/python-net/groupdocs.parser/parser/get_highlight) method.
See the usage examples there.

### See Also
* module [`groupdocs.parser.options`](..)
* class [`HighlightOptions`](/parser/python-net/groupdocs.parser.options/highlightoptions)
