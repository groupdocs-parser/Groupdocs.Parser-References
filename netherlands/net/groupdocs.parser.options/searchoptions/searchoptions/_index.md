---
title: SearchOptions
second_title: GroupDocs.Parser voor .NET API-referentie
description: Initialiseert een nieuw exemplaar van hetSearchOptionsgroupdocs.parser.options/searchoptions klasse.
type: docs
weight: 10
url: /nl/net/groupdocs.parser.options/searchoptions/searchoptions/
---
## SearchOptions(bool, bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_3}

Initialiseert een nieuw exemplaar van het[`SearchOptions`](../../searchoptions) klasse.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages, HighlightOptions leftHighlightOptions, 
    HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een hoofdlettergebruik niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekstzoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
| searchByPages | Boolean | De waarde die aangeeft of de zoekopdracht per pagina wordt uitgevoerd. |
| leftHighlightOptions | HighlightOptions | De opties voor de linkermarkering. |
| rightHighlightOptions | HighlightOptions | De opties voor de juiste highlight. |

### Zie ook

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* naamruimte [GroupDocs.Parser.Options](../../searchoptions)
* montage [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions, HighlightOptions) {#constructor_5}

Initialiseert een nieuw exemplaar van het[`SearchOptions`](../../searchoptions) klasse die wordt gebruikt om te zoeken met de markeringsopties voor extractie van de linker en rechter markering.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions leftHighlightOptions, HighlightOptions rightHighlightOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een hoofdlettergebruik niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekstzoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
| leftHighlightOptions | HighlightOptions | De opties voor de linkermarkering. |
| rightHighlightOptions | HighlightOptions | De opties voor de juiste highlight. |

### Zie ook

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* naamruimte [GroupDocs.Parser.Options](../../searchoptions)
* montage [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, HighlightOptions) {#constructor_4}

Initialiseert een nieuw exemplaar van het[`SearchOptions`](../../searchoptions) klasse die wordt gebruikt om te zoeken met dezelfde highlight-opties voor de extractie van linker- en rechterhighlights.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    HighlightOptions highlightOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een hoofdlettergebruik niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekstzoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
| highlightOptions | HighlightOptions | De opties voor beide hoogtepunten. |

### Zie ook

* class [HighlightOptions](../../highlightoptions)
* class [SearchOptions](../../searchoptions)
* naamruimte [GroupDocs.Parser.Options](../../searchoptions)
* montage [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`SearchOptions`](../../searchoptions) klasse die wordt gebruikt om te zoeken zonder highlight-extractie.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een hoofdlettergebruik niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekstzoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |

### Zie ook

* class [SearchOptions](../../searchoptions)
* naamruimte [GroupDocs.Parser.Options](../../searchoptions)
* montage [GroupDocs.Parser](../../../)

---

## SearchOptions(bool, bool, bool, bool) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`SearchOptions`](../../searchoptions)klasse die wordt gebruikt om te zoeken op pagina's en zonder extractie van hoogtepunten.

```csharp
public SearchOptions(bool matchCase, bool matchWholeWord, bool useRegularExpression, 
    bool searchByPages)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| matchCase | Boolean | De waarde die aangeeft of een hoofdlettergebruik niet wordt genegeerd. |
| matchWholeWord | Boolean | De waarde die aangeeft of tekstzoeken beperkt is tot een heel woord. |
| useRegularExpression | Boolean | De waarde die aangeeft of een reguliere expressie wordt gebruikt. |
| searchByPages | Boolean | De waarde die aangeeft of de zoekopdracht per pagina wordt uitgevoerd. |

### Zie ook

* class [SearchOptions](../../searchoptions)
* naamruimte [GroupDocs.Parser.Options](../../searchoptions)
* montage [GroupDocs.Parser](../../../)

---

## SearchOptions() {#constructor}

Initialiseert een nieuw exemplaar van het[`SearchOptions`](../../searchoptions) klasse met standaardwaarden. Zie opmerkingen voor details.

```csharp
public SearchOptions()
```

### Opmerkingen

De volgende eigenschappen hebben standaardwaarden:

**[`MatchCase`](../matchcase)**

`vals`

**[`MatchWholeWord`](../matchwholeword)**

`vals`

**[`UseRegularExpression`](../useregularexpression)**

`vals`

**[`LeftHighlightOptions`](../lefthighlightoptions)**

`nul`

**[`RightHighlightOptions`](../righthighlightoptions)**

`nul`

### Zie ook

* class [SearchOptions](../../searchoptions)
* naamruimte [GroupDocs.Parser.Options](../../searchoptions)
* montage [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
