---
title: License
second_title: GroupDocs.Parser for Java API Reference
description: Represents GroupDocs.Parser license.
type: docs
weight: 10
url: /java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Represents GroupDocs.Parser license.

This example demonstrates how to setup license.

```

 // Initialize License class
 License license = new License();
 // Set path to .lic file
 license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
```
## Constructors

| Constructor | Description |
| --- | --- |
| [License()](#License--) | Initializes a new instance of the [License](../../com.groupdocs.parser.licensing/license) class. |
## Methods

| Method | Description |
| --- | --- |
| [setLicense(String filePath)](#setLicense-java.lang.String-) | Licenses the component. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licenses the component. |
### License() {#License--}
```
public License()
```


Initializes a new instance of the [License](../../com.groupdocs.parser.licensing/license) class.

### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Licenses the component.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Absolute path to license file. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licenses the component.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | License stream. |

