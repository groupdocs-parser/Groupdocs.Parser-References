---
title: "TemplateLinkedPositionEdges"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "टेक्स्ट फ़ील्ड खोजे जाने वाले लिंक्ड फ़ील्ड के किनारे प्रदान करता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

लिंक्ड फ़ील्ड के किनारों को प्रदान करता है जहाँ टेक्स्ट फ़ील्ड खोजा जाता है। [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) का उपयोग [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) क्लास में किया जाता है।

## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) क्लास का नया उदाहरण प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | उस मान को प्राप्त करता है जो दर्शाता है कि उदाहरण खाली है या नहीं। |
|
|  | [isLeft()](#isLeft--) | उस मान को प्राप्त करता है जो दर्शाता है कि लिंक्ड फ़ील्ड से बाएँ की ओर फ़ील्ड खोजा गया है या नहीं। |
|
|  | [isTop()](#isTop--) | उस मान को प्राप्त करता है जो दर्शाता है कि लिंक्ड फ़ील्ड से ऊपर की ओर फ़ील्ड खोजा गया है या नहीं। |
|
|  | [isRight()](#isRight--) | उस मान को प्राप्त करता है जो दर्शाता है कि लिंक्ड फ़ील्ड से दाएँ की ओर फ़ील्ड खोजा गया है या नहीं। |
|
|  | [isBottom()](#isBottom--) | उस मान को प्राप्त करता है जो दर्शाता है कि लिंक्ड फ़ील्ड से नीचे की ओर फ़ील्ड खोजा गया है या नहीं। |
|
|  | [parse(String s)](#parse-java.lang.String-) | किनारों के स्ट्रिंग प्रतिनिधित्व को उसकी क्लास समकक्ष में परिवर्तित करता है। |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) क्लास का नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | बाएँ | boolean | वह मान जो दर्शाता है कि लिंक्ड फ़ील्ड से बाएँ की ओर फ़ील्ड खोजा गया है। |
|
|  | ऊपर | boolean | वह मान जो दर्शाता है कि लिंक्ड फ़ील्ड से ऊपर की ओर फ़ील्ड खोजा गया है। |
|
|  | दाएँ | boolean | वह मान जो दर्शाता है कि कोई फ़ील्ड लिंक किए गए फ़ील्ड से दाएँ खोजा गया है या नहीं। |
|
|  | नीचे | boolean | वह मान जो दर्शाता है कि कोई फ़ील्ड लिंक किए गए फ़ील्ड से नीचे खोजा गया है या नहीं। |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


उस मान को प्राप्त करता है जो दर्शाता है कि उदाहरण खाली है या नहीं।


**Returns:**
boolean -  true  यदि इंस्टेंस खाली है (सभी फ़ील्ड false हैं); अन्यथा, false ।

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


उस मान को प्राप्त करता है जो दर्शाता है कि लिंक्ड फ़ील्ड से बाएँ की ओर फ़ील्ड खोजा गया है या नहीं।


**Returns:**
boolean -  true  यदि फ़ील्ड लिंक किए गए फ़ील्ड से बाएँ खोजा गया है; अन्यथा, false ।

### isTop() {#isTop--}
```
public boolean isTop()
```


उस मान को प्राप्त करता है जो दर्शाता है कि लिंक्ड फ़ील्ड से ऊपर की ओर फ़ील्ड खोजा गया है या नहीं।


**Returns:**
boolean -  true  यदि फ़ील्ड लिंक किए गए फ़ील्ड से ऊपर खोजा गया है; अन्यथा, false ।

### isRight() {#isRight--}
```
public boolean isRight()
```


उस मान को प्राप्त करता है जो दर्शाता है कि लिंक्ड फ़ील्ड से दाएँ की ओर फ़ील्ड खोजा गया है या नहीं।


**Returns:**
boolean -  true  यदि फ़ील्ड लिंक किए गए फ़ील्ड से दाएँ खोजा गया है; अन्यथा, false ।

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


उस मान को प्राप्त करता है जो दर्शाता है कि लिंक्ड फ़ील्ड से नीचे की ओर फ़ील्ड खोजा गया है या नहीं।


**Returns:**
boolean -  true  यदि फ़ील्ड लिंक किए गए फ़ील्ड से नीचे खोजा गया है; अन्यथा, false ।

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


किनारों के स्ट्रिंग प्रतिनिधित्व को उसकी क्लास समकक्ष में परिवर्तित करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | s | java.lang.String | एक स्ट्रिंग जिसमें परिवर्तित करने के लिए किनारे होते हैं। |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
