---
title: Features
second_title: GroupDocs.Parser for Java API Reference
description: Represents the supported features list.
type: docs
weight: 17
url: /java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Represents the supported features list. Allows to obtain information which features are supported or not for the document.

An instance of this class is used as [Parser.getFeatures()](../../com.groupdocs.parser/parser\#getFeatures--) property. See the usage examples there.

**Learn more:**

 *  [Get supported features][]


[Get supported features]: https://docs.groupdocs.com/display/parserjava/Get+supported+features
## Constructors

| Constructor | Description |
| --- | --- |
| [Features()](#Features--) |  |
## Methods

| Method | Description |
| --- | --- |
| [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Returns the value that indicates whether the feature is supported. |
| [isText()](#isText--) | Gets the value that indicates whether text extraction is supported. |
| [isTextPage()](#isTextPage--) | Gets the value that indicates whether text page extraction is supported. |
| [isFormattedText()](#isFormattedText--) | Gets the value that indicates whether formatted text extraction is supported. |
| [isFormattedTextPage()](#isFormattedTextPage--) | Gets the value that indicates whether formatted text page extraction is supported. |
| [isSearch()](#isSearch--) | Gets the value that indicates whether text search is supported. |
| [isHighlight()](#isHighlight--) | Gets the value that indicates whether highlight extraction is supported. |
| [isBarcodes()](#isBarcodes--) | Gets the value that indicates whether barcodes extraction is supported. |
| [isToc()](#isToc--) | Gets the value that indicates whether table of contents extraction is supported. |
| [isMetadata()](#isMetadata--) | Gets the value that indicates whether metadata extraction is supported. |
| [isContainer()](#isContainer--) | Gets the value that indicates whether container extraction is supported. |
| [isTextAreas()](#isTextAreas--) | Gets the value that indicates whether text areas extraction is supported. |
| [isStructure()](#isStructure--) | Gets the value that indicates whether text structure extraction is supported. |
| [isImages()](#isImages--) | Gets the value that indicates whether images extraction is supported. |
| [isHyperlinks()](#isHyperlinks--) | Gets the value that indicates whether hyperlinks extraction is supported. |
| [isTables()](#isTables--) | Gets the value that indicates whether tables extraction is supported. |
| [isParseByTemplate()](#isParseByTemplate--) | Gets the value that indicates whether parsing by template is supported. |
| [isParseForm()](#isParseForm--) | Gets the value that indicates whether form parsing is supported. |
| [isPreview()](#isPreview--) | Gets the value that indicates whether preview generation is supported. |
| [isOcr()](#isOcr--) | Gets the value that indicates whether OCR functionality is supported. |
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Returns the value that indicates whether the feature is supported.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| featureName | java.lang.String | The feature name. |

**Returns:**
boolean -  true  if the feature is supported; otherwise,  false .
### isText() {#isText--}
```
public boolean isText()
```


Gets the value that indicates whether text extraction is supported.

**Returns:**
boolean -  true  if text extraction is supported; otherwise,  false .
### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Gets the value that indicates whether text page extraction is supported.

**Returns:**
boolean -  true  if text page extraction is supported; otherwise,  false .
### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Gets the value that indicates whether formatted text extraction is supported.

**Returns:**
boolean -  true  if formatted text extraction is supported; otherwise,  false .
### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Gets the value that indicates whether formatted text page extraction is supported.

**Returns:**
boolean -  true  if formatted text page is supported; otherwise,  false .
### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Gets the value that indicates whether text search is supported.

**Returns:**
boolean -  true  if text search is supported; otherwise,  false .
### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Gets the value that indicates whether highlight extraction is supported.

**Returns:**
boolean -  true  if highlight extraction is supported; otherwise,  false .
### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Gets the value that indicates whether barcodes extraction is supported.

**Returns:**
boolean -  true  if barcodes extraction is supported; otherwise,  false .
### isToc() {#isToc--}
```
public boolean isToc()
```


Gets the value that indicates whether table of contents extraction is supported.

**Returns:**
boolean -  true  if table of contents extraction is supported; otherwise,  false .
### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Gets the value that indicates whether metadata extraction is supported.

**Returns:**
boolean -  true  if metadata extraction is supported; otherwise,  false .
### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Gets the value that indicates whether container extraction is supported.

**Returns:**
boolean -  true  if container extraction is supported; otherwise,  false .
### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Gets the value that indicates whether text areas extraction is supported.

**Returns:**
boolean -  true  if text areas extraction is supported; otherwise,  false .
### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Gets the value that indicates whether text structure extraction is supported.

**Returns:**
boolean -  true  if text structure extraction is supported; otherwise,  false .
### isImages() {#isImages--}
```
public boolean isImages()
```


Gets the value that indicates whether images extraction is supported.

**Returns:**
boolean -  true  if images extraction is supported; otherwise,  false .
### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Gets the value that indicates whether hyperlinks extraction is supported.

**Returns:**
boolean -  true  if hyperlinks extraction is supported; otherwise,  false .
### isTables() {#isTables--}
```
public boolean isTables()
```


Gets the value that indicates whether tables extraction is supported.

**Returns:**
boolean -  true  if tables extraction is supported; otherwise,  false .
### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Gets the value that indicates whether parsing by template is supported.

**Returns:**
boolean -  true  if parsing by template is supported; otherwise,  false .
### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Gets the value that indicates whether form parsing is supported.

**Returns:**
boolean -  true  if form parsing is supported; otherwise,  false .
### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Gets the value that indicates whether preview generation is supported.

**Returns:**
boolean -  true  if preview generation is supported; otherwise,  false .
### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Gets the value that indicates whether OCR functionality is supported.

**Returns:**
boolean -  true  if OCR functionality is supported; otherwise,  false .
