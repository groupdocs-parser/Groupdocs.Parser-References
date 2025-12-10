---
title: get_file_info method
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser/parser/get_file_info/
is_root: false
weight: 70
---

## get_file_info {#System.String}

Returns the general information about a file.


### Returns 


An instance of [`FileInfo`](/parser/python-net/groupdocs.parser.options/fileinfo) class.


```python
def get_file_info(self, file_path):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | System.String | The path to the file. |

### Example 


The following code shows how to check whether a file is password-protected:


## get_file_info {#io.RawIOBase}

Returns the general information about a file.


### Returns 


An instance of [`FileInfo`](/parser/python-net/groupdocs.parser.options/fileinfo) class.


```python
def get_file_info(self, document):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | The source input stream. |

### Example 


The following code shows how to check whether a file is password-protected:


## get_file_info {#System.String-groupdocs.parser.options.LoadOptions}

Returns the general information about a file.


### Returns 


An instance of [`FileInfo`](/parser/python-net/groupdocs.parser.options/fileinfo) class.


```python
def get_file_info(self, file_path, load_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | System.String | The path to the file. |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the file. |

### Example 


The following code shows how to check a file type of the password-protected document:


## get_file_info {#io.RawIOBase-groupdocs.parser.options.LoadOptions}

Returns the general information about a file.


### Returns 


An instance of [`FileInfo`](/parser/python-net/groupdocs.parser.options/fileinfo) class.


```python
def get_file_info(self, document, load_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | The source input stream. |
| load_options | groupdocs.parser.options.LoadOptions | The options to open the file. |

### Example 


The following code shows how to check a file type of the password-protected document:



### See Also
* module [`groupdocs.parser`](../../)
* class [`FileInfo`](/parser/python-net/groupdocs.parser.options/fileinfo)
* class [`Parser`](/parser/python-net/groupdocs.parser/parser)
