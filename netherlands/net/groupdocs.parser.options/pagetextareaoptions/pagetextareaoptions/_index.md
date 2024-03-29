---
title: PageTextAreaOptions
second_title: GroupDocs.Parser voor .NET API-referentie
description: Initialiseert een nieuw exemplaar van hetPageTextAreaOptionsgroupdocs.parser.options/pagetextareaoptions class met de OCRgebruiksoptie.
type: docs
weight: 10
url: /nl/net/groupdocs.parser.options/pagetextareaoptions/pagetextareaoptions/
---
## PageTextAreaOptions(bool) {#constructor}

Initialiseert een nieuw exemplaar van het[`PageTextAreaOptions`](../../pagetextareaoptions) class met de OCR-gebruiksoptie.

```csharp
public PageTextAreaOptions(bool useOcr)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| useOcr | Boolean | De waarde die aangeeft of OCR-functionaliteit wordt gebruikt om tekstgebieden te extraheren. |

### Zie ook

* class [PageTextAreaOptions](../../pagetextareaoptions)
* naamruimte [GroupDocs.Parser.Options](../../pagetextareaoptions)
* montage [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(bool, OcrOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`PageTextAreaOptions`](../../pagetextareaoptions) klasse met de mogelijkheid om OCR-opties in te stellen.

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
* naamruimte [GroupDocs.Parser.Options](../../pagetextareaoptions)
* montage [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`PageTextAreaOptions`](../../pagetextareaoptions) klasse met de reguliere expressie. Andere opties zijn standaard ingesteld (zie opmerkingen voor details).

```csharp
public PageTextAreaOptions(string expression)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| expression | String | De reguliere expressie. |

### Opmerkingen

De volgende eigenschappen hebben standaardwaarden:

**[`MatchCase`](../matchcase)**

`vals`

**[`UniteSegments`](../unitesegments)**

`vals`

**[`IgnoreFormatting`](../ignoreformatting)**

`vals`

**[`Rectangle`](../../pageareaoptions/rectangle)**

`nul`

### Zie ook

* class [PageTextAreaOptions](../../pagetextareaoptions)
* naamruimte [GroupDocs.Parser.Options](../../pagetextareaoptions)
* montage [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, Rectangle) {#constructor_4}

Initialiseert een nieuw exemplaar van het[`PageTextAreaOptions`](../../pagetextareaoptions) class met de reguliere expressie en rechthoekig gebied. Andere opties zijn standaard ingesteld (zie opmerkingen voor details).

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

`vals`

**[`UniteSegments`](../unitesegments)**

`vals`

**[`IgnoreFormatting`](../ignoreformatting)**

`vals`

### Zie ook

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* naamruimte [GroupDocs.Parser.Options](../../pagetextareaoptions)
* montage [GroupDocs.Parser](../../../)

---

## PageTextAreaOptions(string, bool, bool, bool, Rectangle) {#constructor_3}

Initialiseert een nieuw exemplaar van het[`PageTextAreaOptions`](../../pagetextareaoptions) klasse.

```csharp
public PageTextAreaOptions(string expression, bool matchCase, bool uniteSegments, 
    bool ignoreFormatting, Rectangle rectangle)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| expression | String | De reguliere expressie. |
| matchCase | Boolean | De waarde die aangeeft of een hoofdlettergebruik niet wordt genegeerd. |
| uniteSegments | Boolean | De waarde die aangeeft of segmenten verenigd zijn. |
| ignoreFormatting | Boolean | De waarde die aangeeft of tekstopmaak wordt genegeerd. |
| rectangle | Rectangle | Het rechthoekige gebied dat paginagebieden bevat. |

### Zie ook

* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [PageTextAreaOptions](../../pagetextareaoptions)
* naamruimte [GroupDocs.Parser.Options](../../pagetextareaoptions)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
