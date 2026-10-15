---
title: "PageTextAreaOptions"
second_title: "GroupDocs.Parser voor .NET API-referentie"
description: "Initialiseert een nieuw exemplaar van de PageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions‑klasse met de OCR‑gebruiksoptie."
type: docs
weight: 10
url: /nl/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---

## PageTextAreaOptions() {#constructor}

Initialiseert een nieuw exemplaar van de [`PageTextAreaOptions`](../../pagetextareaoptions)‑klasse met de OCR‑gebruiksoptie.

```csharp
public PageTextAreaOptions()
```

### Zie ook

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`PageTextAreaOptions`](../../pagetextareaoptions)‑klasse met de OCR‑gebruiksoptie.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| useOcr | Boolean | De waarde die aangeeft of OCR-functionaliteit wordt gebruikt om tekstgebieden te extraheren. |

### Zie ook

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`PageTextAreaOptions`](../../pagetextareaoptions)‑klasse met de mogelijkheid om OCR‑opties in te stellen.

```csharp
public PageTextAreaOptions(bool useOcr, OcrOptions ocrOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| useOcr | Boolean | De waarde die aangeeft of OCR-functionaliteit wordt gebruikt om tekstgebieden te extraheren. |
| ocrOptions | OcrOptions | De extra opties voor OCR-functionaliteit. |

### Zie ook

* class [OcrOptions](../../ocroptions)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_3}

Initialiseert een nieuw exemplaar van de [`PageTextAreaOptions`](../../pagetextareaoptions)‑klasse met de reguliere expressie. Andere opties worden standaard ingesteld (zie opmerkingen voor details).

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| expression | String | De reguliere expressie. |

### Opmerkingen

De volgende eigenschappen hebben standaardwaarden:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`null`

### Zie ook

* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_6}

Initialiseert een nieuw exemplaar van de [`PageTextAreaOptions`](../../pagetextareaoptions) klasse met de reguliere expressie en het rechthoekige gebied. Andere opties worden standaard ingesteld (zie opmerkingen voor details).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| expression | String | De reguliere expressie. |
| rectangle | Rectangle | Het rechthoekige gebied dat paginagebieden bevat. |

### Opmerkingen

De volgende eigenschappen hebben standaardwaarden:

**[`MatchCase`](../matchcase)**

`false`

**[`UniteSegments`](../unitesegments)**

`false`

**[`IgnoreFormatting`](../ignoreformatting)**

`false`

### Zie ook

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle, double) {#constructor_7}

Initialiseert een nieuw exemplaar van de [`PageTextAreaOptions`](../../pagetextareaoptions) klasse met de reguliere expressie, het rechthoekige gebied en de grootte van de genegeerde rand. Andere opties worden standaard ingesteld (zie opmerkingen voor details).

```csharp
public PageTextAreaOptions(string expression, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| expression | String | De reguliere expressie. |
| rectangle | Rectangle | Het rechthoekige gebied dat paginagebieden bevat. |
| rectangleTolerance | Double | De grootte van de rand die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. Het wordt gemeten als een fractie van de hoogte van een tekstelement. |

### Zie ook

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_4}

Initialiseert een nieuw exemplaar van de [`PageTextAreaOptions`](../../pagetextareaoptions) klasse.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| expression | String | De reguliere expressie. |
| matchCase | Boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
| uniteSegments | Boolean | De waarde die aangeeft of segmenten worden samengevoegd. |
| ignoreFormatting | Boolean | De waarde die aangeeft of tekstopmaak wordt genegeerd. |
| rectangle | Rectangle | Het rechthoekige gebied dat paginagebieden bevat. |

### Zie ook

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle, double) {#constructor_5}

Initialiseert een nieuw exemplaar van de [`PageTextAreaOptions`](../../pagetextareaoptions) klasse met de grootte van de genegeerde rand.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| expression | String | De reguliere expressie. |
| matchCase | Boolean | De waarde die aangeeft of een tekstcase niet wordt genegeerd. |
| uniteSegments | Boolean | De waarde die aangeeft of segmenten worden samengevoegd. |
| ignoreFormatting | Boolean | De waarde die aangeeft of tekstopmaak wordt genegeerd. |
| rectangle | Rectangle | Het rechthoekige gebied dat paginagebieden bevat. |
| rectangleTolerance | Double | De grootte van de rand die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. Het wordt gemeten als een fractie van de hoogte van een tekstelement. |

### Zie ook

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
