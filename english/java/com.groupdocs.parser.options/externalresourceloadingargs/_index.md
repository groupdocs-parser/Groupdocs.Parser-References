---
title: ExternalResourceLoadingArgs
second_title: GroupDocs.Parser for Java API Reference
description: Provides the data for  method.
type: docs
weight: 16
url: /java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

Provides the data for [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler\#onLoading-ExternalResourceLoadingArgs-) method.
## Constructors

| Constructor | Description |
| --- | --- |
| [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | Initializes a new instance of the [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) class with rectangular area. |
## Methods

| Method | Description |
| --- | --- |
| [getUri()](#getUri--) | Gets the URI of the external resource. |
| [setUri(String uri)](#setUri-java.lang.String-) | Gets the URI of the external resource. |
| [isSkipped()](#isSkipped--) | Gets the value that indicates whether the loading of the external resource must be skipped. |
| [setSkipped(boolean skipped)](#setSkipped-boolean-) | Sets the value that indicates whether the loading of the external resource must be skipped. |
| [getData()](#getData--) | Gets the user data. |
| [setData(byte[] data)](#setData-byte---) | Sets the user data. |
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


Initializes a new instance of the [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) class with rectangular area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uri | java.lang.String | URI of the external resource. |

### getUri() {#getUri--}
```
public String getUri()
```


Gets the URI of the external resource.

**Returns:**
java.lang.String - A string value that represents URI of the external resource.
### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


Gets the URI of the external resource.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uri | java.lang.String | A string value that represents a new URI of the external resource. |

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


Gets the value that indicates whether the loading of the external resource must be skipped.

**Returns:**
boolean - true if the loading of the external resource must be skipped; otherwise, false.
### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


Sets the value that indicates whether the loading of the external resource must be skipped.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| skipped | boolean | true if the loading of the external resource must be skipped; otherwise, false. |

### getData() {#getData--}
```
public byte[] getData()
```


Gets the user data.

**Returns:**
byte[] - The byte array with the user content of the external resource. null if isn't set.
### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


Sets the user data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | byte[] | The byte array with the user content of the external resource. null if isn't set. |

