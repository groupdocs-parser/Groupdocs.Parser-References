---
title: TemplateRegexPosition
second_title: GroupDocs.Parser for Java API Reference
description: Provides a template field position which uses the regular expression.
type: docs
weight: 18
url: /java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Provides a template field position which uses the regular expression.

The following example shows the situation if the document contains "Invoice Number INV-12345" then template field can be defined in the following way:

```
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
```

In this case as a value the entire string is extracted. To extract only a part of the string the regular expression group "value" is used:

```
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
```

In this case as a value "INV-3337" string is extracted.
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Initializes a new instance of the [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) class. |
| [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Initializes a new instance of the [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) class. |
## Methods

| Method | Description |
| --- | --- |
| [getExpression()](#getExpression--) | Gets the regular expression. |
| [isMatchCase()](#isMatchCase--) | Gets the value that indicates whether a text case isn't ignored. |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Initializes a new instance of the [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| expression | java.lang.String | The regular expression. |

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Initializes a new instance of the [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| expression | java.lang.String | The regular expression. |
| matchCase | boolean | The value that indicates whether a text case isn't ignored. |

### getExpression() {#getExpression--}
```
public String getExpression()
```


Gets the regular expression.

**Returns:**
java.lang.String - A string that represents the regular expression.
### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Gets the value that indicates whether a text case isn't ignored.

**Returns:**
boolean -  true  if a text case isn't ignored; otherwise,  false .
