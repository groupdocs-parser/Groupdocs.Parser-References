---
title: TemplateLinkedPositionEdges
second_title: GroupDocs.Parser for Java API Reference
description: Provides the edges of the linked field where the text field is seached.
type: docs
weight: 16
url: /java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Provides the edges of the linked field where the text field is seached. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) is used in [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) class.
## Constructors

| Constructor | Description |
| --- | --- |
| [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Initializes a new instance of the [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class. |
## Methods

| Method | Description |
| --- | --- |
| [isEmpty()](#isEmpty--) | Gets the value that indicates whether the instance is empty. |
| [isLeft()](#isLeft--) | Gets the value that indicates whether a field is searched by the left from the linked field. |
| [isTop()](#isTop--) | Gets the value that indicates whether a field is searched by the top from the linked field. |
| [isRight()](#isRight--) | Gets the value that indicates whether a field is searched by the right from the linked field. |
| [isBottom()](#isBottom--) | Gets the value that indicates whether a field is searched by the bottom from the linked field. |
| [parse(String s)](#parse-java.lang.String-) | Converts the string representation of edges to its class equivalent. |
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Initializes a new instance of the [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| left | boolean | The value that indicates whether a field is searched by the left from the linked field. |
| top | boolean | The value that indicates whether a field is searched by the top from the linked field. |
| right | boolean | The value that indicates whether a field is searched by the right from the linked field. |
| bottom | boolean | The value that indicates whether a field is searched by the bottom from the linked field. |

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Gets the value that indicates whether the instance is empty.

**Returns:**
boolean -  true  if the instance is empty (all fields are  false ); otherwise,  false .
### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Gets the value that indicates whether a field is searched by the left from the linked field.

**Returns:**
boolean -  true  if a field is searched by the left from the linked field; otherwise,  false .
### isTop() {#isTop--}
```
public boolean isTop()
```


Gets the value that indicates whether a field is searched by the top from the linked field.

**Returns:**
boolean -  true  if a field is searched by the top from the linked field; otherwise,  false .
### isRight() {#isRight--}
```
public boolean isRight()
```


Gets the value that indicates whether a field is searched by the right from the linked field.

**Returns:**
boolean -  true  if a field is searched by the right from the linked field; otherwise,  false .
### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Gets the value that indicates whether a field is searched by the bottom from the linked field.

**Returns:**
boolean -  true  if a field is searched by the bottom from the linked field; otherwise,  false .
### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Converts the string representation of edges to its class equivalent.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.lang.String | A string that contains edges to convert. |

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
